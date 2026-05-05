---
type: community
cohesion: 0.05
members: 62
---

# Errors & File Watcher

**Cohesion:** 0.05 - loosely connected
**Members:** 62 nodes

## Members
- [[.Add()]] - code - server/server.go
- [[.CheckIfTokenExpire()]] - code - jwtauth/jwtauth.go
- [[.Code()]] - code - errors/error_code.go
- [[.Descriptor()]] - code - errors/errors.pb.go
- [[.Error()]] - code - errors/errors.go
- [[.GetClaimsFromJWT()]] - code - jwtauth/jwtauth.go
- [[.GetDomain()]] - code - errors/errors.pb.go
- [[.GetErrorCode()]] - code - errors/errors.pb.go
- [[.GetErrorMessage()]] - code - errors/errors.pb.go
- [[.GetShowType()]] - code - errors/errors.pb.go
- [[.GetSuccess()]] - code - errors/errors.pb.go
- [[.GetTraceId()]] - code - errors/errors.pb.go
- [[.LoginHandler()]] - code - jwtauth/jwtauth.go
- [[.MiddlewareFunc()]] - code - jwtauth/jwtauth.go
- [[.MiddlewareInit()]] - code - jwtauth/jwtauth.go
- [[.Next()_3]] - code - config/source/file/watcher_linux.go
- [[.ParseToken()]] - code - jwtauth/jwtauth.go
- [[.ParseTokenString()]] - code - jwtauth/jwtauth.go
- [[.ProtoMessage()]] - code - errors/errors.pb.go
- [[.ProtoReflect()]] - code - errors/errors.pb.go
- [[.RefreshHandler()]] - code - jwtauth/jwtauth.go
- [[.RefreshToken()]] - code - jwtauth/jwtauth.go
- [[.Stop()_3]] - code - config/source/file/watcher_linux.go
- [[.String()_12]] - code - errors/errors.pb.go
- [[.String()_13]] - code - errors/error_code_string.go
- [[.TokenGenerator()]] - code - jwtauth/jwtauth.go
- [[.Watch()_2]] - code - config/source/file/file.go
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
- [[Equal()]] - code - errors/errors.go
- [[Error]] - code - errors/errors.pb.go
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
- [[errors.pb.go]] - code - errors/errors.pb.go
- [[file_errors_proto_init()]] - code - errors/errors.pb.go
- [[file_errors_proto_rawDescGZIP()]] - code - errors/errors.pb.go
- [[init()]] - code - errors/errors.pb.go
- [[jwtauth.go]] - code - jwtauth/jwtauth.go
- [[newWatcher()_1]] - code - config/source/file/watcher_linux.go
- [[newWatcher()]] - code - config/source/file/watcher.go
- [[watcher_2]] - code - config/source/file/watcher_linux.go
- [[watcher.go]] - code - config/source/file/watcher.go
- [[watcher_linux.go]] - code - config/source/file/watcher_linux.go

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Errors_&_File_Watcher
SORT file.name ASC
```

## Connections to other communities
- 8 edges to [[_COMMUNITY_Storage & Response Models]]
- 7 edges to [[_COMMUNITY_Logger Performance Tests]]
- 5 edges to [[_COMMUNITY_Log Formatter & Color]]
- 5 edges to [[_COMMUNITY_Hash & Field Values]]
- 4 edges to [[_COMMUNITY_Config Core API]]
- 3 edges to [[_COMMUNITY_Config Reader & Observe]]
- 2 edges to [[_COMMUNITY_HTTP Server Options]]
- 1 edge to [[_COMMUNITY_Captcha & Preprocessor Tools]]
- 1 edge to [[_COMMUNITY_SDK Binding & Pagination]]

## Top bridge nodes
- [[.Add()]] - degree 16, connects to 6 communities
- [[.MiddlewareInit()]] - degree 8, connects to 3 communities
- [[.middlewareImpl()]] - degree 7, connects to 3 communities
- [[.ParseToken()]] - degree 12, connects to 2 communities
- [[.jwtFromHeader()]] - degree 4, connects to 2 communities