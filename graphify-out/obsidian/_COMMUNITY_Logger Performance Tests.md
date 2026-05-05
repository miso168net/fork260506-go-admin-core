---
type: community
cohesion: 0.08
members: 128
---

# Logger Performance Tests

**Cohesion:** 0.08 - loosely connected
**Members:** 128 nodes

## Members
- [[.Close()_3]] - code - logger/zap.go
- [[.Debug()_1]] - code - logger/helper.go
- [[.Debugf()]] - code - logger/helper.go
- [[.Debugw()]] - code - logger/helper.go
- [[.EnableLog()]] - code - casbin/log.go
- [[.Enabled()]] - code - logger/level.go
- [[.Error()_10]] - code - tools/gorm/gormlog/logger.go
- [[.Error()_2]] - code - logger/helper.go
- [[.Errorf()]] - code - logger/helper.go
- [[.Errorw()]] - code - logger/helper.go
- [[.Fatal()]] - code - logger/helper.go
- [[.Fatalf()]] - code - logger/helper.go
- [[.Fields()_6]] - code - logger/zap.go
- [[.Float64()_1]] - code - config/reader/json/values.go
- [[.Info()_1]] - code - logger/helper.go
- [[.Infof()]] - code - logger/helper.go
- [[.Infow()]] - code - logger/helper.go
- [[.IsEnabled()]] - code - casbin/log.go
- [[.LogEnforce()]] - code - casbin/log.go
- [[.LogMode()]] - code - tools/gorm/gormlog/logger.go
- [[.LogModel()]] - code - casbin/log.go
- [[.LogPolicy()]] - code - casbin/log.go
- [[.LogRole()]] - code - casbin/log.go
- [[.Logf()_6]] - code - logger/zap.go
- [[.Options()_8]] - code - server/listener/server.go
- [[.Reset()]] - code - errors/errors.pb.go
- [[.String()_27]] - code - storage/queue/memory.go
- [[.Trace()_1]] - code - tools/gorm/gormlog/logger.go
- [[.Trace()]] - code - logger/helper.go
- [[.Tracef()]] - code - logger/helper.go
- [[.Warn()_6]] - code - tools/gorm/gormlog/logger.go
- [[.Warn()_1]] - code - logger/helper.go
- [[.Warnf()]] - code - logger/helper.go
- [[.Warnw()]] - code - logger/helper.go
- [[.getLogger()]] - code - tools/gorm/gormlog/logger.go
- [[.kvToMap()]] - code - logger/helper.go
- [[BenchmarkAsync()]] - code - logger/advanced_features_test.go
- [[BenchmarkAsyncLogger()]] - code - logger/async_test.go
- [[BenchmarkAsyncLogger_vs_Sync()]] - code - logger/async_test.go
- [[BenchmarkAsync_Baseline()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkAsync_HighContention()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkAsync_LargeBuffer()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkAsync_SmallBuffer()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkAsync_WithFields()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkCombined_AsyncSamplingSanitizer()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkCombined_Production()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkDefaultLogger()]] - code - logger/benchmark_test.go
- [[BenchmarkFormatter_Console()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkFormatter_JSON()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkLogrus_Caller()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkLogrus_Logf()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkLogrus_Simple()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkLogrus_WithFields()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSampling()]] - code - logger/advanced_features_test.go
- [[BenchmarkSamplingLogger()]] - code - logger/benchmark_test.go
- [[BenchmarkSampling_First100Then10()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSampling_First10Then1()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSampling_WithFields()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSanitizer()]] - code - logger/advanced_features_test.go
- [[BenchmarkSanitizerLogger()]] - code - logger/sanitizer_test.go
- [[BenchmarkSanitizerLogger_vs_NoSanitize()]] - code - logger/sanitizer_test.go
- [[BenchmarkSanitizer_MultipleSensitive()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSanitizer_NoSensitiveFields()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkSanitizer_WithPassword()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkStress_DeepNesting()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkStress_HighVolume()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkStress_LargeFields()]] - code - logger/performance_benchmark_test.go
- [[BenchmarkZapLogger()]] - code - logger/benchmark_test.go
- [[Get()_2]] - code - sdk/pkg/http.go
- [[Helper]] - code - logger/helper.go
- [[Log]] - code - observe/audit/log.go
- [[Logger]] - code - casbin/log.go
- [[New()_4]] - code - tools/gorm/gormlog/logger.go
- [[NewAsyncLogger()]] - code - logger/async.go
- [[NewLogrusLogger()]] - code - logger/logrus.go
- [[NewSamplingLogger()]] - code - logger/sampling.go
- [[NewSanitizerLogger()]] - code - logger/sanitizer.go
- [[Post()]] - code - sdk/pkg/http.go
- [[SetupLogger()_1]] - code - sdk/pkg/logger/log.go
- [[TestAsyncLogger_Basic()]] - code - logger/async_test.go
- [[TestAsyncLogger_BlockPolicy()]] - code - logger/async_test.go
- [[TestAsyncLogger_BufferFull()]] - code - logger/async_test.go
- [[TestAsyncLogger_ErrorLevel()]] - code - logger/async_test.go
- [[TestAsyncLogger_Fields()]] - code - logger/async_test.go
- [[TestAsyncLogger_GetStats()]] - code - logger/async_test.go
- [[TestAsyncLogger_GracefulShutdown()]] - code - logger/async_test.go
- [[TestAsyncLogger_HighConcurrency()]] - code - logger/async_test.go
- [[TestAsyncLogger_SamplePolicy()]] - code - logger/async_test.go
- [[TestAsyncLogger_Sync()]] - code - logger/async_test.go
- [[TestAsyncPerformance()]] - code - logger/advanced_features_test.go
- [[TestCallerStackDebug()]] - code - logger/caller_debug_test.go
- [[TestCallerStackInLog()]] - code - logger/caller_debug_test.go
- [[TestCombinedFeatures()]] - code - logger/advanced_features_test.go
- [[TestLogrusCallerInfo()]] - code - logger/caller_test.go
- [[TestLogrusCallerWithHelper()]] - code - logger/caller_test.go
- [[TestLogrusCallerWithLogf()]] - code - logger/caller_test.go
- [[TestSampling()]] - code - logger/advanced_features_test.go
- [[TestSanitizer()]] - code - logger/advanced_features_test.go
- [[TestSanitizerLogger_Basic()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_CaseInsensitive()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_CustomMatcher()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_CustomRule()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_EmailMask()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_FieldsChaining()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_IDCardMask()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_MultipleFields()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_NoSanitization()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_NonStringValue()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_PasswordRemove()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_PhoneMask()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_SuffixMatch()]] - code - logger/sanitizer_test.go
- [[TestSanitizerLogger_TokenHash()]] - code - logger/sanitizer_test.go
- [[WithLevel()]] - code - logger/options.go
- [[WithOutput()]] - code - logger/options.go
- [[advanced_features_test.go]] - code - logger/advanced_features_test.go
- [[async_test.go]] - code - logger/async_test.go
- [[benchmark_test.go]] - code - logger/benchmark_test.go
- [[caller_debug_test.go]] - code - logger/caller_debug_test.go
- [[caller_test.go]] - code - logger/caller_test.go
- [[fileWithLineNum()]] - code - tools/gorm/gormlog/logger.go
- [[gormLogger]] - code - tools/gorm/gormlog/logger.go
- [[helperFunction()]] - code - logger/caller_test.go
- [[http.go]] - code - sdk/pkg/http.go
- [[log.go]] - code - casbin/log.go
- [[log.go_2]] - code - sdk/pkg/logger/log.go
- [[logger.go_2]] - code - tools/gorm/gormlog/logger.go
- [[performance_benchmark_test.go]] - code - logger/performance_benchmark_test.go
- [[sanitizer_test.go]] - code - logger/sanitizer_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Performance_Tests
SORT file.name ASC
```

## Connections to other communities
- 46 edges to [[_COMMUNITY_Captcha & Preprocessor Tools]]
- 33 edges to [[_COMMUNITY_Sampling & Extended Logger]]
- 30 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 30 edges to [[_COMMUNITY_Config Reader & Observe]]
- 29 edges to [[_COMMUNITY_Log Formatter & Color]]
- 21 edges to [[_COMMUNITY_Storage & Response Models]]
- 17 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 15 edges to [[_COMMUNITY_SDK Binding & Pagination]]
- 14 edges to [[_COMMUNITY_Config Core API]]
- 11 edges to [[_COMMUNITY_Hash & Field Values]]
- 10 edges to [[_COMMUNITY_Configure & Settings]]
- 10 edges to [[_COMMUNITY_HTTP Server Options]]
- 9 edges to [[_COMMUNITY_API Context & Response]]
- 8 edges to [[_COMMUNITY_File Utils & WebSocket]]
- 7 edges to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Runtime ModeEnv]]

## Top bridge nodes
- [[.Error()_10]] - degree 61, connects to 14 communities
- [[.String()_27]] - degree 82, connects to 13 communities
- [[.Close()_3]] - degree 50, connects to 9 communities
- [[NewLogrusLogger()]] - degree 82, connects to 8 communities
- [[.Logf()_6]] - degree 39, connects to 8 communities