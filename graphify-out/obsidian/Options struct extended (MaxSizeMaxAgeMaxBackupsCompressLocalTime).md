---
source_file: "docs/architecture/code-optimization-v2.md"
type: "document"
community: "Options Refactor Rationale"
location: "#### 1. 扩展 Options 结构体"
tags:
  - graphify/document
  - graphify/EXTRACTED
  - community/Options_Refactor_Rationale
---

# Options struct extended (MaxSize/MaxAge/MaxBackups/Compress/LocalTime)

## Connections
- [[DefaultOptions() reuse pattern]] - `references` [EXTRACTED]
- [[Hardcoded lumberjack rotation problem]] - `rationale_for` [EXTRACTED]
- [[P1 Fix Options.Stdout string to bool]] - `shares_data_with` [INFERRED]
- [[factory.buildAdapterOptions Config wiring]] - `shares_data_with` [EXTRACTED]
- [[sdkconfiglogger.go uses new Option system]] - `references` [INFERRED]

#graphify/document #graphify/EXTRACTED #community/Options_Refactor_Rationale