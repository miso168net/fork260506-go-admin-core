---
type: community
cohesion: 0.20
members: 18
---

# Async/Sampling/Sanitizer/Zap Combinators

**Cohesion:** 0.20 - loosely connected
**Members:** 18 nodes

## Members
- [[.Debug()_5]] - code - logger/zap.go
- [[.Error()_6]] - code - logger/zap.go
- [[.Info()_5]] - code - logger/zap.go
- [[.Init()_7]] - code - logger/zap.go
- [[.Log()_6]] - code - logger/zap.go
- [[.Options()_7]] - code - logger/zap.go
- [[.String()_21]] - code - logger/zap.go
- [[.Warn()_5]] - code - logger/zap.go
- [[.With()]] - code - logger/async.go
- [[.With()_3]] - code - logger/sampling.go
- [[.With()_4]] - code - logger/sanitizer.go
- [[.With()_5]] - code - logger/zap.go
- [[DefaultOptions()]] - code - logger/options.go
- [[NewZapLogger()]] - code - logger/zap.go
- [[toZapFields()]] - code - logger/zap.go
- [[toZapLevel()]] - code - logger/zap.go
- [[zap.go]] - code - logger/zap.go
- [[zapLogger]] - code - logger/zap.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Async/Sampling/Sanitizer/Zap_Combinators
SORT file.name ASC
```

## Connections to other communities
- 13 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 6 edges to [[_COMMUNITY_Field Constructors]]
- 6 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 4 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 2 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 2 edges to [[_COMMUNITY_Sampling Logger]]
- 2 edges to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_Logger Examples]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Masking Core (PII Mask)]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]

## Top bridge nodes
- [[.Debug()_5]] - degree 9, connects to 6 communities
- [[NewZapLogger()]] - degree 12, connects to 5 communities
- [[zapLogger]] - degree 15, connects to 3 communities
- [[.With()_5]] - degree 8, connects to 3 communities
- [[toZapFields()]] - degree 13, connects to 2 communities