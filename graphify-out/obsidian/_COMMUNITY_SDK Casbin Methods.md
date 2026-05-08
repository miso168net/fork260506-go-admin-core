---
type: community
cohesion: 1.00
members: 2
---

# SDK Casbin Methods

**Cohesion:** 1.00 - tightly connected
**Members:** 2 nodes

## Members
- [[.GetCasbin()]] - code - sdk/runtime/application.go
- [[.GetCasbinByTenant()]] - code - sdk/runtime/application.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/SDK_Casbin_Methods
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_SDK Runtime Application]]
- 1 edge to [[_COMMUNITY_SDK App Tenant Methods]]

## Top bridge nodes
- [[.GetCasbin()]] - degree 3, connects to 2 communities
- [[.GetCasbinByTenant()]] - degree 2, connects to 1 community