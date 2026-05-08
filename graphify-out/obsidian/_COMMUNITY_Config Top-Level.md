---
type: community
cohesion: 0.22
members: 10
---

# Config Top-Level

**Cohesion:** 0.22 - loosely connected
**Members:** 10 nodes

## Members
- [[Entity]] - code - config/config.go
- [[Get()]] - code - config/config.go
- [[Load()]] - code - config/config.go
- [[LoadFile()]] - code - config/config.go
- [[NewConfig()]] - code - config/config.go
- [[Option]] - code - config/config.go
- [[Options]] - code - config/config.go
- [[Sync()]] - code - config/config.go
- [[Watch()]] - code - config/config.go
- [[config.go]] - code - config/config.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Top-Level
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_Config Core API]]
- 2 edges to [[_COMMUNITY_Default Config Tests]]
- 1 edge to [[_COMMUNITY_TOML Encoder]]
- 1 edge to [[_COMMUNITY_Config Map  Flag  NoOp Source]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Config Loader Memory]]
- 1 edge to [[_COMMUNITY_Source Test Helpers]]

## Top bridge nodes
- [[config.go]] - degree 14, connects to 4 communities
- [[LoadFile()]] - degree 4, connects to 2 communities
- [[Load()]] - degree 3, connects to 1 community
- [[Get()]] - degree 2, connects to 1 community
- [[NewConfig()]] - degree 2, connects to 1 community