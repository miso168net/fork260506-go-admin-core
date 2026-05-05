---
type: community
cohesion: 0.04
members: 87
---

# Captcha & Preprocessor Tools

**Cohesion:** 0.04 - loosely connected
**Members:** 87 nodes

## Members
- [[.Check()]] - code - logger/pii_mask.go
- [[.Fire()_4]] - code - logger/pii_mask_logrus.go
- [[.Info()_7]] - code - tools/gorm/gormlog/logger.go
- [[.Levels()_4]] - code - logger/pii_mask_logrus.go
- [[.New()]] - code - tools/gorm/gormlog/logger.go
- [[.Next()_2]] - code - config/source/noop.go
- [[.Run()_1]] - code - storage/queue/memory.go
- [[.Scan()_4]] - code - sdk/pkg/utils/json_time.go
- [[.Stop()_2]] - code - config/source/noop.go
- [[.Sync()_4]] - code - logger/pii_mask.go
- [[.Sync()_7]] - code - logger/zap.go
- [[.Trace()_2]] - code - tools/gorm/gormlog/logger.go
- [[.Watch()_3]] - code - config/source/flag/flag.go
- [[.With()_2]] - code - logger/pii_mask.go
- [[.Write()_3]] - code - logger/pii_mask.go
- [[BenchmarkMaskingCore_Disabled()]] - code - logger/pii_mask_test.go
- [[BenchmarkMaskingCore_Enabled()]] - code - logger/pii_mask_test.go
- [[DriverDigitFunc()]] - code - captcha/captcha.go
- [[DriverDigitFunc()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[DriverStringFunc()]] - code - captcha/captcha.go
- [[DriverStringFunc()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[ExtractClaims()_2]] - code - sdk/pkg/jwtauth/deprecated.go
- [[ExtractClaimsFromToken()_1]] - code - sdk/pkg/jwtauth/deprecated.go
- [[Fatal()]] - code - logger/level.go
- [[Fatalf()]] - code - logger/level.go
- [[GetHeaderFirst()]] - code - tools/utils/grpc_header.go
- [[GetMasker()]] - code - logger/pii_mask.go
- [[GetRequestID()]] - code - tools/utils/grpc_header.go
- [[GetToken()_1]] - code - sdk/pkg/jwtauth/deprecated.go
- [[GetUsername()]] - code - tools/utils/grpc_header.go
- [[Masker]] - code - logger/pii_mask.go
- [[New()_2]] - code - tools/gorm/logger/deprecated.go
- [[NewNoopWatcher()]] - code - config/source/noop.go
- [[NewRequestID()]] - code - tools/utils/grpc_header.go
- [[NewWithSeconds()]] - code - sdk/pkg/cronjob/gadmjob.go
- [[ReplaceEnvVars()]] - code - config/reader/preprocessor.go
- [[Scan()]] - code - config/config.go
- [[SetMasker()]] - code - logger/pii_mask.go
- [[SetStore()]] - code - captcha/captcha.go
- [[SetStore()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[TestBackwardCompatibility()]] - code - integration_test.go
- [[TestCaptchaCompatibility()]] - code - integration_test.go
- [[TestCasbinCompatibility()]] - code - integration_test.go
- [[TestGormLogCompatibility()]] - code - integration_test.go
- [[TestImportPaths()]] - code - integration_test.go
- [[TestJWTAuthCompatibility()]] - code - integration_test.go
- [[TestLogger()]] - code - logger/logger_test.go
- [[TestLogger2()]] - code - logger/logger_test.go
- [[TestMaskingCore_DisabledByDefault()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_Enabled()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_NonStringFields()]] - code - logger/pii_mask_test.go
- [[TestMaskingCore_WithFields()]] - code - logger/pii_mask_test.go
- [[TestNew()]] - code - tools/gorm/gormlog/logger_test.go
- [[TestObserveAuditCompatibility()]] - code - integration_test.go
- [[TestReplaceEnvVars()]] - code - config/reader/preprocessor_test.go
- [[TestResponseCompatibility()]] - code - integration_test.go
- [[TestStructArray()]] - code - config/reader/json/values_test.go
- [[TestValues()]] - code - config/reader/json/values_test.go
- [[Verify()]] - code - captcha/captcha.go
- [[Verify()_1]] - code - sdk/pkg/captcha/deprecated.go
- [[WithName()]] - code - logger/options.go
- [[captcha.go]] - code - captcha/captcha.go
- [[configJsonBody]] - code - captcha/captcha.go
- [[deprecated.go_1]] - code - sdk/pkg/captcha/deprecated.go
- [[deprecated.go_3]] - code - sdk/pkg/jwtauth/deprecated.go
- [[deprecated.go_5]] - code - tools/gorm/logger/deprecated.go
- [[gadmjob.go]] - code - sdk/pkg/cronjob/gadmjob.go
- [[grpc_header.go]] - code - tools/utils/grpc_header.go
- [[integration_test.go]] - code - integration_test.go
- [[logger_test.go]] - code - logger/logger_test.go
- [[logger_test.go_1]] - code - tools/gorm/gormlog/logger_test.go
- [[maskFields()]] - code - logger/pii_mask.go
- [[maskingCore]] - code - logger/pii_mask.go
- [[newMaskingCore()]] - code - logger/pii_mask.go
- [[newValues()]] - code - config/reader/json/values.go
- [[noop.go]] - code - config/source/noop.go
- [[noopWatcher]] - code - config/source/noop.go
- [[piiMaskHook]] - code - logger/pii_mask_logrus.go
- [[pii_mask.go]] - code - logger/pii_mask.go
- [[pii_mask_logrus.go]] - code - logger/pii_mask_logrus.go
- [[pii_mask_test.go]] - code - logger/pii_mask_test.go
- [[preprocessor.go]] - code - config/reader/preprocessor.go
- [[preprocessor_test.go]] - code - config/reader/preprocessor_test.go
- [[traceRecorder]] - code - tools/gorm/gormlog/logger.go
- [[transInit()]] - code - sdk/api/translate.go
- [[translate.go]] - code - sdk/api/translate.go
- [[values_test.go]] - code - config/reader/json/values_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Captcha_&_Preprocessor_Tools
SORT file.name ASC
```

## Connections to other communities
- 46 edges to [[_COMMUNITY_Logger Performance Tests]]
- 19 edges to [[_COMMUNITY_Config Core API]]
- 14 edges to [[_COMMUNITY_Storage & Response Models]]
- 13 edges to [[_COMMUNITY_Sampling & Extended Logger]]
- 10 edges to [[_COMMUNITY_Config Reader & Observe]]
- 9 edges to [[_COMMUNITY_Hash & Field Values]]
- 7 edges to [[_COMMUNITY_Log Formatter & Color]]
- 7 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 7 edges to [[_COMMUNITY_SDK Binding & Pagination]]
- 6 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 4 edges to [[_COMMUNITY_API Context & Response]]
- 3 edges to [[_COMMUNITY_Configure & Settings]]
- 1 edge to [[_COMMUNITY_Image & Context Tools]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]

## Top bridge nodes
- [[New()_2]] - degree 43, connects to 11 communities
- [[.Info()_7]] - degree 28, connects to 7 communities
- [[Fatal()]] - degree 16, connects to 7 communities
- [[.Run()_1]] - degree 20, connects to 5 communities
- [[TestLogger()]] - degree 10, connects to 5 communities