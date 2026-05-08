---
type: community
cohesion: 0.17
members: 12
---

# Config Value Types

**Cohesion:** 0.17 - loosely connected
**Members:** 12 nodes

## Members
- [[.Bool()]] - code - config/value.go
- [[.Bytes()_1]] - code - config/value.go
- [[.Duration()]] - code - config/value.go
- [[.Float64()]] - code - config/value.go
- [[.Int()]] - code - config/value.go
- [[.Scan()_1]] - code - config/value.go
- [[.String()_1]] - code - config/value.go
- [[.StringMap()]] - code - config/value.go
- [[.StringSlice()]] - code - config/value.go
- [[newValue()]] - code - config/value.go
- [[value]] - code - config/value.go
- [[value.go]] - code - config/value.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Config_Value_Types
SORT file.name ASC
```

## Connections to other communities
- 1 edge to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_Field Constructors]]

## Top bridge nodes
- [[newValue()]] - degree 3, connects to 2 communities
- [[.Duration()]] - degree 2, connects to 1 community