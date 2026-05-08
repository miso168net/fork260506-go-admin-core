---
type: community
cohesion: 0.07
members: 42
---

# JSON Reader & Preprocessor

**Cohesion:** 0.07 - loosely connected
**Members:** 42 nodes

## Members
- [[.Bytes()_2]] - code - config/reader/json/values.go
- [[.Duration()_1]] - code - config/reader/json/values.go
- [[.Get()_3]] - code - config/reader/json/values.go
- [[.Int()_1]] - code - config/reader/json/values.go
- [[.MarshalJSON()]] - code - sdk/pkg/utils/json_time.go
- [[.Run()_1]] - code - storage/queue/memory.go
- [[.Scan()_3]] - code - config/reader/json/values.go
- [[.Scan()_2]] - code - config/reader/json/values.go
- [[.Scan()_4]] - code - sdk/pkg/utils/json_time.go
- [[.Set()_2]] - code - config/reader/json/values.go
- [[.String()_9]] - code - config/reader/json/values.go
- [[.String()_8]] - code - config/reader/json/values.go
- [[.StringSlice()_1]] - code - config/reader/json/values.go
- [[DriverDigitFunc()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[DriverStringFunc()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[Fatal()]] - code - logger/level.go
- [[JSONTime]] - code - sdk/pkg/utils/json_time.go
- [[ReplaceEnvVars()]] - code - config/reader/preprocessor.go
- [[Scan()]] - code - config/config.go
- [[SetStore()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[TestBackwardCompatibility()]] - code - integration_test.go
- [[TestCaptchaCompatibility()]] - code - integration_test.go
- [[TestCasbinCompatibility()]] - code - integration_test.go
- [[TestGormLogCompatibility()]] - code - integration_test.go
- [[TestImportPaths()]] - code - integration_test.go
- [[TestJWTAuthCompatibility()]] - code - integration_test.go
- [[TestObserveAuditCompatibility()]] - code - integration_test.go
- [[TestReplaceEnvVars()]] - code - config/reader/preprocessor_test.go
- [[TestResponseCompatibility()]] - code - integration_test.go
- [[TestStructArray()]] - code - config/reader/json/values_test.go
- [[TestValues()]] - code - config/reader/json/values_test.go
- [[Verify()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[deprecated.go_1]] - code - sdk/pkg/captcha/deprecated.go
- [[integration_test.go]] - code - integration_test.go
- [[jsonValue]] - code - config/reader/json/values.go
- [[jsonValues]] - code - config/reader/json/values.go
- [[json_time.go]] - code - sdk/pkg/utils/json_time.go
- [[newValues()]] - code - config/reader/json/values.go
- [[preprocessor.go]] - code - config/reader/preprocessor.go
- [[preprocessor_test.go]] - code - config/reader/preprocessor_test.go
- [[values.go]] - code - config/reader/json/values.go
- [[values_test.go]] - code - config/reader/json/values_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/JSON_Reader__Preprocessor
SORT file.name ASC
```

## Connections to other communities
- 17 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 7 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 6 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 3 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_Config Core API]]
- 2 edges to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 2 edges to [[_COMMUNITY_TOML Encoder]]
- 2 edges to [[_COMMUNITY_Memory Queue Operations]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_Captcha Driver]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_Default Config Tests]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_Field Constructors]]
- 1 edge to [[_COMMUNITY_Hash  Field  Table Utils]]
- 1 edge to [[_COMMUNITY_Source Test Helpers]]
- 1 edge to [[_COMMUNITY_Level Functions]]
- 1 edge to [[_COMMUNITY_Logrus Adapter Methods]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_Config Settings & Multi-DB]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]

## Top bridge nodes
- [[Fatal()]] - degree 16, connects to 8 communities
- [[.Run()_1]] - degree 20, connects to 6 communities
- [[jsonValue]] - degree 10, connects to 4 communities
- [[TestCaptchaCompatibility()]] - degree 10, connects to 2 communities
- [[jsonValues]] - degree 8, connects to 2 communities