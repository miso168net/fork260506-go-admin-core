---
type: community
cohesion: 0.05
members: 49
---

# Database Resolver Config

**Cohesion:** 0.05 - loosely connected
**Members:** 49 nodes

## Members
- [[.Debug()_4]] - code - logger/sanitizer.go
- [[.Error()_5]] - code - logger/sanitizer.go
- [[.Fields()_5]] - code - logger/sanitizer.go
- [[.Info()_4]] - code - logger/sanitizer.go
- [[.Init()_9]] - code - tools/database/config.go
- [[.Init()_10]] - code - tools/database/config.go
- [[.Init()_5]] - code - logger/sampling.go
- [[.Init()_6]] - code - logger/sanitizer.go
- [[.Log()_5]] - code - logger/sanitizer.go
- [[.Logf()_5]] - code - logger/sanitizer.go
- [[.Options()_6]] - code - logger/sanitizer.go
- [[.String()_20]] - code - logger/sanitizer.go
- [[.Sync()_6]] - code - logger/sanitizer.go
- [[.Warn()_4]] - code - logger/sanitizer.go
- [[.applySanitizer()]] - code - logger/sanitizer.go
- [[.hashString()]] - code - logger/sanitizer.go
- [[.maskString()]] - code - logger/sanitizer.go
- [[.matchRule()]] - code - logger/sanitizer.go
- [[.sanitizeFields()]] - code - logger/sanitizer.go
- [[CheckExist()]] - code - sdk/pkg/utils/file.go
- [[CheckPermission()]] - code - sdk/pkg/utils/file.go
- [[DBConfig]] - code - tools/database/config.go
- [[DBResolverConfig_1]] - code - tools/database/config.go
- [[Fields()]] - code - logger/logger.go
- [[GetExt()]] - code - sdk/pkg/utils/file.go
- [[GetImgType()]] - code - sdk/pkg/utils/file.go
- [[GetSize()]] - code - sdk/pkg/utils/file.go
- [[GetType()]] - code - sdk/pkg/utils/file.go
- [[Init()]] - code - logger/logger.go
- [[IsNotExistMkDir()]] - code - sdk/pkg/utils/file.go
- [[Log()]] - code - logger/logger.go
- [[Logf()]] - code - logger/logger.go
- [[Logger_1]] - code - logger/logger.go
- [[MkDir()]] - code - sdk/pkg/utils/file.go
- [[NewConfigure()]] - code - tools/database/config.go
- [[NewResolverConfigure()]] - code - tools/database/config.go
- [[Open()]] - code - sdk/pkg/utils/file.go
- [[SanitizerConfig]] - code - logger/sanitizer.go
- [[SanitizerRule]] - code - logger/sanitizer.go
- [[String()]] - code - logger/logger.go
- [[TestDBConfig_Init()]] - code - tools/database/config_test.go
- [[TestIsNotExistMkDir()]] - code - sdk/pkg/utils/file_test.go
- [[config.go_3]] - code - tools/database/config.go
- [[config_test.go]] - code - tools/database/config_test.go
- [[file.go_3]] - code - sdk/pkg/utils/file.go
- [[file_test.go_1]] - code - sdk/pkg/utils/file_test.go
- [[logger.go]] - code - logger/logger.go
- [[sanitizer.go]] - code - logger/sanitizer.go
- [[sanitizerLogger]] - code - logger/sanitizer.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Database_Resolver_Config
SORT file.name ASC
```

## Connections to other communities
- 16 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 8 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 3 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 2 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_Memory Queue Operations]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Field Constructors]]
- 1 edge to [[_COMMUNITY_Sampling Logger]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Config Settings & Multi-DB]]
- 1 edge to [[_COMMUNITY_File  Path Utils]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]

## Top bridge nodes
- [[GetImgType()]] - degree 7, connects to 5 communities
- [[.Init()_10]] - degree 11, connects to 3 communities
- [[Open()]] - degree 8, connects to 3 communities
- [[TestDBConfig_Init()]] - degree 5, connects to 3 communities
- [[sanitizerLogger]] - degree 19, connects to 2 communities