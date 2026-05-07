# Feature Specification: `response` Package (default + antd presets)

**Feature Branch**: `n/a — descriptive spec for existing module`
**Created**: 2026-05-07
**Status**: Draft (descriptive — documents existing behavior, no code change implied)
**Input**: Brainstorming session 2026-05-07 — initial spec-kit document for the
fork; user picked existing-feature documentation, both presets, with an
Observations section instead of code edits.

## Purpose & Reading Notes

This spec records the **as-is contract** of the `response/` package
(`response/return.go`, `response/type.go`) and its `response/antd/`
sub-package (`response/antd/return.go`, `response/antd/model.go`). It is a
*descriptive* spec: it describes what the code does today so that future
contributors and AI agents can reason about the boundary without re-reading
implementation files.

It is **not** a redesign. Where the current behavior looks suspicious,
findings are captured in §"Observations & Open Questions" rather than turned
into requirements. Anything in §Requirements is a fact about the code today.

## User Scenarios & Testing *(mandatory)*

The "user" of this package is a downstream Go developer (e.g., a `go-admin`
HTTP handler) who has a `*gin.Context` and wants to terminate the request
with a JSON body that follows one of the two presets.

### User Story 1 — Return a successful API response (Priority: P1)

A handler computed a result and wants to ship it back as a successful JSON
response with a trace ID, leaving HTTP transport status at 200 OK.

**Why this priority**: This is the most common path through the package and
both presets exist primarily to serve it.

**Independent Test**: Call the relevant preset's success function inside a
gin handler with synthetic context; assert the JSON body shape, the
`c.Set("result", …)` value, and the recorded HTTP status.

**Acceptance Scenarios**:

1. **Given** a `*gin.Context` and arbitrary `data interface{}`,
   **When** `response.OK(c, data, "")` is called,
   **Then** the response body is a `response{ Response{ RequestId, Code:200,
   Msg:"", Status:"" }, Data:data }`, the trace ID is populated from
   `pkg.GenerateMsgIDFromContext(c)`, `c.Get("result")` returns that struct,
   `c.Get("status")` returns `200`, and the request is aborted with HTTP 200.
2. **Given** the same context and a non-empty `msg`,
   **When** `response.OK(c, data, msg)` is called,
   **Then** `Response.Msg` equals `msg` (other fields per Scenario 1).
3. **Given** a `*gin.Context` and a payload,
   **When** `antd.OK(c, data)` is called,
   **Then** the body is `response{ Response{ Success:true, Status:"done",
   TraceId, Host:"" }, Data:data }`, `c.Get("result")` returns that struct,
   `c.Get("status")` returns `200`, and the request is aborted with HTTP 200.
4. **Given** the same antd context,
   **When** `antd.UpFileOK(c, data)` is called,
   **Then** the response is identical to `antd.OK(c, data)` (Scenario 3).

### User Story 2 — Return an error response (Priority: P1)

A handler hit a failure (validation error, downstream timeout, etc.) and
wants to return a structured error to the caller without using a non-200
HTTP status.

**Why this priority**: Error returns are as frequent as successes and the
two presets diverge most visibly here (int code vs string code).

**Independent Test**: Call each preset's `Error` with representative inputs;
assert the body shape, code encoding, and the `c.Set("status", …)` value.

**Acceptance Scenarios**:

1. **Given** a context and `code=400`, `err=errors.New("bad input")`,
   `msg=""`,
   **When** `response.Error(c, code, err, msg)` is called,
   **Then** the body is `response{ Response{ RequestId, Code:400,
   Msg:"bad input", Status:"error" }, Data:nil }`, `c.Get("status")`
   returns `400`, and the HTTP transport status is 200.
2. **Given** a context and `code=500`, `err=errors.New("x")`, `msg="boom"`,
   **When** `response.Error(c, code, err, msg)` is called,
   **Then** `Response.Msg == "boom"` (the explicit `msg` overrides
   `err.Error()`).
