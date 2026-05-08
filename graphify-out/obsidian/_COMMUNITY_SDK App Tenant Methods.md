---
type: community
cohesion: 0.18
members: 11
---

# SDK App Tenant Methods

**Cohesion:** 0.18 - loosely connected
**Members:** 11 nodes

## Members
- [[.GetConfig()]] - code - sdk/runtime/application.go
- [[.GetDb()]] - code - sdk/runtime/application.go
- [[.GetDbByTenant()]] - code - sdk/runtime/application.go
- [[.GetDefaultTenant()]] - code - sdk/runtime/application.go
- [[.GetHandler()]] - code - sdk/runtime/application.go
- [[.SetApp()]] - code - sdk/runtime/application.go
- [[.SetCasbin()]] - code - sdk/runtime/application.go
- [[.SetCasbinExclude()]] - code - sdk/runtime/application.go
- [[.SetCrontab()]] - code - sdk/runtime/application.go
- [[.SetDb()]] - code - sdk/runtime/application.go
- [[.SetHandler()]] - code - sdk/runtime/application.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/SDK_App_Tenant_Methods
SORT file.name ASC
```

## Connections to other communities
- 11 edges to [[_COMMUNITY_SDK Runtime Application]]
- 2 edges to [[_COMMUNITY_SDK Runtime Queue]]
- 1 edge to [[_COMMUNITY_SDK Casbin Methods]]
- 1 edge to [[_COMMUNITY_SDK Crontab Methods]]
- 1 edge to [[_COMMUNITY_SDK GetConfigValue Methods]]
- 1 edge to [[_COMMUNITY_SDK SetConfigValue Methods]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]

## Top bridge nodes
- [[.GetDefaultTenant()]] - degree 16, connects to 6 communities
- [[.SetHandler()]] - degree 3, connects to 2 communities
- [[.GetDb()]] - degree 3, connects to 1 community
- [[.GetConfig()]] - degree 2, connects to 1 community
- [[.GetDbByTenant()]] - degree 2, connects to 1 community