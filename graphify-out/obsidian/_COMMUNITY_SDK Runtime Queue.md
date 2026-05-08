---
type: community
cohesion: 0.33
members: 6
---

# SDK Runtime Queue

**Cohesion:** 0.33 - loosely connected
**Members:** 6 nodes

## Members
- [[.GetMemoryQueue()]] - code - sdk/runtime/application.go
- [[.GetQueue()]] - code - sdk/runtime/application.go
- [[.GetQueueAdapter()]] - code - sdk/runtime/application.go
- [[.GetQueuePrefix()]] - code - sdk/runtime/application.go
- [[NewQueue()]] - code - sdk/runtime/queue.go
- [[queue.go_1]] - code - sdk/runtime/queue.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/SDK_Runtime_Queue
SORT file.name ASC
```

## Connections to other communities
- 4 edges to [[_COMMUNITY_SDK Runtime Application]]
- 2 edges to [[_COMMUNITY_SDK App Tenant Methods]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 1 edge to [[_COMMUNITY_Memory Queue Operations]]

## Top bridge nodes
- [[.GetQueue()]] - degree 3, connects to 2 communities
- [[.GetQueueAdapter()]] - degree 3, connects to 2 communities
- [[NewQueue()]] - degree 6, connects to 1 community
- [[.GetQueuePrefix()]] - degree 3, connects to 1 community
- [[.GetMemoryQueue()]] - degree 2, connects to 1 community