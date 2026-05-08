---
type: community
cohesion: 0.18
members: 20
---

# Field Constructors

**Cohesion:** 0.18 - loosely connected
**Members:** 20 nodes

## Members
- [[.Bool()_1]] - code - config/reader/json/values.go
- [[Any()]] - code - logger/field.go
- [[BenchmarkZapLoggerStructured()]] - code - logger/benchmark_test.go
- [[Bool()]] - code - logger/field.go
- [[ClientIP()]] - code - logger/field.go
- [[Duration()]] - code - logger/field.go
- [[ExampleNewLogrusLogger_structuredFields()]] - code - logger/examples_test.go
- [[FieldError()]] - code - logger/field.go
- [[FieldString()]] - code - logger/field.go
- [[FieldType]] - code - logger/field.go
- [[Int64()]] - code - logger/field.go
- [[Latency()]] - code - logger/field.go
- [[Method()]] - code - logger/field.go
- [[RequestID()]] - code - logger/field.go
- [[StatusCode()]] - code - logger/field.go
- [[Time()]] - code - logger/field.go
- [[TraceID()]] - code - logger/field.go
- [[URI()]] - code - logger/field.go
- [[UserID()]] - code - logger/field.go
- [[field.go]] - code - logger/field.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Field_Constructors
SORT file.name ASC
```

## Connections to other communities
- 6 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 6 edges to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 4 edges to [[_COMMUNITY_Hash  Field  Table Utils]]
- 3 edges to [[_COMMUNITY_Errors & File Watcher]]
- 3 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Config Value Types]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Logger Examples]]
- 1 edge to [[_COMMUNITY_Search FieldTag DSL]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]
- 1 edge to [[_COMMUNITY_Memory Queue Operations]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]

## Top bridge nodes
- [[Duration()]] - degree 8, connects to 5 communities
- [[Int64()]] - degree 11, connects to 4 communities
- [[ExampleNewLogrusLogger_structuredFields()]] - degree 10, connects to 3 communities
- [[BenchmarkZapLoggerStructured()]] - degree 7, connects to 3 communities
- [[field.go]] - degree 18, connects to 2 communities