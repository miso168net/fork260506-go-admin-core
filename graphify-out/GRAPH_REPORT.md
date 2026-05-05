# Graph Report - .  (2026-05-06)

## Corpus Check
- 184 files · ~60,121 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 1373 nodes · 3110 edges · 54 communities detected
- Extraction: 51% EXTRACTED · 49% INFERRED · 0% AMBIGUOUS · INFERRED: 1530 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- [[_COMMUNITY_Logger Performance Tests|Logger Performance Tests]]
- [[_COMMUNITY_Config Core API|Config Core API]]
- [[_COMMUNITY_Storage & Response Models|Storage & Response Models]]
- [[_COMMUNITY_Captcha & Preprocessor Tools|Captcha & Preprocessor Tools]]
- [[_COMMUNITY_SDK Binding & Pagination|SDK Binding & Pagination]]
- [[_COMMUNITY_Config Reader & Observe|Config Reader & Observe]]
- [[_COMMUNITY_Logger Setup & Adapter|Logger Setup & Adapter]]
- [[_COMMUNITY_SDK Application Container|SDK Application Container]]
- [[_COMMUNITY_Errors & File Watcher|Errors & File Watcher]]
- [[_COMMUNITY_Hash & Field Values|Hash & Field Values]]
- [[_COMMUNITY_Log Formatter & Color|Log Formatter & Color]]
- [[_COMMUNITY_Logrus Adapter Methods|Logrus Adapter Methods]]
- [[_COMMUNITY_Sampling & Extended Logger|Sampling & Extended Logger]]
- [[_COMMUNITY_API Context & Response|API Context & Response]]
- [[_COMMUNITY_Configure & Settings|Configure & Settings]]
- [[_COMMUNITY_File Utils & WebSocket|File Utils & WebSocket]]
- [[_COMMUNITY_HTTP Server Options|HTTP Server Options]]
- [[_COMMUNITY_Logger Architecture Docs|Logger Architecture Docs]]
- [[_COMMUNITY_Image & Context Tools|Image & Context Tools]]
- [[_COMMUNITY_v1.6 Migration & Compat|v1.6 Migration & Compat]]
- [[_COMMUNITY_Terminal Text Colors|Terminal Text Colors]]
- [[_COMMUNITY_API Exception Responses|API Exception Responses]]
- [[_COMMUNITY_Storage Message Stream|Storage Message Stream]]
- [[_COMMUNITY_HTTP Response Builder|HTTP Response Builder]]
- [[_COMMUNITY_Options Refactor Rationale|Options Refactor Rationale]]
- [[_COMMUNITY_JSON Encoder|JSON Encoder]]
- [[_COMMUNITY_XML Encoder|XML Encoder]]
- [[_COMMUNITY_Storage Adapter Types|Storage Adapter Types]]
- [[_COMMUNITY_Config Source Adapters|Config Source Adapters]]
- [[_COMMUNITY_Config Reader Types|Config Reader Types]]
- [[_COMMUNITY_v1.6.0-alpha Changes|v1.6.0-alpha Changes]]
- [[_COMMUNITY_Core Boundary Cleanup|Core Boundary Cleanup]]
- [[_COMMUNITY_Database Resolver Config|Database Resolver Config]]
- [[_COMMUNITY_Runtime ModeEnv|Runtime Mode/Env]]
- [[_COMMUNITY_Server Manager|Server Manager]]
- [[_COMMUNITY_Tools Configure|Tools Configure]]
- [[_COMMUNITY_Zap FD Leak Fix|Zap FD Leak Fix]]
- [[_COMMUNITY_Config Encoder Interface|Config Encoder Interface]]
- [[_COMMUNITY_Error Code Strings|Error Code Strings]]
- [[_COMMUNITY_ErrorCoder Type|ErrorCoder Type]]
- [[_COMMUNITY_Response Type|Response Type]]
- [[_COMMUNITY_Application Type|Application Type]]
- [[_COMMUNITY_Gen Type|Gen Type]]
- [[_COMMUNITY_JWT Type|JWT Type]]
- [[_COMMUNITY_SSL Type|SSL Type]]
- [[_COMMUNITY_Deprecated Setup|Deprecated Setup]]
- [[_COMMUNITY_Runtime Type|Runtime Type]]
- [[_COMMUNITY_Logrus Adapter Doc|Logrus Adapter Doc]]
- [[_COMMUNITY_Fork Branch Origin|Fork Branch Origin]]
- [[_COMMUNITY_Logrus Default Rationale|Logrus Default Rationale]]
- [[_COMMUNITY_Config Changeset|Config Changeset]]
- [[_COMMUNITY_Application Singleton|Application Singleton]]
- [[_COMMUNITY_File-Open Error Fix|File-Open Error Fix]]
- [[_COMMUNITY_Search DSL|Search DSL]]

