---
type: community
cohesion: 0.27
members: 19
---

# Deprecated/Logger Mixed Tests

**Cohesion:** 0.27 - loosely connected
**Members:** 19 nodes

## Members
- [[.Info()_7]] - code - tools/gorm/gormlog/logger.go
- [[.Sync()_7]] - code - logger/zap.go
- [[BenchmarkMaskingCore_Disabled()]] - code - logger/pii_mask_test.go
- [[BenchmarkMaskingCore_Enabled()]] - code - logger/pii_mask_test.go
- [[Fatalf()]] - code - logger/level.go
- [[New()_2]] - code - tools/gorm/logger/deprecated.go
- [[NewWithSeconds()]] - code - sdk/pkg/cronjob/gadmjob.go
- [[SetMasker()]] - code - logger/pii_mask.go
- [[TestLogger2()]] - code - logger/logger_test.go
- [[TestMaskingCore_DisabledByDefault()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_Enabled()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_NonStringFields()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_WithFields()]] - code - logger/pii_mask_test.go
- [[TestNew()]] - code - tools/gorm/gormlog/logger_test.go
- [[deprecated.go_5]] - code - tools/gorm/logger/deprecated.go
- [[gadmjob.go]] - code - sdk/pkg/cronjob/gadmjob.go
- [[logger_test.go_1]] - code - tools/gorm/gormlog/logger_test.go
- [[newMaskingCore()]] - code - logger/pii_mask.go
- [[pii_mask_test.go]] - code - logger/pii_mask_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Deprecated/Logger_Mixed_Tests
SORT file.name ASC
```

## Connections to other communities
- 22 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 6 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 6 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 5 edges to [[_COMMUNITY_Logger Examples]]
- 5 edges to [[_COMMUNITY_File Source + GORM Logger]]
- 4 edges to [[_COMMUNITY_Config Loader Memory]]
- 4 edges to [[_COMMUNITY_Masking Core (PII Mask)]]
- 3 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 3 edges to [[_COMMUNITY_Default Config Tests]]
- 3 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 3 edges to [[_COMMUNITY_Field Constructors]]
- 3 edges to [[_COMMUNITY_Database Resolver Config]]
- 3 edges to [[_COMMUNITY_antd_api Wrapper]]
- 2 edges to [[_COMMUNITY_Captcha Driver]]
- 2 edges to [[_COMMUNITY_Config Core API]]
- 2 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 2 edges to [[_COMMUNITY_File Writer  Format Tests]]
- 2 edges to [[_COMMUNITY_Level Functions]]
- 2 edges to [[_COMMUNITY_Sampling Logger]]
- 2 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_Config Value Types]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_Source Watcher]]
- 1 edge to [[_COMMUNITY_Hash  Field  Table Utils]]
- 1 edge to [[_COMMUNITY_Logger LogfDebugf]]
- 1 edge to [[_COMMUNITY_Logrus Adapter Methods]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]
- 1 edge to [[_COMMUNITY_JWT Deprecated Aliases]]
- 1 edge to [[_COMMUNITY_Logger Context + Poster Image]]
- 1 edge to [[_COMMUNITY_gRPC Header Helpers]]

## Top bridge nodes
- [[New()_2]] - degree 43, connects to 22 communities
- [[.Info()_7]] - degree 28, connects to 10 communities
- [[Fatalf()]] - degree 19, connects to 7 communities
- [[.Sync()_7]] - degree 17, connects to 7 communities
- [[TestMaskingCore_NonStringFields()]] - degree 10, connects to 3 communities