---
type: community
cohesion: 0.13
members: 16
---

# Logger Hooks (Caller/Elasticsearch)

**Cohesion:** 0.13 - loosely connected
**Members:** 16 nodes

## Members
- [[.Fire()_2]] - code - logger/logrus.go
- [[.Fire()_1]] - code - logger/logrus.go
- [[.Fire()]] - code - logger/logrus.go
- [[.Levels()_2]] - code - logger/logrus.go
- [[.Levels()_1]] - code - logger/logrus.go
- [[.Levels()]] - code - logger/logrus.go
- [[CallerHook]] - code - logger/logrus.go
- [[ElasticsearchHook]] - code - logger/logrus.go
- [[NewCallerHook()]] - code - logger/logrus.go
- [[NewElasticsearchHook()]] - code - logger/logrus.go
- [[NewSentryHook()]] - code - logger/logrus.go
- [[SentryHook]] - code - logger/logrus.go
- [[init()_3]] - code - logger/logrus.go
- [[logrus.go]] - code - logger/logrus.go
- [[sourceDir()]] - code - logger/logrus.go
- [[toLogrusLevel()]] - code - logger/logrus.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Hooks_Caller/Elasticsearch
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_Logger LogfDebugf]]
- 1 edge to [[_COMMUNITY_Config Loader Memory]]
- 1 edge to [[_COMMUNITY_Metrics Hook]]
- 1 edge to [[_COMMUNITY_Logrus AddHook]]

## Top bridge nodes
- [[logrus.go]] - degree 16, connects to 5 communities
- [[.Fire()_2]] - degree 2, connects to 1 community
- [[toLogrusLevel()]] - degree 2, connects to 1 community