## God Nodes (most connected - your core abstractions)
1. `Log` - 94 edges
2. `NewLogrusLogger()` - 82 edges
3. `WithLevel()` - 72 edges
4. `Application` - 62 edges
5. `WithOutput()` - 61 edges
6. `Errorf()` - 44 edges
7. `New()` - 43 edges
8. `NewSanitizerLogger()` - 27 edges
9. `NewAsyncLogger()` - 26 edges
10. `GinJWTMiddleware` - 22 edges

## Surprising Connections (you probably didn't know these)
- `Logging Architecture PDF (printable, 10pp)` --semantically_similar_to--> `Layered logging architecture (Business/Middleware/Core/Writer)`  [INFERRED] [semantically similar]
  docs/architecture/logging-architecture.pdf → docs/architecture/logging-architecture.md
- `Logging Architecture PDF (printable, 10pp)` --semantically_similar_to--> `Proposal: zap-based Logger (zero alloc)`  [INFERRED] [semantically similar]
  docs/architecture/logging-architecture.pdf → docs/architecture/logging-architecture.md
- `Info()` --calls--> `Log`  [INFERRED]
  logger/level.go → observe/audit/log.go
- `Trace()` --calls--> `Log`  [INFERRED]
  logger/level.go → observe/audit/log.go
- `Debug()` --calls--> `Log`  [INFERRED]
  logger/level.go → observe/audit/log.go

## Hyperedges (group relationships)
- **v1.6.0 Package Migration Program (planning, impl, test, review, docs)** — v160plan_refactor_goals, changelog_package_relocation, changelog_compat_layers, intgtest_31_passing, migrcr_v160beta_approval, v15tov16_migration_guide, tools_readme_migrate_script [EXTRACTED 0.95]
- **Production Logger Pipeline: Sanitizer + Sampling + Async** — readme_production_config, loggeradv_combination_order, loggerarchv2_plugin_order, loggeradv_sanitizer_section, loggeradv_sampling_section, loggeradv_async_section [EXTRACTED 0.90]
- **Logger architecture evolution: problems -> v1 design -> v2 design -> implementation -> code-review fixes** — loggingarch_problem_perf, loggingarch_zap_proposal, loggerarchv2_four_layer, loggerupgrade_v160_zap_intro, fixes_sampling_state_bug [INFERRED 0.80]

## Communities

### Community 0 - "Logger Performance Tests"
Cohesion: 0.08
Nodes (80): BenchmarkAsync(), BenchmarkSampling(), BenchmarkSanitizer(), TestAsyncPerformance(), TestCombinedFeatures(), TestSampling(), TestSanitizer(), NewAsyncLogger() (+72 more)

### Community 1 - "Config Core API"
Cohesion: 0.03
Nodes (39): Bytes(), Config, Map(), watcher, newConfig(), Bool(), file, NewSource() (+31 more)

### Community 2 - "Storage & Response Models"
Cohesion: 0.04
Nodes (34): ListData, lists, Pages, Response, item, Memory, cacheStore, Cache (+26 more)

### Community 3 - "Captcha & Preprocessor Tools"
Cohesion: 0.04
Nodes (51): configJsonBody, DriverDigitFunc(), DriverStringFunc(), Verify(), Scan(), DriverDigitFunc(), DriverStringFunc(), New() (+43 more)

### Community 4 - "SDK Binding & Pagination"
Cohesion: 0.04
Nodes (31): bindConstructor, bindConstructor, Pagination, SysUserOrder, SysUserSearch, TestResolve(), makeTag(), ConvertNumToChars() (+23 more)

