---
type: community
cohesion: 0.17
members: 20
---

# Logger Examples

**Cohesion:** 0.17 - loosely connected
**Members:** 20 nodes

## Members
- [[AdapterFactory]] - code - logger/factory.go
- [[DefaultConfig()]] - code - logger/config.go
- [[ExampleFromLegacyConfig()]] - code - logger/examples_test.go
- [[ExampleNewDevelopmentLogger()]] - code - logger/examples_test.go
- [[ExampleNewFromConfig()]] - code - logger/examples_test.go
- [[ExampleNewProductionLogger()]] - code - logger/examples_test.go
- [[ExampleRegisterAdapter()]] - code - logger/examples_test.go
- [[FromLegacyConfig()]] - code - logger/config.go
- [[GetAdapter()]] - code - logger/factory.go
- [[ListAdapters()]] - code - logger/factory.go
- [[NewDevelopmentLogger()]] - code - logger/factory.go
- [[NewFromConfig()]] - code - logger/factory.go
- [[NewProductionLogger()]] - code - logger/factory.go
- [[RegisterAdapter()]] - code - logger/factory.go
- [[SetupLogger()]] - code - logger/factory.go
- [[applyPlugins()]] - code - logger/factory.go
- [[examples_test.go]] - code - logger/examples_test.go
- [[factory.go]] - code - logger/factory.go
- [[init()_2]] - code - logger/factory.go
- [[parseLevel()]] - code - logger/factory.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Examples
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 5 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_Logger Config Plugins]]
- 3 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 2 edges to [[_COMMUNITY_Default Logger Initialization]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_Field Constructors]]
- 1 edge to [[_COMMUNITY_Logrus AddHook]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Logrus Adapter Methods]]

## Top bridge nodes
- [[NewFromConfig()]] - degree 17, connects to 7 communities
- [[examples_test.go]] - degree 9, connects to 3 communities
- [[ExampleNewDevelopmentLogger()]] - degree 5, connects to 3 communities
- [[SetupLogger()]] - degree 6, connects to 2 communities
- [[ExampleRegisterAdapter()]] - degree 5, connects to 2 communities