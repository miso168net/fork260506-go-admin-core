---
type: community
cohesion: 0.17
members: 16
---

# Sampling Logger

**Cohesion:** 0.17 - loosely connected
**Members:** 16 nodes

## Members
- [[.Debug()_3]] - code - logger/sampling.go
- [[.Error()_4]] - code - logger/sampling.go
- [[.Fields()_4]] - code - logger/sampling.go
- [[.Info()_3]] - code - logger/sampling.go
- [[.Log()_4]] - code - logger/sampling.go
- [[.Logf()_4]] - code - logger/sampling.go
- [[.Options()_5]] - code - logger/sampling.go
- [[.String()_19]] - code - logger/sampling.go
- [[.Sync()_5]] - code - logger/sampling.go
- [[.Warn()_3]] - code - logger/sampling.go
- [[.shouldSample()]] - code - logger/sampling.go
- [[SamplingConfig]] - code - logger/sampling.go
- [[extendedLogger]] - code - logger/sampling.go
- [[sampling.go]] - code - logger/sampling.go
- [[samplingLogger]] - code - logger/sampling.go
- [[samplingState]] - code - logger/sampling.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Sampling_Logger
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]

## Top bridge nodes
- [[samplingLogger]] - degree 15, connects to 3 communities
- [[sampling.go]] - degree 5, connects to 1 community
- [[.Debug()_3]] - degree 3, connects to 1 community
- [[.Info()_3]] - degree 3, connects to 1 community
- [[.Log()_4]] - degree 3, connects to 1 community