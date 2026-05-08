---
type: community
cohesion: 0.18
members: 13
---

# Memory Queue Operations

**Cohesion:** 0.18 - loosely connected
**Members:** 13 nodes

## Members
- [[.GetErrorCount()]] - code - storage/queue/message.go
- [[.Register()_1]] - code - storage/queue/memory.go
- [[.Register()]] - code - sdk/runtime/queue.go
- [[.Run()]] - code - sdk/runtime/queue.go
- [[.SetErrorCount()]] - code - storage/queue/message.go
- [[.Shutdown()_2]] - code - storage/queue/memory.go
- [[.Shutdown()]] - code - sdk/runtime/queue.go
- [[.String()_24]] - code - sdk/runtime/queue.go
- [[.makeQueue()]] - code - storage/queue/memory.go
- [[Memory_1]] - code - storage/queue/memory.go
- [[Queue_1]] - code - sdk/runtime/queue.go
- [[memory.go_3]] - code - storage/queue/memory.go
- [[queue]] - code - storage/queue/memory.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Memory_Queue_Operations
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_Memory Queue Append]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 2 edges to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Field Constructors]]
- 1 edge to [[_COMMUNITY_SDK Runtime Queue]]
- 1 edge to [[_COMMUNITY_Listener & HTTP Server Options]]
- 1 edge to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]

## Top bridge nodes
- [[.Register()_1]] - degree 10, connects to 4 communities
- [[Memory_1]] - degree 7, connects to 3 communities
- [[Queue_1]] - degree 6, connects to 2 communities
- [[.Shutdown()_2]] - degree 4, connects to 2 communities
- [[.makeQueue()]] - degree 3, connects to 1 community