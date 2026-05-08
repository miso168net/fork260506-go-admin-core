---
type: community
cohesion: 0.19
members: 15
---

# Config Settings & Multi-DB

**Cohesion:** 0.19 - loosely connected
**Members:** 15 nodes

## Members
- [[.Init()_8]] - code - sdk/config/config.go
- [[.OnChange()]] - code - sdk/config/config.go
- [[.multiDatabase()]] - code - sdk/config/config.go
- [[.runCallback()]] - code - sdk/config/config.go
- [[GetConfig()]] - code - sdk/config/config.go
- [[Settings]] - code - sdk/config/config.go
- [[Setup()_1]] - code - sdk/config/config.go
- [[WithEntity()]] - code - config/options.go
- [[WithLoader()]] - code - config/options.go
- [[WithReader()]] - code - config/loader/memory/options.go
- [[WithSource()]] - code - config/loader/memory/options.go
- [[config.go_2]] - code - sdk/config/config.go
- [[handleError()]] - code - sdk/config/config.go
- [[options.go_1]] - code - config/loader/memory/options.go
- [[options.go]] - code - config/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Settings__Multi-DB
SORT file.name ASC
```

## Connections to other communities
- 4 edges to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Default Config Tests]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]

## Top bridge nodes
- [[handleError()]] - degree 4, connects to 2 communities
- [[.multiDatabase()]] - degree 3, connects to 2 communities
- [[.Init()_8]] - degree 6, connects to 1 community
- [[Setup()_1]] - degree 6, connects to 1 community
- [[config.go_2]] - degree 5, connects to 1 community