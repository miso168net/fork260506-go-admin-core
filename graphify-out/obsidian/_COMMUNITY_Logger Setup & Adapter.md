---
type: community
cohesion: 0.04
members: 77
---

# Logger Setup & Adapter

**Cohesion:** 0.04 - loosely connected
**Members:** 77 nodes

## Members
- [[.Fields()_2]] - code - logger/default.go
- [[.Init()_3]] - code - logger/default.go
- [[.Log()_2]] - code - logger/default.go
- [[.Logf()_2]] - code - logger/default.go
- [[.Options()_3]] - code - logger/default.go
- [[.Setup()_1]] - code - sdk/config/logger.go
- [[.String()_16]] - code - logger/default.go
- [[.Validate()]] - code - logger/config.go
- [[.WithError()]] - code - logger/helper.go
- [[.WithFields()]] - code - logger/helper.go
- [[.adapterType()]] - code - sdk/config/logger.go
- [[AdapterConfig]] - code - logger/config.go
- [[AdapterFactory]] - code - logger/factory.go
- [[AsyncPluginConfig]] - code - logger/config.go
- [[Config_1]] - code - logger/config.go
- [[ConsoleConfig]] - code - logger/config.go
- [[CoreConfig]] - code - logger/config.go
- [[DefaultConfig()]] - code - logger/config.go
- [[ExampleFromLegacyConfig()]] - code - logger/examples_test.go
- [[ExampleRegisterAdapter()]] - code - logger/examples_test.go
- [[FileConfig]] - code - logger/config.go
- [[FromLegacyConfig()]] - code - logger/config.go
- [[GetAdapter()]] - code - logger/factory.go
- [[LegacyConfig]] - code - logger/config.go
- [[ListAdapters()]] - code - logger/factory.go
- [[Logger_2]] - code - sdk/config/logger.go
- [[LogrusConfig]] - code - logger/config.go
- [[MetricsPluginConfig]] - code - logger/config.go
- [[NetworkConfig]] - code - logger/config.go
- [[NewDevelopmentLogger()]] - code - logger/factory.go
- [[NewFromConfig()]] - code - logger/factory.go
- [[NewLogger()]] - code - logger/default.go
- [[NewProductionLogger()]] - code - logger/factory.go
- [[NewTestLogger()]] - code - logger/factory.go
- [[Option_4]] - code - logger/options.go
- [[Option_2]] - code - config/reader/options.go
- [[Option_3]] - code - config/source/options.go
- [[Options_4]] - code - logger/options.go
- [[Options_2]] - code - config/reader/options.go
- [[Options_3]] - code - config/source/options.go
- [[OutputConfig]] - code - logger/config.go
- [[PluginsConfig]] - code - logger/config.go
- [[RegisterAdapter()]] - code - logger/factory.go
- [[RotationConfig]] - code - sdk/config/logger.go
- [[SamplingPluginConfig]] - code - logger/config.go
- [[SanitizePluginConfig]] - code - logger/config.go
- [[SanitizeRule]] - code - logger/config.go
- [[SetOption()]] - code - logger/options.go
- [[SetupLogger()]] - code - logger/factory.go
- [[TracingPluginConfig]] - code - logger/config.go
- [[WithAsync()]] - code - logger/options.go
- [[WithCallerSkipCount()]] - code - logger/options.go
- [[WithEnableCaller()]] - code - logger/options.go
- [[WithEncoder()]] - code - logger/options.go
- [[WithRotation()]] - code - logger/options.go
- [[WithSampling()]] - code - logger/options.go
- [[WithSanitizer()]] - code - logger/options.go
- [[WithStdout()]] - code - logger/options.go
- [[ZapConfig]] - code - logger/config.go
- [[ZapSamplingConfig]] - code - logger/config.go
- [[ZerologConfig]] - code - logger/config.go
- [[applyPlugins()]] - code - logger/factory.go
- [[buildAdapterOptions()]] - code - logger/factory.go
- [[config.go_1]] - code - logger/config.go
- [[copyFields()]] - code - logger/default.go
- [[default.go_1]] - code - logger/default.go
- [[defaultLogger]] - code - logger/default.go
- [[factory.go]] - code - logger/factory.go
- [[init()_1]] - code - logger/default.go
- [[init()_2]] - code - logger/factory.go
- [[isValidLevel()]] - code - logger/config.go
- [[logCallerfilePath()]] - code - logger/default.go
- [[logger.go_1]] - code - sdk/config/logger.go
- [[options.go_2]] - code - config/reader/options.go
- [[options.go_3]] - code - config/source/options.go
- [[options.go_7]] - code - logger/options.go
- [[parseLevel()]] - code - logger/factory.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Logger_Setup_&_Adapter
SORT file.name ASC
```

## Connections to other communities
- 17 edges to [[_COMMUNITY_Logger Performance Tests]]
- 6 edges to [[_COMMUNITY_Captcha & Preprocessor Tools]]
- 5 edges to [[_COMMUNITY_Config Reader & Observe]]
- 4 edges to [[_COMMUNITY_Log Formatter & Color]]
- 4 edges to [[_COMMUNITY_Logrus Adapter Methods]]
- 4 edges to [[_COMMUNITY_Hash & Field Values]]
- 4 edges to [[_COMMUNITY_SDK Binding & Pagination]]
- 3 edges to [[_COMMUNITY_Storage & Response Models]]
- 3 edges to [[_COMMUNITY_API Context & Response]]
- 3 edges to [[_COMMUNITY_Sampling & Extended Logger]]
- 2 edges to [[_COMMUNITY_Config Core API]]

## Top bridge nodes
- [[NewFromConfig()]] - degree 17, connects to 6 communities
- [[.Setup()_1]] - degree 14, connects to 6 communities
- [[options.go_7]] - degree 17, connects to 5 communities
- [[.Logf()_2]] - degree 12, connects to 3 communities
- [[init()_1]] - degree 5, connects to 3 communities