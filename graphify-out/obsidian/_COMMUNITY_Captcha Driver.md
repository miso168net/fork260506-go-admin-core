---
type: community
cohesion: 0.33
members: 6
---

# Captcha Driver

**Cohesion:** 0.33 - loosely connected
**Members:** 6 nodes

## Members
- [[DriverDigitFunc()]] - code - captcha/captcha.go
- [[DriverStringFunc()]] - code - captcha/captcha.go
- [[SetStore()]] - code - captcha/captcha.go
- [[Verify()]] - code - captcha/captcha.go
- [[captcha.go]] - code - captcha/captcha.go
- [[configJsonBody]] - code - captcha/captcha.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Captcha_Driver
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]

## Top bridge nodes
- [[DriverDigitFunc()]] - degree 3, connects to 2 communities
- [[DriverStringFunc()]] - degree 3, connects to 2 communities
- [[Verify()]] - degree 2, connects to 1 community