3. **Given** an antd context and `errCode="C400"`, `errMsg="bad input"`,
   `showType="2"`,
   **When** `antd.Error(c, errCode, errMsg, showType)` is called,
   **Then** the body is `response{ Response{ Success:false, ErrorCode:"C400",
   ErrorMessage:"bad input", ShowType:"2", TraceId, Status:"" } }`,
   `c.Get("status")` returns `"C400"` (string), and the HTTP transport status
   is 200.

### User Story 3 — Return a paginated list (Priority: P2)

A handler fetched a page of records and wants to return both the rows and
the page metadata in a shape the front-end can paginate against.

**Why this priority**: List endpoints are common but less frequent than
the single-resource cases in US1/US2.

**Independent Test**: Call each pagination function with a known list,
total, page index, and page size; assert the JSON shape and trace ID.

**Acceptance Scenarios**:

1. **Given** `result=[…]`, `count=42`, `pageIndex=2`, `pageSize=20`, `msg=""`,
   **When** `response.PageOK(c, result, count, pageIndex, pageSize, msg)`
   is called,
   **Then** the response wraps a `page{ Page{ Count:42, PageIndex:2,
   PageSize:20 }, List:result }` inside `Data` of the default success body
   (per US1 Scenario 1).
2. **Given** `result=[…]`, `total=42`, `current=2`, `pageSize=20`,
   **When** `antd.PageOK(c, result, total, current, pageSize)` is called,
   **Then** the body is a `pages{ Pages{ Response{Success:true, TraceId},
   Total:42, Current:2, PageSize:20 }, Data:result }` (note the antd-
   specific naming `total/current` instead of `count/pageIndex`).
3. **Given** the same antd inputs,
   **When** `antd.ListOK(c, result, total, current, pageSize)` is called,
   **Then** the body is a `lists{ Response{Success:true, TraceId},
   ListData{ List:result, Total, Current, PageSize } }` — the rows are
   nested one level deeper under `data.list` rather than at `data`.

### User Story 4 — Return a custom-shaped response (Priority: P3)

A handler wants to ship a payload that does not fit either preset's
struct (e.g., a one-off integration response) but still wants a trace ID
attached and the standard middleware hooks set.

**Why this priority**: Escape hatch; rarely used but documented in the API.

**Independent Test**: Call `Custum` with a hand-built `gin.H` and assert
that the trace key is injected and the body matches the input plus that
key.

**Acceptance Scenarios**:

1. **Given** `data = gin.H{"foo": "bar"}`,
   **When** `response.Custum(c, data)` is called,
   **Then** the body equals `gin.H{"foo":"bar", "requestId":<traceID>}`,
   `c.Get("result")` returns the same map, and the HTTP transport status
   is 200. (No `c.Set("status", …)` is called.)
2. **Given** the same `data`,
   **When** `antd.Custum(c, data)` is called,
   **Then** the body equals `gin.H{"foo":"bar", "traceId":<traceID>}`
   (note the **different key name**), `c.Get("result")` returns the same
   map, and HTTP transport status is 200.

### User Story 5 — Plug a custom `Responses` implementation (Priority: P3)

A consumer wants to use a third response shape (e.g., JSON:API) without
forking the package. They construct a struct that implements the
`response.Responses` interface and assign it to `response.Default`.

**Why this priority**: The interface exists and `Default` is exported, but
this is rarely exercised; documenting the contract is what matters.

**Independent Test**: Replace `response.Default` with a fake that records
calls; invoke `response.OK`/`response.Error` and verify the recorded
sequence matches the contract.

**Acceptance Scenarios**:

1. **Given** a custom struct `X` implementing `Responses`,
   **When** `response.Default = X{}` and a handler calls `response.OK(c,
   data, "msg")`,
   **Then** the package calls, in this order, `Default.Clone()`,
   `SetData(data)`, `SetSuccess(true)`, `SetMsg("msg")`,
   `SetTraceID(<id>)`, `SetCode(200)`, then aborts with the cloned value.
