---
type: community
cohesion: 0.08
members: 122
---

# Async/Sampling/Sanitizer Tests

**Cohesion:** 0.08 - loosely connected
**Members:** 122 nodes

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
- [[.LogModel()]] - code - casbin/log.go
- [[.LogPolicy()]] - code - casbin/log.go
- [[.LogRole()]] - code - casbin/log.go
- [[.Logf()_6]] - code - logger/zap.go
- [[.Options()_8]] - code - server/listener/server.go
- [[.Reset()]] - code - errors/errors.pb.go
- [[.String()_27]] - code - storage/queue/memory.go
- [[.Trace()]] - code - logger/helper.go
- [[.Tracef()]] - code - logger/helper.go
- [[.Warn()_1]] - code - logger/helper.go
- [[.Warnf()]] - code - logger/helper.go
- [[.Warnw()]] - code - logger/helper.go
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
- [[BenchmarkLogrusLogger()]] - code - logger/examples_test.go
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
- [[ExampleNewLogrusLogger()]] - code - logger/examples_test.go
- [[Get()_2]] - code - sdk/pkg/http.go
- [[Helper]] - code - logger/helper.go
- [[Log]] - code - observe/audit/log.go
- [[Logger]] - code - casbin/log.go
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
- [[helperFunction()]] - code - logger/caller_test.go
- [[http.go]] - code - sdk/pkg/http.go
- [[log.go]] - code - casbin/log.go
- [[log.go_2]] - code - sdk/pkg/logger/log.go
- [[performance_benchmark_test.go]] - code - logger/performance_benchmark_test.go
- [[sanitizer_test.go]] - code - logger/sanitizer_test.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Async/Sampling/Sanitizer_Tests
SORT file.name ASC
```

## Connections to other communities
- 28 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 22 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 17 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 16 edges to [[_COMMUNITY_Database Resolver Config]]
- 15 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 13 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 11 edges to [[_COMMUNITY_Default Config Tests]]
- 11 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 10 edges to [[_COMMUNITY_File Source + GORM Logger]]
- 10 edges to [[_COMMUNITY_Source Test Helpers]]
- 10 edges to [[_COMMUNITY_Listener & HTTP Server Options]]
- 8 edges to [[_COMMUNITY_Default Logger Initialization]]
- 8 edges to [[_COMMUNITY_Level Functions]]
- 8 edges to [[_COMMUNITY_File  Path Utils]]
- 7 edges to [[_COMMUNITY_Errors & File Watcher]]
- 7 edges to [[_COMMUNITY_Logger Examples]]
- 7 edges to [[_COMMUNITY_Sampling Logger]]
- 6 edges to [[_COMMUNITY_Config Loader Memory]]
- 6 edges to [[_COMMUNITY_Field Constructors]]
- 6 edges to [[_COMMUNITY_Memory Queue Append]]
- 5 edges to [[_COMMUNITY_Hash  Field  Table Utils]]
- 5 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 5 edges to [[_COMMUNITY_antd_api Wrapper]]
- 4 edges to [[_COMMUNITY_Logger LogfDebugf]]
- 3 edges to [[_COMMUNITY_File Writer  Format Tests]]
- 3 edges to [[_COMMUNITY_Logrus AddHook]]
- 3 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 3 edges to [[_COMMUNITY_Audit FormatFunc & Stream]]
- 3 edges to [[_COMMUNITY_antd Response Methods]]
- 2 edges to [[_COMMUNITY_Captcha Driver]]
- 2 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_Logger Hooks (CallerElasticsearch)]]
- 2 edges to [[_COMMUNITY_IP Helpers]]
- 2 edges to [[_COMMUNITY_Memory Queue Operations]]
- 2 edges to [[_COMMUNITY_Search FieldTag DSL]]
- 1 edge to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_TOML Encoder]]
- 1 edge to [[_COMMUNITY_ReaderSource Options]]
- 1 edge to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 1 edge to [[_COMMUNITY_Error Descriptor Methods]]
- 1 edge to [[_COMMUNITY_Audit OptionsReader]]
- 1 edge to [[_COMMUNITY_Masking Core (PII Mask)]]
- 1 edge to [[_COMMUNITY_antd_api Bind Constructor]]
- 1 edge to [[_COMMUNITY_API Bind Constructor]]
- 1 edge to [[_COMMUNITY_Config Settings & Multi-DB]]
- 1 edge to [[_COMMUNITY_Runtime ModeEnv]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_gRPC Header Helpers]]

## Top bridge nodes
- [[.String()_27]] - degree 82, connects to 27 communities
- [[.Error()_10]] - degree 61, connects to 23 communities
- [[.Close()_3]] - degree 50, connects to 15 communities
- [[.Logf()_6]] - degree 39, connects to 12 communities
- [[NewLogrusLogger()]] - degree 82, connects to 10 communities