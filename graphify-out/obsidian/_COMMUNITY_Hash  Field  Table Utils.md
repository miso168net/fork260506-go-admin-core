---
type: community
cohesion: 0.10
members: 33
---

# Hash / Field / Table Utils

**Cohesion:** 0.10 - loosely connected
**Members:** 33 nodes

## Members
- [[Crc16Hash()]] - code - sdk/pkg/table/analysis.go
- [[Crc32Hash()]] - code - sdk/pkg/table/analysis.go
- [[Crc8Hash()]] - code - sdk/pkg/table/analysis.go
- [[CreateSubTable()]] - code - sdk/pkg/table/analysis.go
- [[DynamicTable()]] - code - sdk/pkg/table/analysis.go
- [[ExtractClaims()_1]] - code - jwtauth/user/user.go
- [[GenerateRandomKey16()]] - code - sdk/pkg/security.go
- [[GenerateRandomKey20()]] - code - sdk/pkg/security.go
- [[GenerateRandomKey6()]] - code - sdk/pkg/security.go
- [[Get()_1]] - code - jwtauth/user/user.go
- [[GetCurrentTime()]] - code - sdk/pkg/string.go
- [[GetCurrentTimeStr()]] - code - sdk/pkg/string.go
- [[GetDeptId()]] - code - jwtauth/user/user.go
- [[GetDeptName()]] - code - jwtauth/user/user.go
- [[GetRoleId()]] - code - jwtauth/user/user.go
- [[GetRoleName()]] - code - jwtauth/user/user.go
- [[GetUserId()]] - code - jwtauth/user/user.go
- [[GetUserIdStr()]] - code - jwtauth/user/user.go
- [[GetUserName()]] - code - jwtauth/user/user.go
- [[Int()]] - code - logger/field.go
- [[Int64ToString()]] - code - sdk/pkg/int.go
- [[IntToString()]] - code - sdk/pkg/int.go
- [[Round()]] - code - sdk/pkg/int.go
- [[SetPassword()]] - code - sdk/pkg/security.go
- [[StringToInt()]] - code - sdk/pkg/string.go
- [[StructToJsonStr()]] - code - sdk/pkg/string.go
- [[UIntToString()]] - code - sdk/pkg/int.go
- [[analysis.go]] - code - sdk/pkg/table/analysis.go
- [[generateRandString()]] - code - sdk/pkg/security.go
- [[int.go]] - code - sdk/pkg/int.go
- [[security.go]] - code - sdk/pkg/security.go
- [[string.go]] - code - sdk/pkg/string.go
- [[user.go]] - code - jwtauth/user/user.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Hash_/_Field_/_Table_Utils
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 4 edges to [[_COMMUNITY_Field Constructors]]
- 2 edges to [[_COMMUNITY_Errors & File Watcher]]
- 2 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_DeprecatedLogger Mixed Tests]]
- 1 edge to [[_COMMUNITY_CacheConfig Del Operations]]
- 1 edge to [[_COMMUNITY_File Writer  Format Tests]]
- 1 edge to [[_COMMUNITY_Source Test Helpers]]

## Top bridge nodes
- [[Int()]] - degree 18, connects to 6 communities
- [[generateRandString()]] - degree 9, connects to 3 communities
- [[GetCurrentTimeStr()]] - degree 10, connects to 1 community
- [[GetUserIdStr()]] - degree 5, connects to 1 community
- [[StringToInt()]] - degree 2, connects to 1 community