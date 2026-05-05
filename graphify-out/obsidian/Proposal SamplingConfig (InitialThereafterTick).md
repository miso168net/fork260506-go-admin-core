---
source_file: "docs/architecture/logging-architecture.md"
type: "document"
community: "Logger Architecture Docs"
location: "#### 2.2.2 性能优化组件"
tags:
  - graphify/document
  - graphify/INFERRED
  - community/Logger_Architecture_Docs
---

# Proposal: SamplingConfig (Initial/Thereafter/Tick)

## Connections
- [[Identified perf problems (no sampling, copy overhead, sync write)]] - `rationale_for` [EXTRACTED]
- [[P0 Fix Sampling shared-state bug via samplingState pointer]] - `implements` [INFERRED]
- [[Sampling docs (per-window N initial then 1M)]] - `implements` [INFERRED]

#graphify/document #graphify/INFERRED #community/Logger_Architecture_Docs