### Community 5 - "Config Reader & Observe"
Cohesion: 0.04
Nodes (59): NewConfig(), FormatFunc, Option, Options, ReadOption, ReadOptions, Record, Stream (+51 more)

### Community 6 - "Logger Setup & Adapter"
Cohesion: 0.04
Nodes (59): DefaultConfig(), FromLegacyConfig(), isValidLevel(), Logger, RotationConfig, copyFields(), init(), logCallerfilePath() (+51 more)

### Community 7 - "SDK Application Container"
Cohesion: 0.04
Nodes (6): NewCache(), NewQueue(), Application, Config, Router, Routers

### Community 8 - "Errors & File Watcher"
Cohesion: 0.05
Nodes (17): Equal(), Error, ErrorCode, FromError(), New(), Parse(), file_errors_proto_init(), file_errors_proto_rawDescGZIP() (+9 more)

### Community 9 - "Hash & Field Values"
Cohesion: 0.06
Nodes (40): Crc16Hash(), Crc32Hash(), Crc8Hash(), BenchmarkZapLoggerStructured(), value, BenchmarkLogrusLogger(), ExampleNewFromConfig(), ExampleNewLogrusLogger() (+32 more)

### Community 10 - "Log Formatter & Color"
Cohesion: 0.06
Nodes (23): sprint(), toString(), formatDuration(), formatField(), formatGormLog(), getLevelColor(), isKeyField(), stripAnsiCodes() (+15 more)

### Community 11 - "Logrus Adapter Methods"
Cohesion: 0.04
Nodes (29): ExampleNewLogrusLogger_addHook(), Debug(), Debugf(), Error(), GetLevel(), Info(), Infof(), Trace() (+21 more)

### Community 12 - "Sampling & Extended Logger"
Cohesion: 0.05
Nodes (15): ExampleNewDevelopmentLogger(), Any(), Time(), extendedLogger, SamplingConfig, samplingLogger, samplingState, SanitizerConfig (+7 more)

### Community 13 - "API Context & Response"
Cohesion: 0.07
Nodes (14): Api, Api, loggerKey, Custum(), Error(), OK(), PageOK(), NewHelper() (+6 more)

### Community 14 - "Configure & Settings"
Cohesion: 0.06
Nodes (24): handleError(), NewResolverConfigure(), Settings, Setup(), TestDBConfig_Init(), DBConfig, DBResolverConfig, CheckExist() (+16 more)

### Community 15 - "File Utils & WebSocket"
Cohesion: 0.08
Nodes (12): FileCreate(), FileMonitoringById(), ReplaceHelper, BroadCastMessageData, Client, GroupMessageData, Manager, MessageData (+4 more)

### Community 16 - "HTTP Server Options"
Cohesion: 0.08
Nodes (13): Handler(), Option, options, Server, setDefaultOption(), setDefaultOptions(), New(), NewHealthz() (+5 more)

### Community 17 - "Logger Architecture Docs"
Cohesion: 0.09
Nodes (29): P0 Fix: Sampling shared-state bug via samplingState pointer, Async docs (channel queue, drop/block/sample policy, OnDropped), Combination order: Sanitizer -> Sampling -> Async, Rationale: Error/Fatal bypass async to avoid loss, Sampling docs (per-window N initial then 1/M), Sanitizer docs (mask/hash/remove strategies, default rules), Unified YAML Config (core/adapter/output/plugins), Field zero-allocation system (+21 more)

### Community 18 - "Image & Context Tools"
Cohesion: 0.13
Nodes (9): FromContext(), NewContext(), loggerKey, DImage, DText, GetQRImage(), NewPNG(), Pt (+1 more)

### Community 19 - "v1.6 Migration & Compat"
Cohesion: 0.21
Nodes (14): Compatibility Layers (deprecated.go), tools/migrate-v1.6.sh Migration Script, Package Relocation (sdk/pkg to root), v1.6.0-beta Release, Integration Tests: 31/31 passing, Cross-path validation (new <-> old), v1.6.0-beta Code Review Approval, Zero-cost type alias verification (+6 more)

### Community 20 - "Terminal Text Colors"
Cohesion: 0.38
Nodes (9): Black(), Blue(), Cyan(), Green(), Magenta(), Red(), SetColor(), White() (+1 more)

