---
type: community
cohesion: 0.29
members: 7
---

# Logger Options Refactor Rationale

**Cohesion:** 0.29 - loosely connected
**Members:** 7 nodes

## Members
- [[DefaultOptions() reuse pattern]] - document - docs/architecture/code-optimization-v2.md
- [[Hardcoded lumberjack rotation problem]] - document - docs/architecture/code-optimization-v2.md
- [[Options struct extended (MaxSizeMaxAgeMaxBackupsCompressLocalTime)]] - document - docs/architecture/code-optimization-v2.md
- [[P1 Fix Options.Stdout string to bool]] - document - docs/architecture/code-review-fixes.md
- [[Rationale config-code separation principle]] - document - docs/architecture/code-optimization-v2.md
- [[factory.buildAdapterOptions Config wiring]] - document - docs/architecture/code-optimization-v2.md
- [[sdkconfiglogger.go uses new Option system]] - document - docs/architecture/code-review-core-boundary.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Options_Refactor_Rationale
SORT file.name ASC
```
