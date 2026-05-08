---
type: community
cohesion: 0.50
members: 5
---

# Captcha Cache Store

**Cohesion:** 0.50 - moderately connected
**Members:** 5 nodes

## Members
- [[.Get()]] - code - captcha/store.go
- [[.Set()]] - code - captcha/store.go
- [[.Verify()]] - code - captcha/store.go
- [[cacheStore]] - code - captcha/store.go
- [[store.go]] - code - captcha/store.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Captcha_Cache_Store
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 1 edge to [[_COMMUNITY_antd Response Methods]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]

## Top bridge nodes
- [[.Get()]] - degree 4, connects to 2 communities
- [[.Set()]] - degree 2, connects to 1 community
- [[store.go]] - degree 2, connects to 1 community