### Community 21 - "API Exception Responses"
Cohesion: 0.33
Nodes (8): AuthError(), newAPIException(), NotFound(), ParameterError(), ResponseJson(), ServerError(), UnknownError(), APIException

### Community 22 - "Storage Message Stream"
Cohesion: 0.2
Nodes (1): Message

### Community 23 - "HTTP Response Builder"
Cohesion: 0.22
Nodes (2): Page, Response

### Community 24 - "Options Refactor Rationale"
Cohesion: 0.29
Nodes (7): DefaultOptions() reuse pattern, factory.buildAdapterOptions Config wiring, Hardcoded lumberjack rotation problem, Options struct extended (MaxSize/MaxAge/MaxBackups/Compress/LocalTime), Rationale: config-code separation principle, sdk/config/logger.go uses new Option system, P1 Fix: Options.Stdout string to bool

### Community 25 - "JSON Encoder"
Cohesion: 0.33
Nodes (1): jsonEncoder

### Community 26 - "XML Encoder"
Cohesion: 0.33
Nodes (1): xmlEncoder

### Community 27 - "Storage Adapter Types"
Cohesion: 0.33
Nodes (5): AdapterCache, AdapterLocker, AdapterQueue, ConsumerFunc, Messager

### Community 28 - "Config Source Adapters"
Cohesion: 0.5
Nodes (5): config.NewConfig + file.NewSource Test, File Source (yaml/json/toml/xml), Flag Source (CLI flag mapping), Memory Source (in-memory JSON), config.Setup with FileSource

### Community 29 - "Config Reader Types"
Cohesion: 0.5
Nodes (3): Reader, Value, Values

### Community 30 - "v1.6.0-alpha Changes"
Cohesion: 0.5
Nodes (4): Removed Logrus Plugin Support, Single Module Architecture (4 go.mod to 1), v1.6.0-alpha Release, Standardize on Zap as Recommended Logger

### Community 31 - "Core Boundary Cleanup"
Cohesion: 0.5
Nodes (4): Core boundary: infra-only, no business logic, Removed legacy sdk/pkg/logger/options.go, Removed sdk/pkg/middleware/request_logger.go (business rule), Simplified SetupLogger from 68 to 11 lines

### Community 32 - "Database Resolver Config"
Cohesion: 0.67
Nodes (2): Database, DBResolverConfig

### Community 33 - "Runtime Mode/Env"
Cohesion: 0.67
Nodes (1): Mode

### Community 34 - "Server Manager"
Cohesion: 0.67
Nodes (2): Manager, Runnable

### Community 35 - "Tools Configure"
Cohesion: 0.67
Nodes (2): Configure, ResolverConfigure

### Community 36 - "Zap FD Leak Fix"
Cohesion: 0.67
Nodes (3): Logger.Close() new API, P1 Fix: Init() cleans old resources, P0 Fix: Zap file descriptor leak

### Community 37 - "Config Encoder Interface"
Cohesion: 1.0
Nodes (1): Encoder

### Community 38 - "Error Code Strings"
Cohesion: 1.0
Nodes (0): 

### Community 39 - "ErrorCoder Type"
Cohesion: 1.0
Nodes (1): ErrorCoder

### Community 40 - "Response Type"
Cohesion: 1.0
Nodes (1): Responses

### Community 41 - "Application Type"
Cohesion: 1.0
Nodes (1): Application

### Community 42 - "Gen Type"
Cohesion: 1.0
Nodes (1): Gen

### Community 43 - "JWT Type"
Cohesion: 1.0
Nodes (1): Jwt

### Community 44 - "SSL Type"
Cohesion: 1.0
Nodes (1): Ssl

### Community 45 - "Deprecated Setup"
Cohesion: 1.0
Nodes (0): 

### Community 46 - "Runtime Type"
Cohesion: 1.0
Nodes (1): Runtime

### Community 47 - "Logrus Adapter Doc"
Cohesion: 1.0
Nodes (2): logger.NewLogrusLogger Factory, Logrus Adapter (50+ hooks)

### Community 48 - "Fork Branch Origin"
Cohesion: 1.0
Nodes (2): main branch forked from dev (2026-05-06), Upstream master stale 3y5m rationale

### Community 49 - "Logrus Default Rationale"
Cohesion: 1.0
Nodes (2): Logrus chosen as default adapter, Rationale: ecosystem (50+ hooks) outweighs raw speed

