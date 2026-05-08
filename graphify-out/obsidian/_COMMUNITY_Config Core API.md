---
type: community
cohesion: 0.19
members: 20
---

# Config Core API

**Cohesion:** 0.19 - loosely connected
**Members:** 20 nodes

## Members
- [[.Bytes()]] - code - config/default.go
- [[.Close()]] - code - config/default.go
- [[.Get()_1]] - code - config/default.go
- [[.Init()]] - code - config/default.go
- [[.Load()]] - code - config/default.go
- [[.Next()]] - code - config/default.go
- [[.Options()]] - code - config/default.go
- [[.Scan()]] - code - config/default.go
- [[.Snapshot()]] - code - config/loader/memory/memory.go
- [[.Stop()]] - code - config/default.go
- [[.String()]] - code - config/default.go
- [[.Sync()]] - code - config/default.go
- [[.Values()]] - code - config/reader/json/json.go
- [[.Watch()]] - code - config/default.go
- [[.run()]] - code - config/default.go
- [[Config]] - code - sdk/config/config.go
- [[Equal()]] - code - errors/errors.go
- [[default.go]] - code - config/default.go
- [[newConfig()]] - code - config/default.go
- [[watcher]] - code - config/default.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Core_API
SORT file.name ASC
```

## Connections to other communities
- 12 edges to [[_COMMUNITY_Config Loader Memory]]
- 4 edges to [[_COMMUNITY_Config Settings & Multi-DB]]
- 3 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_Config Top-Level]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_Config Value Types]]
- 1 edge to [[_COMMUNITY_TOML Encoder]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Config Loader]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]

## Top bridge nodes
- [[Config]] - degree 18, connects to 5 communities
- [[.Values()]] - degree 13, connects to 4 communities
- [[.Init()]] - degree 9, connects to 3 communities
- [[.run()]] - degree 10, connects to 2 communities
- [[.Snapshot()]] - degree 7, connects to 2 communities