---
type: community
cohesion: 0.25
members: 8
---

# Audit FormatFunc & Stream

**Cohesion:** 0.25 - loosely connected
**Members:** 8 nodes

## Members
- [[FormatFunc]] - code - observe/audit/log.go
- [[JSONFormat()]] - code - observability/audit/deprecated.go
- [[JSONFormat()_1]] - code - observe/audit/log.go
- [[Record]] - code - observe/audit/log.go
- [[Stream]] - code - observe/audit/log.go
- [[TextFormat()]] - code - observability/audit/deprecated.go
- [[TextFormat()_1]] - code - observe/audit/log.go
- [[log.go_1]] - code - observe/audit/log.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Audit_FormatFunc__Stream
SORT file.name ASC
```

## Connections to other communities
- 3 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_Audit OptionsReader]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]

## Top bridge nodes
- [[TextFormat()_1]] - degree 4, connects to 2 communities
- [[log.go_1]] - degree 6, connects to 1 community
- [[JSONFormat()_1]] - degree 3, connects to 1 community
- [[JSONFormat()]] - degree 2, connects to 1 community
- [[TextFormat()]] - degree 2, connects to 1 community