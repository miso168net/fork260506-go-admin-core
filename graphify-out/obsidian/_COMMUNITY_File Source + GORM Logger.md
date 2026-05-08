---
type: community
cohesion: 0.16
members: 17
---

# File Source + GORM Logger

**Cohesion:** 0.16 - loosely connected
**Members:** 17 nodes

## Members
- [[.LogMode()]] - code - tools/gorm/gormlog/logger.go
- [[.New()]] - code - tools/gorm/gormlog/logger.go
- [[.Trace()_1]] - code - tools/gorm/gormlog/logger.go
- [[.Trace()_2]] - code - tools/gorm/gormlog/logger.go
- [[.Value()]] - code - sdk/pkg/utils/json_time.go
- [[.Warn()_6]] - code - tools/gorm/gormlog/logger.go
- [[.getLogger()]] - code - tools/gorm/gormlog/logger.go
- [[New()_4]] - code - tools/gorm/gormlog/logger.go
- [[NewSource()]] - code - config/source/file/file.go
- [[TestLogger()]] - code - logger/logger_test.go
- [[WithName()]] - code - logger/options.go
- [[file.go]] - code - config/source/file/file.go
- [[fileWithLineNum()]] - code - tools/gorm/gormlog/logger.go
- [[gormLogger]] - code - tools/gorm/gormlog/logger.go
- [[logger.go_2]] - code - tools/gorm/gormlog/logger.go
- [[logger_test.go]] - code - logger/logger_test.go
- [[traceRecorder]] - code - tools/gorm/gormlog/logger.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/File_Source__GORM_Logger
SORT file.name ASC
```

## Connections to other communities
- 10 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 5 edges to [[_COMMUNITY_antd_api Wrapper]]
- 5 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 2 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 1 edge to [[_COMMUNITY_Logger LogfDebugf]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 1 edge to [[_COMMUNITY_Source Test Helpers]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Logger Context + Poster Image]]
- 1 edge to [[_COMMUNITY_Default Logger Initialization]]
- 1 edge to [[_COMMUNITY_Logger Examples]]
- 1 edge to [[_COMMUNITY_Sampling Logger]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_Audit OptionsReader]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]

## Top bridge nodes
- [[.Warn()_6]] - degree 14, connects to 8 communities
- [[.Value()]] - degree 9, connects to 6 communities
- [[TestLogger()]] - degree 10, connects to 5 communities
- [[.getLogger()]] - degree 10, connects to 4 communities
- [[gormLogger]] - degree 7, connects to 2 communities