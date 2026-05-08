---
type: community
cohesion: 0.70
members: 5
---

# gRPC Header Helpers

**Cohesion:** 0.70 - tightly connected
**Members:** 5 nodes

## Members
- [[GetHeaderFirst()]] - code - tools/utils/grpc_header.go
- [[GetRequestID()]] - code - tools/utils/grpc_header.go
- [[GetUsername()]] - code - tools/utils/grpc_header.go
- [[NewRequestID()]] - code - tools/utils/grpc_header.go
- [[grpc_header.go]] - code - tools/utils/grpc_header.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/gRPC_Header_Helpers
SORT file.name ASC
```

## Connections to other communities
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_Formatters & Conversion Helpers]]

## Top bridge nodes
- [[GetHeaderFirst()]] - degree 5, connects to 2 communities
- [[NewRequestID()]] - degree 4, connects to 2 communities