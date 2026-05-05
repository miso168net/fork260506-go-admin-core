---
type: community
cohesion: 0.04
members: 88
---

# Storage & Response Models

**Cohesion:** 0.04 - loosely connected
**Members:** 88 nodes

## Members
- [[.AddError()_2]] - code - sdk/service/service.go
- [[.Clone()_1]] - code - response/antd/model.go
- [[.Connect()]] - code - sdk/runtime/cache.go
- [[.Decrease()_1]] - code - storage/cache/memory.go
- [[.Decrease()]] - code - sdk/runtime/cache.go
- [[.Del()_3]] - code - storage/cache/memory.go
- [[.Del()]] - code - config/default.go
- [[.Del()_1]] - code - config/reader/json/values.go
- [[.Del()_2]] - code - sdk/runtime/cache.go
- [[.Empty()]] - code - sdk/config/queue.go
- [[.Expire()_1]] - code - storage/cache/memory.go
- [[.Expire()]] - code - sdk/runtime/cache.go
- [[.Get()_5]] - code - storage/cache/memory.go
- [[.Get()]] - code - captcha/store.go
- [[.Get()_4]] - code - sdk/runtime/cache.go
- [[.HashDel()_1]] - code - storage/cache/memory.go
- [[.HashDel()]] - code - sdk/runtime/cache.go
- [[.HashGet()_1]] - code - storage/cache/memory.go
- [[.HashGet()]] - code - sdk/runtime/cache.go
- [[.Increase()_1]] - code - storage/cache/memory.go
- [[.Increase()]] - code - sdk/runtime/cache.go
- [[.PutToken()]] - code - sdk/runtime/cache.go
- [[.Set()_4]] - code - storage/cache/memory.go
- [[.Set()]] - code - captcha/store.go
- [[.Set()_3]] - code - sdk/runtime/cache.go
- [[.SetCode()_1]] - code - response/antd/model.go
- [[.SetData()_1]] - code - response/antd/model.go
- [[.SetMsg()_1]] - code - response/antd/model.go
- [[.SetPrefix()]] - code - sdk/runtime/cache.go
- [[.SetSuccess()_1]] - code - response/antd/model.go
- [[.SetTraceID()_1]] - code - response/antd/model.go
- [[.Setup()]] - code - sdk/config/cache.go
- [[.Setup()_2]] - code - sdk/config/queue.go
- [[.String()_26]] - code - storage/cache/memory.go
- [[.String()_23]] - code - sdk/runtime/cache.go
- [[.Token()]] - code - sdk/runtime/cache.go
- [[.Verify()]] - code - captcha/store.go
- [[.calculate()]] - code - storage/cache/memory.go
- [[.connect()]] - code - storage/cache/memory.go
- [[.getItem()]] - code - storage/cache/memory.go
- [[.setItem()]] - code - storage/cache/memory.go
- [[BenchmarkSetCollect()]] - code - captcha/store_test.go
- [[Cache]] - code - sdk/config/cache.go
- [[Cache_1]] - code - sdk/runtime/cache.go
- [[Custum()]] - code - response/antd/return.go
- [[Error()_1]] - code - response/antd/return.go
- [[Errorf()]] - code - logger/level.go
- [[GenerateMsgIDFromContext()]] - code - sdk/pkg/utils.go
- [[GetLocalHost()]] - code - sdk/pkg/ip.go
- [[GetLocation()]] - code - sdk/pkg/ip.go
- [[ListData]] - code - response/antd/model.go
- [[ListOK()]] - code - response/antd/return.go
- [[Memory]] - code - storage/cache/memory.go
- [[NewCacheStore()]] - code - captcha/store.go
- [[NewMemory()]] - code - storage/queue/memory.go
- [[OK()]] - code - response/antd/return.go
- [[PageOK()]] - code - response/antd/return.go
- [[Pages]] - code - response/antd/model.go
- [[Queue]] - code - sdk/config/queue.go
- [[QueueMemory]] - code - sdk/config/queue.go
- [[Response_1]] - code - response/antd/model.go
- [[Service]] - code - sdk/service/service.go
- [[TestGetClear()]] - code - captcha/store_test.go
- [[TestMemory_Append()]] - code - storage/queue/memory_test.go
- [[TestMemory_Get()]] - code - storage/cache/memory_test.go
- [[TestNewCacheStore()]] - code - captcha/store_test.go
- [[TestNewMemoryQueue()]] - code - sdk/runtime/queue_test.go
- [[TestQueue_Register()]] - code - sdk/runtime/queue_test.go
- [[TestSetGet()]] - code - captcha/store_test.go
- [[TestStore_CollectNotExpire()]] - code - captcha/store_test.go
- [[TestStore_SetGoCollect()]] - code - captcha/store_test.go
- [[UpFileOK()]] - code - response/antd/return.go
- [[cache.go]] - code - sdk/config/cache.go
- [[cacheStore]] - code - captcha/store.go
- [[getStore()]] - code - captcha/store_test.go
- [[ip.go]] - code - sdk/pkg/ip.go
- [[item]] - code - storage/cache/memory.go
- [[lists]] - code - response/antd/model.go
- [[memory.go_2]] - code - storage/cache/memory.go
- [[memory_test.go]] - code - storage/cache/memory_test.go
- [[model.go_1]] - code - response/antd/model.go
- [[queue.go]] - code - sdk/config/queue.go
- [[queue_test.go]] - code - sdk/runtime/queue_test.go
- [[return.go_1]] - code - response/antd/return.go
- [[return.go]] - code - response/return.go
- [[service.go]] - code - sdk/service/service.go
- [[store.go]] - code - captcha/store.go
- [[store_test.go]] - code - captcha/store_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Storage_&_Response_Models
SORT file.name ASC
```

## Connections to other communities
- 21 edges to [[_COMMUNITY_Logger Performance Tests]]
- 14 edges to [[_COMMUNITY_Captcha & Preprocessor Tools]]
- 9 edges to [[_COMMUNITY_Config Core API]]
- 9 edges to [[_COMMUNITY_API Context & Response]]
- 8 edges to [[_COMMUNITY_Config Reader & Observe]]
- 8 edges to [[_COMMUNITY_Errors & File Watcher]]
- 5 edges to [[_COMMUNITY_SDK Binding & Pagination]]
- 4 edges to [[_COMMUNITY_Log Formatter & Color]]
- 4 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 3 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 3 edges to [[_COMMUNITY_HTTP Server Options]]
- 3 edges to [[_COMMUNITY_SDK Application Container]]
- 2 edges to [[_COMMUNITY_Hash & Field Values]]
- 2 edges to [[_COMMUNITY_Configure & Settings]]
- 1 edge to [[_COMMUNITY_File Utils & WebSocket]]

## Top bridge nodes
- [[Errorf()]] - degree 44, connects to 9 communities
- [[.Get()_5]] - degree 27, connects to 7 communities
- [[.Set()_4]] - degree 26, connects to 7 communities
- [[NewMemory()]] - degree 13, connects to 4 communities
- [[GenerateMsgIDFromContext()]] - degree 11, connects to 3 communities