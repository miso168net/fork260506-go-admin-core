---
type: community
cohesion: 0.22
members: 9
---

# SDK Utils (UUID/Hmac/Time)

**Cohesion:** 0.22 - loosely connected
**Members:** 9 nodes

## Members
- [[.Write()_4]] - code - sdk/pkg/ws/ws.go
- [[Base64ToImage()]] - code - sdk/pkg/utils/utils.go
- [[GetCurrentTimeStamp()]] - code - sdk/pkg/utils/utils.go
- [[GetUUID()]] - code - sdk/pkg/utils/utils.go
- [[Hmac()]] - code - sdk/pkg/utils/utils.go
- [[IsStringEmpty()]] - code - sdk/pkg/utils/utils.go
- [[PathExists()]] - code - sdk/pkg/utils/utils.go
- [[RemoveRepByMap()]] - code - sdk/pkg/utils/utils.go
- [[utils.go_1]] - code - sdk/pkg/utils/utils.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/SDK_Utils_UUID/Hmac/Time
SORT file.name ASC
```

## Connections to other communities
- 3 edges to [[_COMMUNITY_Default Config Tests]]
- 3 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_Source Watcher]]
- 2 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_File  Path Utils]]
- 1 edge to [[_COMMUNITY_Default Logger Initialization]]
- 1 edge to [[_COMMUNITY_Masking Core (PII Mask)]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_Memory Queue Append]]

## Top bridge nodes
- [[.Write()_4]] - degree 13, connects to 8 communities
- [[Hmac()]] - degree 4, connects to 2 communities
- [[GetUUID()]] - degree 3, connects to 2 communities
- [[RemoveRepByMap()]] - degree 3, connects to 2 communities
- [[utils.go_1]] - degree 8, connects to 1 community