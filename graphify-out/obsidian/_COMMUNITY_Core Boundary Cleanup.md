---
type: community
cohesion: 0.50
members: 4
---

# Core Boundary Cleanup

**Cohesion:** 0.50 - moderately connected
**Members:** 4 nodes

## Members
- [[Core boundary infra-only, no business logic]] - document - docs/architecture/code-review-core-boundary.md
- [[Removed legacy sdkpkgloggeroptions.go]] - document - docs/architecture/code-review-core-boundary.md
- [[Removed sdkpkgmiddlewarerequest_logger.go (business rule)]] - document - docs/architecture/code-review-core-boundary.md
- [[Simplified SetupLogger from 68 to 11 lines]] - document - docs/architecture/code-review-core-boundary.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Core_Boundary_Cleanup
SORT file.name ASC
```
