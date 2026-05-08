---
type: community
cohesion: 0.67
members: 3
---

# IP Helpers

**Cohesion:** 0.67 - moderately connected
**Members:** 3 nodes

## Members
- [[GetLocalHost()]] - code - sdk/pkg/ip.go
- [[GetLocation()]] - code - sdk/pkg/ip.go
- [[ip.go]] - code - sdk/pkg/ip.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/IP_Helpers
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]

## Top bridge nodes
- [[GetLocation()]] - degree 3, connects to 2 communities
- [[GetLocalHost()]] - degree 2, connects to 1 community