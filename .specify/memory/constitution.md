<!--
SYNC IMPACT REPORT
Version change: (template, unfilled) → 1.0.0
Bump rationale: initial ratification — the prior file held only placeholder
tokens, so this is the first concrete adoption (MINOR-equivalent additions
from a 0.0.0 baseline are published as 1.0.0 per project convention).
Modified principles: N/A (initial ratification — five principles introduced)
Added sections:
  - Core Principles (I–V)
  - Additional Constraints & Quality Gates
  - Development Workflow
  - Governance
Removed sections: N/A (template placeholders fully replaced)
Templates requiring updates:
  - ✅ .specify/templates/plan-template.md — Constitution Check stays as a
    per-feature gate placeholder; no rule conflict introduced.
  - ✅ .specify/templates/spec-template.md — no constitution-driven sections
    affected.
  - ✅ .specify/templates/tasks-template.md — Phase N "Polish" already covers
    benchmarks/race tests required by Principle III; per-feature task lists
    must include a `-race` and (where relevant) a `-bench` task.
  - ✅ .specify/templates/checklist-template.md — not impacted by the
    principles in this version.
  - N/A .specify/templates/commands/ — directory does not exist in this repo.
  - ✅ README.md — Go 1.25+ baseline, Apache 2.0 license, and logger pipeline
    description are already consistent with the constitution.
  - N/A docs/quickstart.md — does not exist; CLAUDE.md + README.md serve as
    runtime guidance per the Governance section.
Follow-up TODOs: none.
-->

# go-admin-core Constitution

## Core Principles

### I. Core Boundary — Infrastructure Only (NON-NEGOTIABLE)

The `go-admin-core` module MUST contain only reusable infrastructure: logging,
configuration, storage adapters, server primitives, error types, captcha, JWT,
Casbin wiring, and observability. Business rules — request shaping for a
specific app, RBAC policy decisions, domain validation — MUST NOT live in this
module. Code that embeds an opinion about a particular product belongs in the
consumer (e.g., `go-admin`), not here.

**Rationale:** v1.6 cleanup explicitly removed
`sdk/pkg/middleware/request_logger.go` and collapsed `SetupLogger` from 68
lines to 11 because business policy was leaking into core. A boundary that
drifts becomes a liability for every downstream fork.

### II. Composable Adapters over Monoliths

Every feature MUST be a small, independently usable unit that composes through
documented interfaces. The production logger pipeline
(`Sanitizer → Sampling → Async`) is the canonical shape: each layer is a
`logger.Logger` and can be used alone, swapped, or reordered. New storage
backends, queues, and config sources MUST follow the same adapter-contract
pattern.

**Rationale:** Composability lets consumers pay only for what they use, and it
bounds the blast radius of a regression — a bug in `samplingState` cannot
corrupt async writes when each layer is isolated.

### III. Test-First, Race-Verified, Benchmark-Bound (NON-NEGOTIABLE)

Production code in this module MUST ship with tests written before the
implementation, exercised under `go test -race`, and — for any
performance-sensitive path — accompanied by a benchmark checked into the
repository. Concurrent code without a race-detector run is treated as broken.
Performance claims without a checked-in benchmark are treated as anecdote.

**Rationale:** The logger advertises 45×/29×/34× boosts and 100k+ QPS. Those
numbers are only trustworthy because the repo runs `-race` and `-bench` as
part of the verification loop. Removing either turns advertised behavior into
folklore.

### IV. Backward Compatibility Within a MAJOR Version

Within a single MAJOR version, package relocations MUST ship a zero-cost
compatibility shim (type alias + thin re-export), and behavior changes MUST
preserve the public API surface. Deprecations require a `deprecated.go` entry,
a documented sunset window of at least one MINOR release, and a migration
script or rewrite recipe. Anything that breaks an importing consumer requires
a MAJOR bump.

**Rationale:** v1.6 collapsed four `go.mod` files into one and relocated
`sdk/pkg/*` to the module root, yet downstream code kept compiling because the
aliases were verified zero-cost. That discipline is what lets a fork track
upstream without forking the user base.

### V. Observability is a Default, Not a Feature

Every long-lived component MUST emit structured, level-tagged logs by default.
Sensitive fields (phone, email, password, token, anything resembling a secret)
MUST be sanitized at the logger boundary, not by each call site. Sampling MUST
be configurable for high-frequency paths. Code paths that bypass the async
pipeline (e.g., `Error`, `Fatal`) MUST be documented as such so consumers can
reason about loss windows.

**Rationale:** Production users inherit our defaults. If sanitization is
opt-in, PII leaks; if sampling is opt-in, log storms cost money. The defaults
must be safe in production without configuration.

## Additional Constraints & Quality Gates

- **Language baseline:** Go 1.25.1 or higher. Changes that require a newer
  toolchain MUST bump `go.mod` and the README badge in the same commit.
- **License:** Apache 2.0. New files MUST be license-compatible; vendored code
  MUST carry an accepted notice.
- **Dependencies:** Adding a new direct dependency requires a one-line
  justification in the PR description; bumps are reviewed at version-change
  time.
- **Concurrency contracts:** Any exported type touched by more than one
  goroutine MUST document its safety guarantee (safe / external-sync-required
  / single-writer) in its godoc comment.
- **Resource hygiene:** Components that open files, sockets, or background
  goroutines MUST expose `Close() error` and MUST be covered by a leak test —
  the v1.6 zap FD-leak fix is the canonical pattern.
- **Knowledge graph freshness:** After material code changes in a working
  session, run `graphify update .` so `graphify-out/GRAPH_REPORT.md` reflects
  the current structure for future readers.

## Development Workflow

- **Specs first:** Non-trivial features go through `/speckit-specify` →
  `/speckit-plan` → `/speckit-tasks` → `/speckit-implement`. The
  `Constitution Check` gate in `plan-template.md` MUST evaluate every
  principle above before Phase 0 research, and again after Phase 1 design.
- **Branching:** Feature work happens on `###-feature-name` branches cut from
  `main`. `main` tracks the active development line (per
  `x_fork.branch-origin.md`); `master` is preserved as the historical default
  and is not used for new work.
- **Reviews:** Every PR MUST link to (a) the spec or issue, (b) test output
  including `-race`, and (c) benchmark output if a performance-sensitive path
  was touched.
- **Commits:** Commit messages SHOULD reference the principle being upheld
  when a change is principle-driven (e.g., "Principle I: move auth middleware
  out of core").

## Governance

This constitution supersedes informal practice. Where another document
conflicts with these principles, this file wins until amended.

- **Amendments:** Open a PR that edits this file plus every artifact it
  impacts (templates, README, command files). The PR description MUST contain
  a Sync Impact Report and a version-bump rationale.
- **Versioning policy (semantic):**
  - **MAJOR** — a principle is removed, redefined incompatibly, or a
    governance rule is revoked.
  - **MINOR** — a new principle or section is added, or an existing principle
    gains materially expanded normative guidance.
  - **PATCH** — clarifications, wording, typos, non-semantic refinements.
- **Compliance review:** Every `/speckit-plan` Constitution Check is a
  compliance review. Reviewers MUST reject plans that violate a principle
  without an entry in the plan's `Complexity Tracking` table justifying the
  deviation.
- **Runtime guidance:** Day-to-day "how do I do X" questions are answered by
  `CLAUDE.md`, `README.md`, and the `graphify-out/` knowledge graph — not by
  this constitution.

**Version**: 1.0.0 | **Ratified**: 2026-05-07 | **Last Amended**: 2026-05-07
