---
type: community
cohesion: 0.29
members: 7
---

# Reader/Source Options

**Cohesion:** 0.29 - loosely connected
**Members:** 7 nodes

## Members
- [[Option_2]] - code - config/reader/options.go
- [[Option_3]] - code - config/source/options.go
- [[Options_2]] - code - config/reader/options.go
- [[Options_3]] - code - config/source/options.go
- [[WithEncoder()]] - code - logger/options.go
- [[options.go_2]] - code - config/reader/options.go
- [[options.go_3]] - code - config/source/options.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Reader/Source_Options
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 2 edges to [[_COMMUNITY_Logger Setup & Adapter]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]

## Top bridge nodes
- [[WithEncoder()]] - degree 5, connects to 2 communities
- [[options.go_2]] - degree 4, connects to 1 community
- [[options.go_3]] - degree 4, connects to 1 community