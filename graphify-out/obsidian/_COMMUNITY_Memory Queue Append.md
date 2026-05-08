---
type: community
cohesion: 0.16
members: 19
---

# Memory Queue Append

**Cohesion:** 0.16 - loosely connected
**Members:** 19 nodes

## Members
- [[.Append()_1]] - code - storage/queue/memory.go
- [[.Append()]] - code - sdk/runtime/queue.go
- [[.GetID()_1]] - code - storage/queue/message.go
- [[.GetPrefix()_1]] - code - storage/queue/message.go
- [[.GetStream()_1]] - code - storage/queue/message.go
- [[.GetStreamMessage()]] - code - sdk/runtime/application.go
- [[.GetValues()_1]] - code - storage/queue/message.go
- [[.SetAppRouters()]] - code - sdk/runtime/application.go
- [[.SetBefore()]] - code - sdk/runtime/application.go
- [[.SetHandlerByTenant()]] - code - sdk/runtime/application.go
- [[.SetID()_1]] - code - storage/queue/message.go
- [[.SetPrefix()_2]] - code - storage/queue/message.go
- [[.SetStream()_1]] - code - storage/queue/message.go
- [[.SetValues()_1]] - code - storage/queue/message.go
- [[Message_1]] - code - storage/queue/message.go
- [[TestMemory_Append()]] - code - storage/queue/memory_test.go
- [[TestMemory_Register()]] - code - storage/queue/memory_test.go
- [[memory_test.go_1]] - code - storage/queue/memory_test.go
- [[message.go_1]] - code - storage/queue/message.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Memory_Queue_Append
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_Memory Queue Operations]]
- 6 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 5 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 5 edges to [[_COMMUNITY_SDK Runtime Application]]
- 3 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_Config Loader Memory]]
- 2 edges to [[_COMMUNITY_Logger Examples]]
- 2 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 2 edges to [[_COMMUNITY_antd_api Bind Constructor]]
- 2 edges to [[_COMMUNITY_API Bind Constructor]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_Search FieldTag DSL]]
- 2 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Config Settings & Multi-DB]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_Default Config Tests]]
- 1 edge to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 1 edge to [[_COMMUNITY_SDK App Tenant Methods]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]

## Top bridge nodes
- [[.Append()_1]] - degree 46, connects to 18 communities
- [[TestMemory_Register()]] - degree 8, connects to 4 communities
- [[TestMemory_Append()]] - degree 5, connects to 2 communities
- [[Message_1]] - degree 11, connects to 1 community
- [[.GetStreamMessage()]] - degree 4, connects to 1 community