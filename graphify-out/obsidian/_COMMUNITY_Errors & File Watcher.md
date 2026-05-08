---
type: community
cohesion: 0.07
members: 50
---

# Errors & File Watcher

**Cohesion:** 0.07 - loosely connected
**Members:** 50 nodes

## Members
- [[.Add()]] - code - server/server.go
- [[.CheckIfTokenExpire()]] - code - jwtauth/jwtauth.go
- [[.Code()]] - code - errors/error_code.go
- [[.Error()]] - code - errors/errors.go
- [[.GetClaimsFromJWT()]] - code - jwtauth/jwtauth.go
- [[.LoginHandler()]] - code - jwtauth/jwtauth.go
- [[.MiddlewareFunc()]] - code - jwtauth/jwtauth.go
- [[.MiddlewareInit()]] - code - jwtauth/jwtauth.go
- [[.Next()_3]] - code - config/source/file/watcher_linux.go
- [[.ParseToken()]] - code - jwtauth/jwtauth.go
- [[.ParseTokenString()]] - code - jwtauth/jwtauth.go
- [[.Read()]] - code - config/source/file/file.go
- [[.RefreshHandler()]] - code - jwtauth/jwtauth.go
- [[.RefreshToken()]] - code - jwtauth/jwtauth.go
- [[.Stop()_3]] - code - config/source/file/watcher_linux.go
- [[.String()_13]] - code - errors/error_code_string.go
- [[.String()_10]] - code - config/source/file/file.go
- [[.TokenGenerator()]] - code - jwtauth/jwtauth.go
- [[.Watch()_2]] - code - config/source/file/file.go
- [[.Write()]] - code - config/source/file/file.go
- [[.jwtFromCookie()]] - code - jwtauth/jwtauth.go
- [[.jwtFromHeader()]] - code - jwtauth/jwtauth.go
- [[.jwtFromParam()]] - code - jwtauth/jwtauth.go
- [[.jwtFromQuery()]] - code - jwtauth/jwtauth.go
- [[.middlewareImpl()]] - code - jwtauth/jwtauth.go
- [[.privateKey()]] - code - jwtauth/jwtauth.go
- [[.publicKey()]] - code - jwtauth/jwtauth.go
- [[.readKeys()]] - code - jwtauth/jwtauth.go
- [[.signedString()]] - code - jwtauth/jwtauth.go
- [[.unauthorized()]] - code - jwtauth/jwtauth.go
- [[.usingPublicKeyAlgo()]] - code - jwtauth/jwtauth.go
- [[ErrorCode]] - code - errors/error_code_string.go
- [[ExtractClaims()]] - code - jwtauth/jwtauth.go
- [[ExtractClaimsFromToken()]] - code - jwtauth/jwtauth.go
- [[FromError()]] - code - errors/errors.go
- [[GetToken()]] - code - jwtauth/jwtauth.go
- [[GinJWTMiddleware]] - code - jwtauth/jwtauth.go
- [[MapClaims]] - code - jwtauth/jwtauth.go
- [[New()]] - code - errors/errors.go
- [[New()_1]] - code - jwtauth/jwtauth.go
- [[Parse()]] - code - errors/errors.go
- [[error_code.go]] - code - errors/error_code.go
- [[errors.go]] - code - errors/errors.go
- [[file]] - code - config/source/file/file.go
- [[jwtauth.go]] - code - jwtauth/jwtauth.go
- [[newWatcher()_1]] - code - config/source/file/watcher_linux.go
- [[newWatcher()]] - code - config/source/file/watcher.go
- [[watcher_2]] - code - config/source/file/watcher_linux.go
- [[watcher.go]] - code - config/source/file/watcher.go
- [[watcher_linux.go]] - code - config/source/file/watcher_linux.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Errors__File_Watcher
SORT file.name ASC
```

## Connections to other communities
- 7 edges to [[_COMMUNITY_AsyncSamplingSanitizer Tests]]
- 5 edges to [[_COMMUNITY_Formatters & Conversion Helpers]]
- 4 edges to [[_COMMUNITY_CacheCaptchaMemory Tests Mix]]
- 3 edges to [[_COMMUNITY_Field Constructors]]
- 3 edges to [[_COMMUNITY_antd Response Methods]]
- 2 edges to [[_COMMUNITY_File Writer  Format Tests]]
- 2 edges to [[_COMMUNITY_Source Test Helpers]]
- 2 edges to [[_COMMUNITY_Hash  Field  Table Utils]]
- 2 edges to [[_COMMUNITY_Listener & HTTP Server Options]]
- 1 edge to [[_COMMUNITY_Config Loader Memory]]
- 1 edge to [[_COMMUNITY_Source Watcher]]
- 1 edge to [[_COMMUNITY_File Source + GORM Logger]]
- 1 edge to [[_COMMUNITY_Database Resolver Config]]
- 1 edge to [[_COMMUNITY_Config Core API]]
- 1 edge to [[_COMMUNITY_Error Descriptor Methods]]
- 1 edge to [[_COMMUNITY_Cache Memory Operations]]
- 1 edge to [[_COMMUNITY_JSON Reader & Preprocessor]]
- 1 edge to [[_COMMUNITY_Search Query Tests]]

## Top bridge nodes
- [[.Add()]] - degree 16, connects to 7 communities
- [[.Read()]] - degree 6, connects to 4 communities
- [[.MiddlewareInit()]] - degree 8, connects to 3 communities
- [[.middlewareImpl()]] - degree 7, connects to 3 communities
- [[.ParseToken()]] - degree 12, connects to 2 communities