2. **Given** the same setup,
   **When** the handler calls `response.Error(c, 500, err, "boom")`,
   **Then** the call order is `Clone()`, `SetMsg(err.Error())`,
   `SetMsg("boom")`, `SetTraceID(<id>)`, `SetCode(500)`,
   `SetSuccess(false)`. (Note: `SetMsg` is called twice when both `err`
   and `msg` are non-empty — see Observations.)

### Edge Cases

- **Nil `gin.Context`**: not handled; package will panic. Documented as
  caller responsibility.
- **Empty `msg` and nil `err` in `response.Error`**: produces a response
  with `Msg:""` and `Status:"error"`. The caller is responsible for
  passing at least one signal.
- **`response.Custum` with a key that collides with `requestId`**: the
  package overwrites it with the generated trace ID.
- **`antd.Custum` with a key that collides with `traceId`**: same
  overwrite behavior, but on the `traceId` key.
- **`antd.Error` with `errCode == "200"` or `errCode == "0"`**: the
  numeric `SetCode` path on the underlying struct treats those as
  success, but the public `antd.Error` accepts `errCode` as a free-form
  string and writes it directly without going through `SetCode`. So
  `antd.Error(c, "200", …)` ships `success:false, errorCode:"200"` —
  semantically self-contradictory.

## Requirements *(mandatory)*

These describe the package's current contract.

### Functional Requirements

- **FR-001**: Every response body produced by `OK`, `Error`, `PageOK`,
  `UpFileOK`, `ListOK`, and `Custum` (in either preset) MUST include a
  trace identifier obtained from `pkg.GenerateMsgIDFromContext(c)`.
  - In default preset, the field is named `requestId`.
  - In antd preset, the field is named `traceId`.
- **FR-002**: All terminating calls MUST use `c.AbortWithStatusJSON(
  http.StatusOK, …)`. The HTTP transport status is therefore always 200,
  regardless of semantic success or failure. Semantic outcome is conveyed
  in the body.
- **FR-003**: The default preset's `Code` field MUST hold the int passed
  to `Error` (typically an HTTP status code), and `Status` MUST be set to
  `"error"` when `SetSuccess(false)` is called. `SetSuccess(true)` does
  NOT clear `Status` or set it to `"success"`.
- **FR-004**: The antd preset's `ErrorCode` field MUST be the string
  passed to `Error` verbatim. The `SetCode(int32)` method on the antd
  struct produces an `ErrorCode` of the form `"C<num>"` for non-{0,200}
  codes, but this method is only reachable through the
  `Responses`-interface path (US5), not through the public `antd.Error`.
- **FR-005**: Both `OK` paths MUST call `Clone()` on the configured
  `Default` before mutating state, ensuring no shared state across
  concurrent requests. (The default implementation's `Clone()` is a
  value-copy; future custom implementations MUST preserve this
  invariant.)
- **FR-006**: Every terminating call MUST publish two values to the gin
  context for downstream middleware:
  - `c.Set("result", <body struct or map>)` — the exact value sent.
  - `c.Set("status", <code>)` — the int (default), HTTP 200 (success
    paths), or the original `errCode` string (antd error path).
  - `Custum` (both presets) is the lone exception: it sets `result` only,
    not `status`.
- **FR-007**: When `response.Error` is given a non-empty `msg` AND a
  non-nil `err`, the explicit `msg` MUST take precedence; the package
  records this by calling `SetMsg` twice (first with `err.Error()`, then
  with `msg`).
- **FR-008**: Pagination shapes are preset-specific and MUST NOT be
  cross-mapped:
  - Default: `Page{Count, PageIndex, PageSize}` + `List` field, with rows
    placed at `data.list`.
  - antd `PageOK`: rows at `data` (top-level under the response), with
    `total/current/pageSize` siblings.
  - antd `ListOK`: rows at `data.list`, with `total/current/pageSize`
    siblings of `list`.
