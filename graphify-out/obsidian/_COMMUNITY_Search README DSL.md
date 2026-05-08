---
type: community
cohesion: 1.00
members: 1
---

# Search README DSL

**Cohesion:** 1.00 - tightly connected
**Members:** 1 nodes

## Members
- [[Search struct-tag DSL (exactcontainsgtinorder)]] - document - tools/search/README.md

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Search_README_DSL
SORT file.name ASC
```
