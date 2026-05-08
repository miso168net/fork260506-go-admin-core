---
type: community
cohesion: 0.23
members: 13
---

# Source Test Helpers

**Cohesion:** 0.23 - loosely connected
**Members:** 13 nodes

## Members
- [[.Read()_3]] - code - sdk/pkg/ws/ws.go
- [[IncludeUnset()]] - code - config/source/flag/options.go
- [[NewSource()_2]] - code - config/source/memory/memory.go
- [[TestConfig()]] - code - config/source/file/file_test.go
- [[TestFile()]] - code - config/source/file/file_test.go
- [[TestFlagsrc_Read()]] - code - config/source/flag/flag_test.go
- [[TestFlagsrc_ReadAll()]] - code - config/source/flag/flag_test.go
- [[file_test.go]] - code - config/source/file/file_test.go
- [[flag_test.go]] - code - config/source/flag/flag_test.go
- [[includeUnsetKey]] - code - config/source/flag/options.go
- [[initTestFlags()]] - code - config/source/flag/flag_test.go
- [[memory.go_1]] - code - config/source/memory/memory.go
- [[options.go_5]] - code - config/source/flag/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Source_Test_Helpers
SORT file.name ASC
```

## Connections to other communities
- 10 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 7 edges to [[_COMMUNITY_Default Config Tests]]
- 3 edges to [[_COMMUNITY_Config Loader Memory]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 2 edges to [[_COMMUNITY_Errors & File Watcher]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_Database Resolver Config]]
- 2 edges to [[_COMMUNITY_File  Path Utils]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Hash  Field  Table Utils]]

## Top bridge nodes
- [[.Read()_3]] - degree 13, connects to 7 communities
- [[TestConfig()]] - degree 9, connects to 5 communities
- [[NewSource()_2]] - degree 12, connects to 4 communities
- [[TestFile()]] - degree 9, connects to 3 communities
- [[TestFlagsrc_ReadAll()]] - degree 7, connects to 2 communities