---
type: community
cohesion: 0.21
members: 13
---

# Masking Core (PII Mask)

**Cohesion:** 0.21 - loosely connected
**Members:** 13 nodes

## Members
- [[.Check()]] - code - logger/pii_mask.go
- [[.Fire()_4]] - code - logger/pii_mask_logrus.go
- [[.Levels()_4]] - code - logger/pii_mask_logrus.go
- [[.Sync()_4]] - code - logger/pii_mask.go
- [[.With()_2]] - code - logger/pii_mask.go
- [[.Write()_3]] - code - logger/pii_mask.go
- [[GetMasker()]] - code - logger/pii_mask.go
- [[Masker]] - code - logger/pii_mask.go
- [[maskFields()]] - code - logger/pii_mask.go
- [[maskingCore]] - code - logger/pii_mask.go
- [[piiMaskHook]] - code - logger/pii_mask_logrus.go
- [[pii_mask.go]] - code - logger/pii_mask.go
- [[pii_mask_logrus.go]] - code - logger/pii_mask_logrus.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Masking_Core_PII_Mask
SORT file.name ASC
```

## Connections to other communities
- 4 edges to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 1 edge to [[_COMMUNITY_AsyncSamplingSanitizerZap Combinators]]
- 1 edge to [[_COMMUNITY_SDK Utils (UUIDHmacTime)]]

## Top bridge nodes
- [[pii_mask.go]] - degree 6, connects to 1 community
- [[GetMasker()]] - degree 5, connects to 1 community
- [[maskFields()]] - degree 5, connects to 1 community
- [[.Write()_3]] - degree 4, connects to 1 community
- [[.With()_2]] - degree 3, connects to 1 community