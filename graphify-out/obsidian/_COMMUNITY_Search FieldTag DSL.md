---
type: community
cohesion: 0.19
members: 17
---

# Search Field/Tag DSL

**Cohesion:** 0.19 - loosely connected
**Members:** 17 nodes

## Members
- [[.SetJoinOn()_1]] - code - tools/search/condition.go
- [[.SetJoinOn()]] - code - tools/search/condition.go
- [[.SetOr()]] - code - tools/search/condition.go
- [[.SetOrder()]] - code - tools/search/condition.go
- [[.SetWhere()]] - code - tools/search/condition.go
- [[Condition]] - code - tools/search/condition.go
- [[Field]] - code - logger/field.go
- [[GormCondition]] - code - tools/search/condition.go
- [[GormJoin]] - code - tools/search/condition.go
- [[GormPublic]] - code - tools/search/condition.go
- [[ResolveSearchQuery()]] - code - tools/search/query.go
- [[condition.go]] - code - tools/search/condition.go
- [[makeTag()]] - code - tools/search/condition.go
- [[otherSql()]] - code - tools/search/query.go
- [[pgSql()]] - code - tools/search/query.go
- [[query.go]] - code - tools/search/query.go
- [[resolveSearchTag]] - code - tools/search/condition.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Search_Field/Tag_DSL
SORT file.name ASC
```

## Connections to other communities
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 2 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 2 edges to [[_COMMUNITY_Memory Queue Append]]
- 1 edge to [[_COMMUNITY_Field Constructors]]
- 1 edge to [[_COMMUNITY_antd_api Bind Constructor]]
- 1 edge to [[_COMMUNITY_API Bind Constructor]]
- 1 edge to [[_COMMUNITY_antd_api Wrapper]]
- 1 edge to [[_COMMUNITY_Excel Writer]]
- 1 edge to [[_COMMUNITY_Search Query Tests]]

## Top bridge nodes
- [[Field]] - degree 8, connects to 5 communities
- [[otherSql()]] - degree 7, connects to 1 community
- [[pgSql()]] - degree 7, connects to 1 community
- [[ResolveSearchQuery()]] - degree 6, connects to 1 community
- [[makeTag()]] - degree 4, connects to 1 community