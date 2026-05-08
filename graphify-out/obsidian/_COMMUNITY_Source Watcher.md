---
type: community
cohesion: 0.40
members: 5
---

# Source Watcher

**Cohesion:** 0.40 - moderately connected
**Members:** 5 nodes

## Members
- [[.Sum()]] - code - config/source/changeset.go
- [[ChangeSet]] - code - config/source/source.go
- [[Source]] - code - config/source/source.go
- [[Watcher_1]] - code - config/source/source.go
- [[source.go]] - code - config/source/source.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Source_Watcher
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_Config Loader Memory]]
- 2 edges to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]
- 1 edge to [[_COMMUNITY_YAML Encoder + JSON Reader]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_Errors & File Watcher]]
- 1 edge to [[_COMMUNITY_Config Map  Flag  NoOp Source]]

## Top bridge nodes
- [[.Sum()]] - degree 9, connects to 6 communities