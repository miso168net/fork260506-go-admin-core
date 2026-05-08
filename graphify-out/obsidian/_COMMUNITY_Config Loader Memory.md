---
type: community
cohesion: 0.22
members: 20
---

# Config Loader Memory

**Cohesion:** 0.22 - loosely connected
**Members:** 20 nodes

## Members
- [[.Close()_1]] - code - config/loader/memory/memory.go
- [[.Get()_2]] - code - config/loader/memory/memory.go
- [[.Next()_1]] - code - config/source/memory/watcher.go
- [[.Read()_2]] - code - config/source/memory/memory.go
- [[.Stop()_1]] - code - config/source/memory/watcher.go
- [[.String()_6]] - code - config/source/memory/memory.go
- [[.Sync()_1]] - code - config/loader/memory/memory.go
- [[.Update()]] - code - config/source/memory/memory.go
- [[.Watch()_1]] - code - config/source/memory/memory.go
- [[.Write()_2]] - code - config/source/memory/memory.go
- [[.loaded()]] - code - config/loader/memory/memory.go
- [[.reload()]] - code - config/loader/memory/memory.go
- [[Merge()]] - code - tools/poster/poster.go
- [[NewLoader()]] - code - config/loader/memory/memory.go
- [[genVer()]] - code - config/loader/memory/memory.go
- [[memory]] - code - config/source/memory/memory.go
- [[memory.go]] - code - config/loader/memory/memory.go
- [[updateValue]] - code - config/loader/memory/memory.go
- [[watcher_1]] - code - config/source/memory/watcher.go
- [[watcher.go_1]] - code - config/source/memory/watcher.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Loader_Memory
SORT file.name ASC
```

## Connections to other communities
- 12 edges to [[_COMMUNITY_Config Core API]]
- 7 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 6 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 4 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 3 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 2 edges to [[_COMMUNITY_Source Watcher]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_TOML Encoder]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Logger LogfDebugf]]
- 1 edge to [[_COMMUNITY_Logger Hooks (CallerElasticsearch)]]
- 1 edge to [[_COMMUNITY_Logger Context + Poster Image]]

## Top bridge nodes
- [[.Next()_1]] - degree 16, connects to 8 communities
- [[.Sync()_1]] - degree 12, connects to 6 communities
- [[.Watch()_1]] - degree 15, connects to 4 communities
- [[.Update()]] - degree 11, connects to 4 communities
- [[NewLoader()]] - degree 7, connects to 4 communities