### Community 50 - "Config Changeset"
Cohesion: 1.0
Nodes (0): 

### Community 51 - "Application Singleton"
Cohesion: 1.0
Nodes (0): 

### Community 52 - "File-Open Error Fix"
Cohesion: 1.0
Nodes (1): P0 Fix: File-open error warning to stderr

### Community 53 - "Search DSL"
Cohesion: 1.0
Nodes (1): Search struct-tag DSL (exact/contains/gt/in/order)

## Knowledge Gaps
- **144 isolated node(s):** `configJsonBody`, `Entity`, `Options`, `Option`, `Encoder` (+139 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **Thin community `Config Encoder Interface`** (2 nodes): `encoder.go`, `Encoder`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Error Code Strings`** (2 nodes): `_()`, `error_code_string.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `ErrorCoder Type`** (2 nodes): `ErrorCoder`, `type.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Response Type`** (2 nodes): `Responses`, `type.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Application Type`** (2 nodes): `Application`, `application.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Gen Type`** (2 nodes): `Gen`, `gen.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `JWT Type`** (2 nodes): `Jwt`, `jwt.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `SSL Type`** (2 nodes): `Ssl`, `ssl.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Deprecated Setup`** (2 nodes): `Setup()`, `deprecated.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Runtime Type`** (2 nodes): `Runtime`, `type.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Logrus Adapter Doc`** (2 nodes): `logger.NewLogrusLogger Factory`, `Logrus Adapter (50+ hooks)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Fork Branch Origin`** (2 nodes): `main branch forked from dev (2026-05-06)`, `Upstream master stale 3y5m rationale`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Logrus Default Rationale`** (2 nodes): `Logrus chosen as default adapter`, `Rationale: ecosystem (50+ hooks) outweighs raw speed`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Config Changeset`** (1 nodes): `changeset.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Application Singleton`** (1 nodes): `application.go`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `File-Open Error Fix`** (1 nodes): `P0 Fix: File-open error warning to stderr`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.
- **Thin community `Search DSL`** (1 nodes): `Search struct-tag DSL (exact/contains/gt/in/order)`
  Too small to be a meaningful cluster - may be noise or needs more connections extracted.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `NewLogrusLogger()` connect `Logger Performance Tests` to `Config Core API`, `Captcha & Preprocessor Tools`, `SDK Binding & Pagination`, `Logger Setup & Adapter`, `Hash & Field Values`, `Log Formatter & Color`, `Logrus Adapter Methods`, `Sampling & Extended Logger`?**
  _High betweenness centrality (0.078) - this node is a cross-community bridge._
- **Why does `New()` connect `Captcha & Preprocessor Tools` to `Logger Performance Tests`, `Config Core API`, `Storage & Response Models`, `SDK Binding & Pagination`, `Config Reader & Observe`, `Hash & Field Values`, `Log Formatter & Color`, `Sampling & Extended Logger`, `API Context & Response`, `Configure & Settings`, `Image & Context Tools`?**
  _High betweenness centrality (0.070) - this node is a cross-community bridge._
- **Why does `Application` connect `SDK Application Container` to `SDK Binding & Pagination`?**
  _High betweenness centrality (0.065) - this node is a cross-community bridge._
- **Are the 93 inferred relationships involving `Log` (e.g. with `TestCaptchaCompatibility()` and `TestJWTAuthCompatibility()`) actually correct?**
  _`Log` has 93 INFERRED edges - model-reasoned connections that need verification._
- **Are the 76 inferred relationships involving `NewLogrusLogger()` (e.g. with `TestSampling()` and `TestSanitizer()`) actually correct?**
  _`NewLogrusLogger()` has 76 INFERRED edges - model-reasoned connections that need verification._
- **Are the 71 inferred relationships involving `WithLevel()` (e.g. with `TestSampling()` and `TestSanitizer()`) actually correct?**
  _`WithLevel()` has 71 INFERRED edges - model-reasoned connections that need verification._
- **Are the 60 inferred relationships involving `WithOutput()` (e.g. with `TestSampling()` and `TestSanitizer()`) actually correct?**
  _`WithOutput()` has 60 INFERRED edges - model-reasoned connections that need verification._