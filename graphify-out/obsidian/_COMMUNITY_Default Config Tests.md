---
type: community
cohesion: 0.26
members: 14
---

# Default Config Tests

**Cohesion:** 0.26 - loosely connected
**Members:** 14 nodes

## Members
- [[GetDirFiles()]] - code - sdk/pkg/utils/utils.go
- [[Name()_1]] - code - observe/audit/options.go
- [[NewConfig()_1]] - code - sdk/runtime/application.go
- [[TestConfigLoadWithGoodFile()]] - code - config/default_test.go
- [[TestConfigLoadWithInvalidFile()]] - code - config/default_test.go
- [[TestConfigMerge()]] - code - config/default_test.go
- [[TestConfigWatcherDirtyOverrite()]] - code - config/default_test.go
- [[WithPath()]] - code - logger/writer/options.go
- [[createFileForIssue18()]] - code - config/default_test.go
- [[createFileForTest()]] - code - config/default_test.go
- [[default_test.go]] - code - config/default_test.go
- [[equalS()]] - code - config/default_test.go
- [[filePathKey]] - code - config/source/file/options.go
- [[options.go_4]] - code - config/source/file/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Default_Config_Tests
SORT file.name ASC
```

## Connections to other communities
- 11 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 7 edges to [[_COMMUNITY_Source Test Helpers]]
- 4 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 4 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 3 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 3 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 2 edges to [[_COMMUNITY_Config Top-Level]]
- 2 edges to [[_COMMUNITY_Audit OptionsReader]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Memory Source Options]]
- 1 edge to [[_COMMUNITY_Writer Options]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]
- 1 edge to [[_COMMUNITY_Config Settings & Multi-DB]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_SDK Runtime Routers]]

## Top bridge nodes
- [[WithPath()]] - degree 14, connects to 5 communities
- [[TestConfigMerge()]] - degree 11, connects to 5 communities
- [[TestConfigLoadWithInvalidFile()]] - degree 10, connects to 5 communities
- [[NewConfig()_1]] - degree 9, connects to 5 communities
- [[TestConfigWatcherDirtyOverrite()]] - degree 8, connects to 5 communities