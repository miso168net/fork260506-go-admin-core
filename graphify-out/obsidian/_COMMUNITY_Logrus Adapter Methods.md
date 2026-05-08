---
type: community
cohesion: 0.20
members: 18
---

# Logrus Adapter Methods

**Cohesion:** 0.20 - loosely connected
**Members:** 18 nodes

## Members
- [[.Debug()_2]] - code - logger/logrus.go
- [[.Error()_3]] - code - logger/logrus.go
- [[.Fields()_3]] - code - logger/logrus.go
- [[.GetLogrusLogger()]] - code - logger/logrus.go
- [[.Info()_2]] - code - logger/logrus.go
- [[.Init()_4]] - code - logger/logrus.go
- [[.Log()_3]] - code - logger/logrus.go
- [[.Options()_4]] - code - logger/logrus.go
- [[.SetFormatter()]] - code - logger/logrus.go
- [[.String()_18]] - code - logger/logrus.go
- [[.Sync()_3]] - code - logger/logrus.go
- [[.Warn()_2]] - code - logger/logrus.go
- [[.With()_1]] - code - logger/logrus.go
- [[.WithContext()_1]] - code - logger/logrus.go
- [[WithFields()]] - code - logger/options.go
- [[extractContextFields()]] - code - logger/zap.go
- [[logrusAdapter]] - code - logger/logrus.go
- [[toLogrusFields()]] - code - logger/logrus.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logrus_Adapter_Methods
SORT file.name ASC
```

## Connections to other communities
- 11 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 3 edges to [[_COMMUNITY_File Source + GORM Logger]]
- 3 edges to [[_COMMUNITY_Logger LogfDebugf]]
- 3 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_Logger Hooks (CallerElasticsearch)]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 2 edges to [[_COMMUNITY_antd_api Wrapper]]
- 1 edge to [[_COMMUNITY_Logger Examples]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Logrus AddHook]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_Logger Setup & Adapter]]

## Top bridge nodes
- [[WithFields()]] - degree 13, connects to 5 communities
- [[logrusAdapter]] - degree 18, connects to 3 communities
- [[extractContextFields()]] - degree 4, connects to 3 communities
- [[.Log()_3]] - degree 7, connects to 2 communities
- [[toLogrusFields()]] - degree 7, connects to 2 communities