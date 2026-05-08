---
type: community
cohesion: 0.16
members: 17
---

# YAML Encoder + JSON Reader

**Cohesion:** 0.16 - loosely connected
**Members:** 17 nodes

## Members
- [[.Decode()_3]] - code - config/encoder/yaml/yaml.go
- [[.Encode()_3]] - code - config/encoder/yaml/yaml.go
- [[.Merge()]] - code - config/reader/json/json.go
- [[.String()_7]] - code - config/reader/json/json.go
- [[.String()_5]] - code - config/encoder/yaml/yaml.go
- [[GetImage()]] - code - tools/poster/source.go
- [[NewEncoder()_3]] - code - config/encoder/yaml/yaml.go
- [[NewOptions()]] - code - config/source/options.go
- [[NewReader()]] - code - config/reader/json/json.go
- [[TestReader()]] - code - config/reader/json/json_test.go
- [[getResourceReader()]] - code - tools/poster/source.go
- [[json.go_1]] - code - config/reader/json/json.go
- [[jsonReader]] - code - config/reader/json/json.go
- [[json_test.go]] - code - config/reader/json/json_test.go
- [[source.go_1]] - code - tools/poster/source.go
- [[yaml.go]] - code - config/encoder/yaml/yaml.go
- [[yamlEncoder]] - code - config/encoder/yaml/yaml.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/YAML_Encoder__JSON_Reader
SORT file.name ASC
```

## Connections to other communities
- 3 edges to [[_COMMUNITY_Config Core API]]
- 3 edges to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 3 edges to [[_COMMUNITY_Config Loader Memory]]
- 2 edges to [[_COMMUNITY_ReaderSource Options]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_TOML Encoder]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]
- 1 edge to [[_COMMUNITY_Source Watcher]]
- 1 edge to [[_COMMUNITY_File  Path Utils]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]

## Top bridge nodes
- [[TestReader()]] - degree 8, connects to 6 communities
- [[NewOptions()]] - degree 7, connects to 4 communities
- [[getResourceReader()]] - degree 7, connects to 4 communities
- [[NewReader()]] - degree 8, connects to 3 communities
- [[.Merge()]] - degree 7, connects to 3 communities