- **FR-009**: The `response.Default` symbol MUST be a swappable, package-
  level `Responses`. Reassignment is the public extension point. The
  package is NOT goroutine-safe across reassignments — callers MUST
  reassign before serving requests.
- **FR-010**: Constants `Silent="0"`, `MessageWarn="1"`,
  `MessageError="2"`, `Notification="4"`, `Page="9"` in `response/antd`
  MUST be the only sanctioned values for `ShowType`. The package does
  not validate this; callers are trusted.

### Key Entities

- **`Responses` (interface, `response/type.go`)**: Six methods —
  `SetCode(int32)`, `SetTraceID(string)`, `SetMsg(string)`,
  `SetData(interface{})`, `SetSuccess(bool)`, `Clone() Responses`.
  Implemented by the default `response` struct and the antd `response`
  struct.
- **`Response` (default, `response/type.go`)**: Public fields
  `RequestId`, `Code (int32)`, `Msg`, `Status`. Wire-tagged for
  protobuf and JSON.
- **`response` (default, unexported)**: Embeds `Response`, adds
  `Data interface{}`. The actual body type returned to clients.
- **`Page` / `page` (default)**: `Page{Count, PageIndex, PageSize}`;
  `page` embeds `Page` plus `List interface{}`.
- **`Response` (antd, `response/antd/model.go`)**: Public fields
  `Success`, `ErrorCode`, `ErrorMessage`, `ShowType`, `TraceId`,
  `Host`, `Status`.
- **`response` (antd, unexported)**: Embeds antd `Response`, adds `Data
  interface{}` (with `omitempty`). The body type for `OK`/`Error`/
  `Custum`.
- **`Pages` / `pages` (antd)**: `Pages{Response, Data, Total, Current,
  PageSize}`; `pages` embeds `Pages` and re-declares `Data interface{}`
  — effectively a Go field-shadowing pattern (see Observations).
- **`lists` (antd, unexported)**: `{Response, ListData}`. Used by
  `ListOK`.
- **`ListData` (antd)**: `{List, Total, Current, PageSize}`.

## Success Criteria *(mandatory)*

These are measurable invariants a reviewer can check against any tagged
release of this package.

- **SC-001**: 100% of responses produced by the package's exported
  functions (in either preset) carry a non-empty trace identifier when
  `pkg.GenerateMsgIDFromContext` returns a non-empty value. Mechanically:
  every public function above includes a call to that function before
  abort.
- **SC-002**: The HTTP transport status is 200 for 100% of code paths
  through `OK`, `Error`, `PageOK`, `UpFileOK`, `ListOK`, and `Custum`.
- **SC-003**: For any single request, exactly one terminating call (one
  of the six functions above) is sufficient to produce a complete body;
  no combination of two is required.
- **SC-004**: Within a single preset, success and error responses share
  the same outer JSON skeleton (`requestId/code/msg/status` for default;
  `success/errorCode/errorMessage/showType/traceId/host/status` for
  antd). A consumer can write a single decoder per preset.
- **SC-005**: External dependencies are limited to the standard library
  (`net/http`, `fmt`) and `github.com/gin-gonic/gin`. The only in-repo
  dependency is `github.com/go-admin-team/go-admin-core/sdk/pkg` for
  trace-ID generation. The `response/antd` sub-package additionally
  imports the parent `response` package to satisfy the `Responses`
  interface return type from `Clone()`. Verifiable from the import
  blocks of `return.go`, `type.go`, `antd/return.go`, and
  `antd/model.go`.

## Assumptions

- Callers always operate inside a gin handler chain and possess a valid
  `*gin.Context`. No nil-check is performed.
- `pkg.GenerateMsgIDFromContext(c)` is available, side-effect-free, and
  produces a string suitable for both `requestId` and `traceId` fields.
