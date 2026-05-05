---
type: community
cohesion: 0.04
members: 81
---

# Config Reader & Observe

**Cohesion:** 0.04 - loosely connected
**Members:** 81 nodes

## Members
- [[.Read()_3]] - code - sdk/pkg/ws/ws.go
- [[.Write()_4]] - code - sdk/pkg/ws/ws.go
- [[.checkFile()]] - code - logger/writer/file.go
- [[.getFilename()]] - code - logger/writer/file.go
- [[.write()]] - code - logger/writer/file.go
- [[Count()]] - code - observability/audit/deprecated.go
- [[Count()_1]] - code - observe/audit/options.go
- [[Entity]] - code - config/config.go
- [[FileWriter]] - code - logger/writer/file.go
- [[Format()]] - code - observability/audit/deprecated.go
- [[Format()_1]] - code - observe/audit/options.go
- [[FormatFunc]] - code - observe/audit/log.go
- [[Get()]] - code - config/config.go
- [[GetFileSize()]] - code - sdk/pkg/file.go
- [[IncludeUnset()]] - code - config/source/flag/options.go
- [[JSONFormat()]] - code - observability/audit/deprecated.go
- [[JSONFormat()_1]] - code - observe/audit/log.go
- [[Load()]] - code - config/config.go
- [[LoadFile()]] - code - config/config.go
- [[Name()]] - code - observability/audit/deprecated.go
- [[Name()_1]] - code - observe/audit/options.go
- [[NewConfig()_1]] - code - sdk/runtime/application.go
- [[NewConfig()]] - code - config/config.go
- [[NewFileWriter()]] - code - logger/writer/file.go
- [[NewSource()_2]] - code - config/source/memory/memory.go
- [[Option_6]] - code - observe/audit/options.go
- [[Option]] - code - config/config.go
- [[Option_5]] - code - logger/writer/options.go
- [[Options_6]] - code - observe/audit/options.go
- [[Options]] - code - config/config.go
- [[Options_5]] - code - logger/writer/options.go
- [[ReadOption]] - code - observe/audit/options.go
- [[ReadOptions]] - code - observe/audit/options.go
- [[Record]] - code - observe/audit/log.go
- [[Since()]] - code - observability/audit/deprecated.go
- [[Since()_1]] - code - observe/audit/options.go
- [[Size()]] - code - observability/audit/deprecated.go
- [[Size()_1]] - code - observe/audit/options.go
- [[Stream]] - code - observe/audit/log.go
- [[Sync()]] - code - config/config.go
- [[TestConfig()]] - code - config/source/file/file_test.go
- [[TestConfigLoadWithGoodFile()]] - code - config/default_test.go
- [[TestConfigLoadWithInvalidFile()]] - code - config/default_test.go
- [[TestConfigMerge()]] - code - config/default_test.go
- [[TestConfigWatcherDirtyOverrite()]] - code - config/default_test.go
- [[TestFile()]] - code - config/source/file/file_test.go
- [[TestFlagsrc_Read()]] - code - config/source/flag/flag_test.go
- [[TestFlagsrc_ReadAll()]] - code - config/source/flag/flag_test.go
- [[TestFormat()]] - code - config/source/file/format_test.go
- [[TextFormat()]] - code - observability/audit/deprecated.go
- [[TextFormat()_1]] - code - observe/audit/log.go
- [[Watch()]] - code - config/config.go
- [[WithCap()]] - code - logger/writer/options.go
- [[WithChangeSet()]] - code - config/source/memory/options.go
- [[WithJSON()]] - code - config/source/memory/options.go
- [[WithPath()]] - code - logger/writer/options.go
- [[WithSuffix()]] - code - logger/writer/options.go
- [[WithYAML()]] - code - config/source/memory/options.go
- [[changeSetKey]] - code - config/source/memory/options.go
- [[config.go]] - code - config/config.go
- [[createFileForIssue18()]] - code - config/default_test.go
- [[createFileForTest()]] - code - config/default_test.go
- [[default_test.go]] - code - config/default_test.go
- [[deprecated.go]] - code - observability/audit/deprecated.go
- [[equalS()]] - code - config/default_test.go
- [[file.go_1]] - code - logger/writer/file.go
- [[filePathKey]] - code - config/source/file/options.go
- [[file_test.go]] - code - config/source/file/file_test.go
- [[flag_test.go]] - code - config/source/flag/flag_test.go
- [[format_test.go]] - code - config/source/file/format_test.go
- [[includeUnsetKey]] - code - config/source/flag/options.go
- [[initTestFlags()]] - code - config/source/flag/flag_test.go
- [[log.go_1]] - code - observe/audit/log.go
- [[memory.go_1]] - code - config/source/memory/memory.go
- [[options.go_4]] - code - config/source/file/options.go
- [[options.go_5]] - code - config/source/flag/options.go
- [[options.go_6]] - code - config/source/memory/options.go
- [[options.go_8]] - code - logger/writer/options.go
- [[options.go_9]] - code - observe/audit/options.go
- [[setDefault()]] - code - logger/writer/options.go
- [[withData()]] - code - config/source/memory/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Reader_&_Observe
SORT file.name ASC
```

## Connections to other communities
- 30 edges to [[_COMMUNITY_Logger Performance Tests]]
- 13 edges to [[_COMMUNITY_Config Core API]]
- 10 edges to [[_COMMUNITY_Captcha & Preprocessor Tools]]
- 9 edges to [[_COMMUNITY_Log Formatter & Color]]
- 8 edges to [[_COMMUNITY_Storage & Response Models]]
- 5 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 5 edges to [[_COMMUNITY_File Utils & WebSocket]]
- 3 edges to [[_COMMUNITY_Errors & File Watcher]]
- 3 edges to [[_COMMUNITY_Configure & Settings]]
- 2 edges to [[_COMMUNITY_SDK Binding & Pagination]]
- 2 edges to [[_COMMUNITY_Hash & Field Values]]
- 1 edge to [[_COMMUNITY_SDK Application Container]]

## Top bridge nodes
- [[.Read()_3]] - degree 13, connects to 7 communities
- [[.Write()_4]] - degree 13, connects to 6 communities
- [[Format()_1]] - degree 12, connects to 5 communities
- [[TestConfigMerge()]] - degree 11, connects to 4 communities
- [[TestConfigLoadWithInvalidFile()]] - degree 10, connects to 3 communities