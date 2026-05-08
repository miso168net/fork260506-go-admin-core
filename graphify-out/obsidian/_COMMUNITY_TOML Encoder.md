---
type: community
cohesion: 0.29
members: 8
---

# TOML Encoder

**Cohesion:** 0.29 - loosely connected
**Members:** 8 nodes

## Members
- [[.Bytes()_3]] - code - config/reader/json/values.go
- [[.Decode()_1]] - code - config/encoder/toml/toml.go
- [[.Encode()_1]] - code - config/encoder/toml/toml.go
- [[.String()_3]] - code - config/encoder/toml/toml.go
- [[Bytes()]] - code - config/config.go
- [[NewEncoder()_1]] - code - config/encoder/toml/toml.go
- [[toml.go]] - code - config/encoder/toml/toml.go
- [[tomlEncoder]] - code - config/encoder/toml/toml.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/TOML_Encoder
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Config Top-Level]]
- 1 edge to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_Config Loader Memory]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]

## Top bridge nodes
- [[.Bytes()_3]] - degree 7, connects to 4 communities
- [[.Encode()_1]] - degree 5, connects to 2 communities
- [[Bytes()]] - degree 2, connects to 1 community