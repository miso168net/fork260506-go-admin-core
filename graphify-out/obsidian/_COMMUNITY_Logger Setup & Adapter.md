---
type: community
cohesion: 0.16
members: 18
---

# Logger Setup & Adapter

**Cohesion:** 0.16 - loosely connected
**Members:** 18 nodes

## Members
- [[.Setup()_1]] - code - sdk/config/logger.go
- [[.adapterType()]] - code - sdk/config/logger.go
- [[Logger_2]] - code - sdk/config/logger.go
- [[NewTestLogger()]] - code - logger/factory.go
- [[Option_4]] - code - logger/options.go
- [[Options_4]] - code - logger/options.go
- [[RotationConfig]] - code - sdk/config/logger.go
- [[SetOption()]] - code - logger/options.go
- [[WithAsync()]] - code - logger/options.go
- [[WithCallerSkipCount()]] - code - logger/options.go
- [[WithEnableCaller()]] - code - logger/options.go
- [[WithRotation()]] - code - logger/options.go
- [[WithSampling()]] - code - logger/options.go
- [[WithSanitizer()]] - code - logger/options.go
- [[WithStdout()]] - code - logger/options.go
- [[buildAdapterOptions()]] - code - logger/factory.go
- [[logger.go_1]] - code - sdk/config/logger.go
- [[options.go_7]] - code - logger/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Setup__Adapter
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 3 edges to [[_COMMUNITY_Default Config Tests]]
- 3 edges to [[_COMMUNITY_Logger Examples]]
- 2 edges to [[_COMMUNITY_ReaderSource Options]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 2 edges to [[_COMMUNITY_File Source + GORM Logger]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_Default Logger Initialization]]
- 1 edge to [[_COMMUNITY_Level Functions]]
- 1 edge to [[_COMMUNITY_Logrus Adapter Methods]]

## Top bridge nodes
- [[.Setup()_1]] - degree 14, connects to 7 communities
- [[options.go_7]] - degree 17, connects to 6 communities
- [[buildAdapterOptions()]] - degree 5, connects to 3 communities
- [[NewTestLogger()]] - degree 4, connects to 3 communities