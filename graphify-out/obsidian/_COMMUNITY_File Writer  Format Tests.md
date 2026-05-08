---
type: community
cohesion: 0.36
members: 9
---

# File Writer / Format Tests

**Cohesion:** 0.36 - loosely connected
**Members:** 9 nodes

## Members
- [[.checkFile()]] - code - logger/writer/file.go
- [[.getFilename()]] - code - logger/writer/file.go
- [[.write()]] - code - logger/writer/file.go
- [[FileWriter]] - code - logger/writer/file.go
- [[Format()_1]] - code - observe/audit/options.go
- [[NewFileWriter()]] - code - logger/writer/file.go
- [[TestFormat()]] - code - config/source/file/format_test.go
- [[file.go_1]] - code - logger/writer/file.go
- [[format_test.go]] - code - config/source/file/format_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/File_Writer_/_Format_Tests
SORT file.name ASC
```

## Connections to other communities
- 3 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 3 edges to [[_COMMUNITY_Audit OptionsReader]]
- 2 edges to [[_COMMUNITY_Errors & File Watcher]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_Default Logger Initialization]]
- 1 edge to [[_COMMUNITY_Writer Options]]
- 1 edge to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 1 edge to [[_COMMUNITY_Default Config Tests]]
- 1 edge to [[_COMMUNITY_Audit FormatFunc & Stream]]
- 1 edge to [[_COMMUNITY_Hash  Field  Table Utils]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]

## Top bridge nodes
- [[Format()_1]] - degree 12, connects to 7 communities
- [[.write()]] - degree 7, connects to 4 communities
- [[.checkFile()]] - degree 7, connects to 3 communities
- [[TestFormat()]] - degree 5, connects to 3 communities
- [[NewFileWriter()]] - degree 4, connects to 1 community