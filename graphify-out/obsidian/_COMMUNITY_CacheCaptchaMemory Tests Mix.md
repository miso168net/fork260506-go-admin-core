---
type: community
cohesion: 0.21
members: 19
---

# Cache/Captcha/Memory Tests Mix

**Cohesion:** 0.21 - loosely connected
**Members:** 19 nodes

## Members
- [[.Get()_5]] - code - storage/cache/memory.go
- [[BenchmarkSetCollect()]] - code - captcha/store_test.go
- [[Errorf()]] - code - logger/level.go
- [[NewCacheStore()]] - code - captcha/store.go
- [[NewMemory()]] - code - storage/queue/memory.go
- [[TestGetClear()]] - code - captcha/store_test.go
- [[TestMemory_Get()]] - code - storage/cache/memory_test.go
- [[TestNewCacheStore()]] - code - captcha/store_test.go
- [[TestNewMemoryQueue()]] - code - sdk/runtime/queue_test.go
- [[TestQueue_Register()]] - code - sdk/runtime/queue_test.go
- [[TestSetGet()]] - code - captcha/store_test.go
- [[TestStore_CollectNotExpire()]] - code - captcha/store_test.go
- [[TestStore_SetGoCollect()]] - code - captcha/store_test.go
- [[getStore()]] - code - captcha/store_test.go
- [[memory_test.go]] - code - storage/cache/memory_test.go
- [[queue_test.go]] - code - sdk/runtime/queue_test.go
- [[store_test.go]] - code - captcha/store_test.go
- [[transInit()]] - code - sdk/api/translate.go
- [[translate.go]] - code - sdk/api/translate.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Cache/Captcha/Memory_Tests_Mix
SORT file.name ASC
```

## Connections to other communities
- 15 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 7 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 6 edges to [[_COMMUNITY_antd Response Methods]]
- 6 edges to [[_COMMUNITY_Cache Memory Operations]]
- 4 edges to [[_COMMUNITY_Default Config Tests]]
- 4 edges to [[_COMMUNITY_Errors & File Watcher]]
- 4 edges to [[_COMMUNITY_antd_api Wrapper]]
- 3 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_Listener & HTTP Server Options]]
- 3 edges to [[_COMMUNITY_Memory Queue Append]]
- 2 edges to [[_COMMUNITY_Captcha Cache Store]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_Logger LogfDebugf]]
- 2 edges to [[_COMMUNITY_Config Core API]]
- 2 edges to [[_COMMUNITY_Config Loader Memory]]
- 2 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_Logger Examples]]
- 2 edges to [[_COMMUNITY_Level Functions]]
- 2 edges to [[_COMMUNITY_Database Resolver Config]]
- 2 edges to [[_COMMUNITY_SDK Runtime Queue]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_Logger Config Plugins]]
- 1 edge to [[_COMMUNITY_SDK Service]]
- 1 edge to [[_COMMUNITY_SDK Cache Config]]
- 1 edge to [[_COMMUNITY_SDK Queue Config]]
- 1 edge to [[_COMMUNITY_IP Helpers]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_Memory Queue Operations]]
- 1 edge to [[_COMMUNITY_Excel Writer]]
- 1 edge to [[_COMMUNITY_gRPC Header Helpers]]

## Top bridge nodes
- [[Errorf()]] - degree 44, connects to 16 communities
- [[.Get()_5]] - degree 27, connects to 15 communities
- [[NewMemory()]] - degree 13, connects to 8 communities
- [[TestStore_CollectNotExpire()]] - degree 7, connects to 3 communities
- [[TestNewMemoryQueue()]] - degree 6, connects to 3 communities