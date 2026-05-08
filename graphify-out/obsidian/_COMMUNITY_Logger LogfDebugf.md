---
type: community
cohesion: 0.20
members: 10
---

# Logger Logf/Debugf

**Cohesion:** 0.20 - loosely connected
**Members:** 10 nodes

## Members
- [[.Logf()_3]] - code - logger/logrus.go
- [[.getEntryWithCaller()]] - code - logger/logrus.go
- [[Debugf()]] - code - logger/level.go
- [[Infof()]] - code - logger/level.go
- [[Setup()]] - code - casbin/mycasbin.go
- [[Warnf()]] - code - logger/level.go
- [[formatCaller()]] - code - logger/logrus.go
- [[mycasbin.go]] - code - casbin/mycasbin.go
- [[shouldSkipFrame()]] - code - logger/logrus.go
- [[updateCallback()]] - code - casbin/mycasbin.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Logf/Debugf
SORT file.name ASC
```

## Connections to other communities
- 4 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 3 edges to [[_COMMUNITY_Level Functions]]
- 3 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_Logger Hooks (CallerElasticsearch)]]
- 1 edge to [[_COMMUNITY_antd_api Wrapper]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Config Loader Memory]]
- 1 edge to [[_COMMUNITY_Listener & HTTP Server Options]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]

## Top bridge nodes
- [[.Logf()_3]] - degree 7, connects to 3 communities
- [[Infof()]] - degree 5, connects to 3 communities
- [[updateCallback()]] - degree 5, connects to 3 communities
- [[.getEntryWithCaller()]] - degree 6, connects to 2 communities
- [[Debugf()]] - degree 3, connects to 2 communities