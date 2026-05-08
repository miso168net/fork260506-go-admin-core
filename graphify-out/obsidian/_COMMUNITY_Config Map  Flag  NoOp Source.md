---
type: community
cohesion: 0.13
members: 17
---

# Config Map / Flag / NoOp Source

**Cohesion:** 0.13 - loosely connected
**Members:** 17 nodes

## Members
- [[.Map()]] - code - config/default.go
- [[.Map()_1]] - code - config/reader/json/values.go
- [[.Next()_2]] - code - config/source/noop.go
- [[.Read()_1]] - code - config/source/flag/flag.go
- [[.Stop()_2]] - code - config/source/noop.go
- [[.String()_11]] - code - config/source/flag/flag.go
- [[.StringMap()_1]] - code - config/reader/json/values.go
- [[.Watch()_3]] - code - config/source/flag/flag.go
- [[.Write()_1]] - code - config/source/flag/flag.go
- [[Map()]] - code - config/config.go
- [[NewNoopWatcher()]] - code - config/source/noop.go
- [[NewSource()_1]] - code - config/source/flag/flag.go
- [[flag.go]] - code - config/source/flag/flag.go
- [[flagsrc]] - code - config/source/flag/flag.go
- [[noop.go]] - code - config/source/noop.go
- [[noopWatcher]] - code - config/source/noop.go
- [[reverse()]] - code - config/source/flag/flag.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Map_/_Flag_/_NoOp_Source
SORT file.name ASC
```

## Connections to other communities
- 3 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_Source Watcher]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]

## Top bridge nodes
- [[.Read()_1]] - degree 8, connects to 4 communities
- [[.Map()_1]] - degree 6, connects to 2 communities
- [[flag.go]] - degree 4, connects to 1 community
- [[reverse()]] - degree 3, connects to 1 community
- [[.Map()]] - degree 2, connects to 1 community