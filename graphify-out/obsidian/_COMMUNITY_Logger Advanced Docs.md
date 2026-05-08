---
type: community
cohesion: 0.09
members: 29
---

# Logger Advanced Docs

**Cohesion:** 0.09 - loosely connected
**Members:** 29 nodes

## Members
- [[3-phase migration v1.6.0 to v2.0.0]] - document - docs/architecture/logging-architecture.md
- [[4-phase upgrade plan (compat - Zap - structured - sampling)]] - document - docs/migration/logger-upgrade-v1.6.0.md
- [[Async Logger (45x boost)]] - document - README.md
- [[Async docs (channel queue, dropblocksample policy, OnDropped)]] - document - logger/README_ADVANCED.md
- [[Combination order Sanitizer - Sampling - Async]] - document - logger/README_ADVANCED.md
- [[Controllability problems (PII leak, no audit)]] - document - docs/architecture/logging-architecture.md
- [[Field zero-allocation system]] - document - docs/architecture/logger-architecture-v2.md
- [[Four-Layer Architecture (AppCoreAdapterPluginWriter)]] - document - docs/architecture/logger-architecture-v2.md
- [[Identified perf problems (no sampling, copy overhead, sync write)]] - document - docs/architecture/logging-architecture.md
- [[Layered logging architecture (BusinessMiddlewareCoreWriter)]] - document - docs/architecture/logging-architecture.md
- [[Logger Interface (minimal) + StructuredLogger (extended)]] - document - docs/architecture/logger-architecture-v2.md
- [[Logging Architecture PDF (printable, 10pp)]] - document - docs/architecture/logging-architecture.pdf
- [[P0 Fix Sampling shared-state bug via samplingState pointer]] - document - docs/architecture/code-review-fixes.md
- [[Perf comparison Default 12000 vs Zap 400 vs Sampling 24 nsop]] - document - docs/migration/logger-upgrade-v1.6.0.md
- [[Plugin Execution Order Sanitize-Tracing-Metrics-Sampling-Async]] - document - docs/architecture/logger-architecture-v2.md
- [[Production-Grade Combined Config (Sanitizer to Sampling to Async)]] - document - README.md
- [[Proposal RequestLogger middleware (skipsanitizetrace extraction)]] - document - docs/architecture/logging-architecture.md
- [[Proposal SamplingConfig (InitialThereafterTick)]] - document - docs/architecture/logging-architecture.md
- [[Proposal WithSanitize (MaskAllMaskPartialMaskHash)]] - document - docs/architecture/logging-architecture.md
- [[Proposal zap-based Logger (zero alloc)]] - document - docs/architecture/logging-architecture.md
- [[Rationale 101 ROI (3wk effort, 30wk return)]] - document - docs/architecture/logging-architecture.md
- [[Rationale ErrorFatal bypass async to avoid loss]] - document - logger/README_ADVANCED.md
- [[Sampling Logger (29x boost)]] - document - README.md
- [[Sampling docs (per-window N initial then 1M)]] - document - logger/README_ADVANCED.md
- [[Sanitizer Logger (PII redaction)]] - document - README.md
- [[Sanitizer docs (maskhashremove strategies, default rules)]] - document - logger/README_ADVANCED.md
- [[Unified YAML Config (coreadapteroutputplugins)]] - document - docs/architecture/logger-architecture-v2.md
- [[Usability problems (no structured, no context, no trace_id)]] - document - docs/architecture/logging-architecture.md
- [[v1.6.0 Zap + Sampling logger introduction]] - document - docs/migration/logger-upgrade-v1.6.0.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Advanced_Docs
SORT file.name ASC
```
