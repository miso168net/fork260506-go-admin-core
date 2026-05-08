---
type: community
cohesion: 0.08
members: 33
---

# File / Path Utils

**Cohesion:** 0.08 - loosely connected
**Members:** 33 nodes

## Members
- [[.DoWork()]] - code - sdk/pkg/file.go
- [[.Info()_6]] - code - sdk/pkg/ws/ws.go
- [[.LenClient()]] - code - sdk/pkg/ws/ws.go
- [[.LenGroup()]] - code - sdk/pkg/ws/ws.go
- [[.RegisterClient()]] - code - sdk/pkg/ws/ws.go
- [[.Send()]] - code - sdk/pkg/ws/ws.go
- [[.SendAll()]] - code - sdk/pkg/ws/ws.go
- [[.SendAllService()]] - code - sdk/pkg/ws/ws.go
- [[.SendGroup()]] - code - sdk/pkg/ws/ws.go
- [[.SendGroupService()]] - code - sdk/pkg/ws/ws.go
- [[.SendService()]] - code - sdk/pkg/ws/ws.go
- [[.Start()]] - code - sdk/pkg/ws/ws.go
- [[.UnRegisterClient()]] - code - sdk/pkg/ws/ws.go
- [[.UnWsClient()]] - code - sdk/pkg/ws/ws.go
- [[.WsClient()]] - code - sdk/pkg/ws/ws.go
- [[.walkCallback()]] - code - sdk/pkg/file.go
- [[BroadCastMessageData]] - code - sdk/pkg/ws/ws.go
- [[Client]] - code - sdk/pkg/ws/ws.go
- [[FileCreate()]] - code - sdk/pkg/file.go
- [[FileMonitoringById()]] - code - sdk/pkg/file.go
- [[GetCurrentPath()]] - code - sdk/pkg/file.go
- [[GroupMessageData]] - code - sdk/pkg/ws/ws.go
- [[Manager]] - code - sdk/pkg/ws/ws.go
- [[MessageData]] - code - sdk/pkg/ws/ws.go
- [[PathCreate()]] - code - sdk/pkg/file.go
- [[PathExist()]] - code - sdk/pkg/file.go
- [[ReplaceHelper]] - code - sdk/pkg/file.go
- [[SendAll()]] - code - sdk/pkg/ws/ws.go
- [[SendGroup()]] - code - sdk/pkg/ws/ws.go
- [[SendOne()]] - code - sdk/pkg/ws/ws.go
- [[WsLogout()]] - code - sdk/pkg/ws/ws.go
- [[file.go_2]] - code - sdk/pkg/file.go
- [[ws.go]] - code - sdk/pkg/ws/ws.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/File_/_Path_Utils
SORT file.name ASC
```

## Connections to other communities
- 8 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_Audit OptionsReader]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]

## Top bridge nodes
- [[FileMonitoringById()]] - degree 5, connects to 3 communities
- [[.WsClient()]] - degree 5, connects to 2 communities
- [[Client]] - degree 3, connects to 2 communities
- [[.Start()]] - degree 3, connects to 2 communities
- [[.Info()_6]] - degree 8, connects to 1 community