- A request invokes at most one terminating call from this package; the
  second would race with the abort already issued.
- The two presets are alternatives, not layers: a project picks one and
  imports either `response` or `response/antd`, but not both per
  endpoint.
- Front-ends understand HTTP-200-with-body-error semantics; clients that
  expect non-2xx for failures need to be adapted upstream.
- `response.Default` is configured (or left at its zero-value default)
  before the HTTP server starts serving traffic.

## Observations & Open Questions

These are findings noted while writing the spec. Each is a candidate for
a separate spec / fix; none are addressed here.

- **O-1 — `OK` signature drift between presets**: default `OK(c, data,
  msg)` accepts a message; antd `OK(c, data)` does not. A consumer that
  wants to switch presets cannot do so by import-rename alone.
  *Question*: was the `msg` parameter on default `OK` deliberate, or a
  legacy from before antd existed?
- **O-2 — Error code type asymmetry**: default uses `int`, antd uses
  `string`. A central error helper that funnels into either preset has
  to fork at the boundary. *Question*: is there an internal mapping
  convention (e.g., antd `"C400"` ↔ default `400`) the maintainers
  expect?
- **O-3 — `c.AbortWithStatusJSON(http.StatusOK, …)` for errors**: keeps
  the HTTP transport on 200 even for failures. *Question*: is this a
  deliberate front-end contract (Ant Design Pro convention) or an early
  decision that has stuck around?
- **O-4 — `Pages` / `pages` field shadowing in antd**: `pages` embeds
  `Pages` and redeclares `Data interface{}`. The outer `Data` shadows
  the inner one, but only `pages.Data` is set in `PageOK`, and the
  embedded `Pages.Data` ends up zero. The JSON tag (`omitempty`)
  hides this in output. *Question*: is the inner `Data` field intended
  to be removed?
- **O-5 — Trace field name divergence**: default `Custum` injects
  `requestId`, antd `Custum` injects `traceId`. Same value, different
  key name within the same package directory. *Question*: should
  callers of `Custum` standardize on one key?
- **O-6 — `SetSuccess` asymmetry in default preset**: `SetSuccess(true)`
  is a no-op on `Status`; `SetSuccess(false)` writes `"error"`. So a
  caller cannot transition a response from error back to success
  through this method alone. *Question*: should success set
  `Status:"success"` (or `""`) explicitly?
- **O-7 — `antd.Error` bypasses `SetCode`**: the public `antd.Error`
  writes `ErrorCode` directly from a string argument and never calls
  `SetCode(int32)`. The `C<num>` formatting logic in `SetCode` is
  therefore dead code along the public path. It is only reachable when
  a custom `Responses` is plugged in (US5) and goes through the
  default `Error` flow… but the default `Error` only exists in the
  *default* preset, not antd. *Question*: is the antd `SetCode`
  method live, or vestigial?
- **O-8 — `Custum` does not call `c.Set("status", …)`**: every other
  terminating call in the package does. Middleware that reads
  `c.Get("status")` cannot distinguish "Custum used" from "missing
  middleware". *Question*: is this deliberate (Custum is fully escape-
  hatch) or an oversight?
- **O-9 — `Host` field in antd `Response` is never populated**: the
  struct declares it, the JSON tag is present, but no code path writes
  to it. *Question*: dead field, or intended to be filled by a
  middleware not in this package?

## Out of Scope

- Changing the package's behavior, signatures, or JSON shapes.
- Adding tests for the existing behavior. (A separate plan would do
  that under Constitution Principle III.)
- Reconciling the default and antd presets, or deprecating one.
- Documenting `pkg.GenerateMsgIDFromContext` internals.
- Documenting consumers of `c.Get("result")` / `c.Get("status")`.

---

*Generated via `/superpowers:brainstorming` on 2026-05-07. Companion to
the project constitution v1.0.0 ratified the same day.*
