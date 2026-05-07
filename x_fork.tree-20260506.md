# 專案檔案結構與用途註解(2026-05-06 snapshot)

本檔案對應 `tree` 命令在 `fork260506-go-admin-core/` 根目錄的輸出,
為每個檔案/目錄補上一行用途註解,作為閱讀程式碼前的索引。

- 命名沿用 `x_fork.graphify-20260506.md` 的「snapshot 日期」慣例。
- `graphify-out/` 整個目錄為 graphify 工具自動生成,僅在目錄層級註明用途,
  不深入其內容(內部結構參見 graphify 工具文件)。
- 其餘 Go 原始碼、設定、文件每一檔都附註解。

```
.
├── CHANGELOG.md                       # 人類可讀的版本變更紀錄
├── CLAUDE.md                          # 給 Claude Code 看的專案指令(graphify 規則 + 提示)
├── LICENSE                            # Apache 2.0 授權書
├── README.md                          # 英文 README(招牌:logger 三層 pipeline 效能數字)
├── README.zh-CN.md                    # 簡體中文 README
│
├── captcha/                           # 圖形驗證碼模組
│   ├── captcha.go                     # 驅動初始化 / 設定 driver(digit/string)
│   ├── store.go                       # 驗證碼 store(預設 in-memory)
│   └── store_test.go                  # store 單元測試
│
├── casbin/                            # Casbin RBAC 權限引擎封裝
│   ├── log.go                         # Casbin 內部用的 logger 接線
│   └── mycasbin.go                    # enforcer + adapter 初始化(預設 GORM adapter)
│
├── config/                            # 多來源設定(fork 自 go-micro/config 風格)
│   ├── README.md                      # config 模組總說明
│   ├── config.go                      # Config interface(NewConfig/Load/Watch/Reader)
│   ├── default.go                     # Default Config 實作(loader+reader 組裝)
│   ├── default_test.go                # Default 行為測試
│   ├── options.go                     # Config options(loader/reader/source...)
│   ├── value.go                       # 預設 Value 實作(Bytes/Bool/Int/Map...)
│   │
│   ├── encoder/                       # 序列化編碼器子系統
│   │   ├── encoder.go                 # Encoder interface(Encode/Decode/String)
│   │   ├── json/json.go               # JSON encoder
│   │   ├── toml/toml.go               # TOML encoder
│   │   ├── xml/xml.go                 # XML encoder
│   │   └── yaml/yaml.go               # YAML encoder(預設)
│   │
│   ├── loader/                        # source → reader 的串接層
│   │   ├── loader.go                  # Loader interface(Load/Snapshot/Sync/Watch)
│   │   └── memory/                    # 預設 in-memory loader 實作
│   │       ├── memory.go              # memory loader 主體(merge + watch)
│   │       └── options.go             # memory loader options
│   │
│   ├── reader/                        # 把 source bytes 變成 typed Value
│   │   ├── options.go                 # Reader options(Encoder)
│   │   ├── preprocessor.go            # 字串預處理(env var 插值)
│   │   ├── preprocessor_test.go
│   │   ├── reader.go                  # Reader interface
│   │   └── json/                      # 唯一 Reader 實作(JSON 為共通中介格式)
│   │       ├── json.go                # JSON Reader(Merge/Values/Parse)
│   │       ├── json_test.go
│   │       ├── values.go              # JSON Values 實作(Get/Map/Scan/Bytes)
│   │       └── values_test.go
│   │
│   ├── secrets/                       # config 加密 / 解密
│   │   ├── secrets.go                 # Secrets interface
│   │   ├── box/                       # NaCl box(asymmetric, public-key)
│   │   │   ├── box.go
│   │   │   └── box_test.go
│   │   └── secretbox/                 # NaCl secretbox(symmetric)
│   │       ├── secretbox.go
│   │       └── secretbox_test.go
│   │
│   └── source/                        # 設定資料來源(file/env/flag/memory)
│       ├── changeset.go               # ChangeSet 型別(format/data/timestamp/checksum)
│       ├── noop.go                    # No-op source(測試用 placeholder)
│       ├── options.go                 # 各 source 共用 options 基底
│       ├── source.go                  # Source interface(Read/Watch/Write/String)
│       │
│       ├── env/                       # 環境變數來源
│       │   ├── README.md
│       │   ├── env.go                 # env source 主體(prefix 過濾 + JSON 化)
│       │   ├── env_test.go
│       │   ├── options.go             # env-specific options(StrippedPrefixes)
│       │   └── watcher.go             # env watcher(no-op,env 不會自己變)
│       │
│       ├── file/                      # 檔案來源(yaml/json/toml/xml)
│       │   ├── README.md
│       │   ├── file.go                # file source 主體(讀檔 + format detect)
│       │   ├── file_test.go
│       │   ├── format.go              # 從副檔名推斷 format
│       │   ├── format_test.go
│       │   ├── options.go             # file options(Path)
│       │   ├── watcher.go             # 跨平台 file watcher(fsnotify)
│       │   └── watcher_linux.go       # Linux 專用 inotify 實作(build tag)
│       │
│       ├── flag/                      # CLI flag 來源
│       │   ├── README.md
│       │   ├── flag.go                # flag source(把 std `flag` 當 source)
│       │   ├── flag_test.go
│       │   └── options.go             # flag options(IncludeUnset)
│       │
│       └── memory/                    # in-memory JSON 來源(測試 / 動態注入)
│           ├── README.md
│           ├── memory.go              # memory source 主體
│           ├── options.go             # memory options(ChangeSet)
│           └── watcher.go             # memory watcher(支援動態 Update)
│
├── docs/                              # 設計與遷移文件
│   ├── architecture/                  # 架構決策紀錄
│   │   ├── code-optimization-v2.md    # code-review 後的最佳化清單
│   │   ├── code-review-core-boundary.md # 「core 不放業務邏輯」cleanup 的 review
│   │   ├── code-review-fixes.md       # review 修正紀錄
│   │   ├── logger-architecture-v2.md  # Logger v2(四層架構)設計
│   │   ├── logging-architecture.md    # Logger 整體架構說明(含問題分析、提案)
│   │   └── logging-architecture.pdf   # 同上,印刷版 PDF(10 頁)
│   ├── migration/                     # v1.5 → v1.6 遷移文件
│   │   ├── CODE_REVIEW_REPORT.md      # v1.6 code review 報告
│   │   ├── INTEGRATION_TEST_REPORT.md # 31/31 整合測試報告
│   │   ├── logger-upgrade-v1.6.0.md   # Logger 升級說明
│   │   ├── v1.5-to-v1.6.md            # 6 條路徑對應的遷移指南
│   │   └── v1.6.0-plan.md             # v1.6.0 重構計畫(目標 + 路線圖)
│   └── superpowers/                   # superpowers / brainstorming 產出
│       └── specs/
│           └── 2026-05-07-response-package-design.md # response 套件 spec(本工作流產出)
│
├── errors/                            # 錯誤碼模組
│   ├── error_code.go                  # 錯誤碼常數定義
│   ├── error_code_string.go           # `stringer` 自動生成的 String() 方法
│   ├── errors.go                      # Error/ErrorCoder 主要型別 + helpers
│   ├── errors.pb.go                   # protoc 自動生成
│   ├── errors.proto                   # protobuf schema(error_code 定義來源)
│   └── type.go                        # ErrorCoder interface 宣告
│
├── go.mod                             # Go module 宣告(Go 1.25.1+)
│
├── graphify-out/                      # graphify 知識圖譜輸出目錄(整個目錄由工具生成、勿手改)
│
├── integration_test.go                # 跨子套件相容性測試(v1.6 重構驗證)
│
├── jwtauth/                           # JWT 認證(gin-jwt 包裝)
│   ├── jwtauth.go                     # GinJWTMiddleware 設定 + Claims 抽取
│   └── user/
│       └── user.go                    # 從 gin.Context 取 user info(Id/Name/Role/Dept)
│
├── logger/                            # 核心 logger 模組(專案招牌)
│   ├── README_ADVANCED.md             # 進階用法(Async + Sampling + Sanitizer 組合)
│   ├── advanced_features_test.go      # 進階功能整合測試
│   ├── async.go                       # Async logger(channel queue + drop/block/sample policy)
│   ├── async_test.go
│   ├── benchmark_test.go              # Logger benchmark suite(README 上的數字來源)
│   ├── caller_debug_test.go           # caller 追蹤 debug 用測試
│   ├── caller_test.go                 # caller 行號修正測試
│   ├── config.go                      # Logger config 結構(YAML 對應)
│   ├── console_formatter.go           # 終端 formatter(level 上色 + 結構化欄位)
│   ├── context.go                     # `loggerKey` + FromContext / NewContext
│   ├── default.go                     # DefaultConfig + 預設 Logger 初始化
│   ├── examples_test.go               # godoc Example(被 README 引用)
│   ├── factory.go                     # Logger factory(根據 config 選 adapter + 套 plugin)
│   ├── field.go                       # zero-allocation Field 系統(Any/Time/Int/...)
│   ├── helper.go                      # Helper / 短手 API(Debugf/Infof/...)
│   ├── level.go                       # Level + 全域 Trace/Debug/Info/Warn/Error/Fatal
│   ├── logger.go                      # Logger interface(專案核心抽象)
│   ├── logger_test.go
│   ├── logrus.go                      # Logrus adapter(專案預設,生態 50+ hooks)
│   ├── options.go                     # Logger options(WithPath/WithLevel/...)
│   ├── performance_benchmark_test.go  # 進階 benchmark(壓力測試 / 高併發)
│   ├── pii_mask.go                    # PII mask hook(zap core 形式)
│   ├── pii_mask_logrus.go             # PII mask hook(logrus 形式)
│   ├── pii_mask_test.go
│   ├── sampling.go                    # Sampling logger(N initial 然後 1/M)
│   ├── sanitizer.go                   # Sanitizer logger(mask/hash/remove 三策略)
│   ├── sanitizer_test.go
│   ├── test.log                       # 測試產出檔(理應由 .gitignore 排除,留意)
│   ├── writer/                        # 檔案寫入子模組
│   │   ├── file.go                    # 檔案寫入器(lumberjack 包裝,輪轉)
│   │   └── options.go                 # File writer options(MaxSize/MaxAge/...)
│   └── zap.go                         # Zap adapter(替代選擇,效能更高)
│
├── observability/                     # 觀測性(舊路徑,v1.6 後僅保留 alias)
│   └── audit/
│       └── deprecated.go              # 重新匯出 observe/audit(向下相容用)
│
├── observe/                           # 觀測性(v1.6 新路徑)
│   └── audit/
│       ├── log.go                     # Audit log 結構與寫入函式
│       └── options.go                 # Audit options
│
├── response/                          # HTTP response 建構器(本工作流已寫出 spec)
│   ├── antd/                          # Ant Design Pro 風格 preset
│   │   ├── model.go                   # antd Response/Pages/lists/ListData 型別
│   │   └── return.go                  # antd OK/Error/PageOK/UpFileOK/ListOK/Custum
│   ├── model.go                       # 預設 Response/Page 型別
│   ├── return.go                      # 預設 OK/Error/PageOK/Custum
│   └── type.go                        # Responses interface(兩 preset 共用)
│
├── sdk/                               # SDK 容器與通用工具(歷史包袱最重的目錄)
│   ├── antd_api/                      # antd 風格的 api wrapper
│   │   ├── api.go
│   │   └── binding.go
│   │
│   ├── api/                           # gin handler 共用基底
│   │   ├── api.go                     # Api struct(內含 logger / orm / errors)
│   │   ├── binding.go                 # request → struct 綁定 + 驗證 + i18n
│   │   ├── binding_test.go
│   │   ├── request_logger.go          # request logger 中介(此檔案於 v1.6 從 core 搬出)
│   │   └── translate.go               # i18n 翻譯 helper
│   │
│   ├── application.go                 # Application 單例(SDK 容器入口、god node)
│   │
│   ├── config/                        # SDK 層的 settings(YAML 直接 unmarshal 目標)
│   │   ├── application.go             # Application config 子結構
│   │   ├── cache.go                   # Cache 區段
│   │   ├── config.go                  # Settings 集合 + Setup(初始化)
│   │   ├── database.go                # Database / DBResolver 區段
│   │   ├── gen.go                     # code-gen 工具區段
│   │   ├── jwt.go                     # JWT 區段
│   │   ├── logger.go                  # Logger 區段(連結到 logger 模組)
│   │   ├── queue.go                   # Queue 區段
│   │   └── ssl.go                     # SSL 區段
│   │
│   ├── pkg/                           # 雜項工具(v1.6 大部分已搬到 root,留 alias)
│   │   ├── env.go                     # env 變數讀取 helper
│   │   ├── file.go                    # 檔案/路徑 helper(MkDir/PathExist/FileCreate)
│   │   ├── http.go                    # HTTP header / 請求工具
│   │   ├── int.go                     # int↔string 轉換工具
│   │   ├── ip.go                      # ClientIP / GetLocalHost
│   │   ├── security.go                # hash / 隨機字串 / Hmac
│   │   ├── string.go                  # 字串雜項(IsEmpty/Reverse/...)
│   │   ├── textcolor.go               # 終端色彩 ANSI wrapper(Red/Green/...)
│   │   ├── translate.go               # ParseAcceptLanguage
│   │   ├── url.go                     # URL parse / build
│   │   ├── utils.go                   # 雜項上層 wrapper(GenerateMsgIDFromContext 在這)
│   │   │
│   │   ├── captcha/deprecated.go      # 已搬到 root captcha/,留 alias
│   │   ├── casbin/deprecated.go       # 已搬到 root casbin/,留 alias
│   │   ├── jwtauth/deprecated.go      # 已搬到 root jwtauth/,留 alias
│   │   ├── response/deprecated.go     # 已搬到 root response/,留 alias
│   │   ├── logger/log.go              # `Log` audit logger 入口(常被當 god node 引用)
│   │   ├── cronjob/gadmjob.go         # cron job 包裝(robfig/cron)
│   │   ├── table/analysis.go          # 動態子表 / 分表分析
│   │   │
│   │   ├── utils/                     # 又一層 utils 子集(歷史殘留,可考慮整併)
│   │   │   ├── file.go                # 檔案工具子集
│   │   │   ├── file_test.go
│   │   │   ├── json_time.go           # JSONTime(自訂 JSON marshal 的 time.Time)
│   │   │   ├── response.go            # 舊式 response helper(請優先用 root response/)
│   │   │   └── utils.go               # 雜項
│   │   │
│   │   └── ws/ws.go                   # WebSocket Manager(BroadCast/Group/SendOne)
│   │
│   ├── runtime/                       # SDK runtime 介面(讓 application 可換 adapter)
│   │   ├── application.go             # Runtime Application interface
│   │   ├── cache.go                   # Cache adapter interface
│   │   ├── queue.go                   # Queue adapter interface
│   │   ├── queue_test.go
│   │   └── type.go                    # Mode / Runtime 型別
│   │
│   └── service/
│       └── service.go                 # Service runnable 抽象(Server Manager 用)
│
├── server/                            # HTTP server primitives
│   ├── listener/                      # 自訂 listener(ratelimit/healthz hook)
│   │   ├── options.go
│   │   └── server.go
│   ├── manager.go                     # Manager(管理多個 Runnable / graceful shutdown)
│   ├── options.go                     # Server options
│   └── server.go                      # Server interface
│
├── storage/                           # 通用 cache / queue adapter 介面 + memory 實作
│   ├── cache/
│   │   ├── memory.go                  # in-memory Cache 實作
│   │   ├── memory_test.go
│   │   └── message.go                 # Cache message 型別
│   ├── queue/
│   │   ├── memory.go                  # in-memory Queue 實作
│   │   ├── memory_test.go
│   │   └── message.go                 # Queue message 型別
│   └── type.go                        # AdapterCache / AdapterLocker / AdapterQueue 介面
│
├── tools/                             # 補助工具與外掛
│   ├── README.md                      # tools 目錄總說明
│   ├── migrate-v1.6.sh                # v1.6 路徑遷移自動腳本(import path rewrite)
│   │
│   ├── database/                      # DB config 載入工具
│   │   ├── config.go                  # DB config 設定載入(from YAML)
│   │   ├── config_test.go
│   │   └── type.go                    # Database / DBResolverConfig 型別
│   │
│   ├── gorm/                          # GORM 整合
│   │   ├── gormlog/
│   │   │   ├── logger.go              # GORM logger(修正 caller file/line 顯示)
│   │   │   └── logger_test.go
│   │   └── logger/
│   │       └── deprecated.go          # 舊路徑 alias → gormlog
│   │
│   ├── language/
│   │   └── parser.go                  # Accept-Language parser(語系優先序)
│   │
│   ├── poster/                        # 圖文海報生成(QR / 文字 / 合成)
│   │   ├── poster.go                  # 海報主流程(MergeImage/DrawText)
│   │   └── source.go                  # 海報資源(QR、字型、底圖)載入
│   │
│   ├── search/                        # struct-tag DSL 查詢構建器
│   │   ├── README.md
│   │   ├── condition.go               # 條件構建(exact/contains/gt/in/order)
│   │   ├── query.go                   # ResolveSearchQuery 主流程
│   │   └── query_test.go
│   │
│   ├── transfer/
│   │   └── gin.go                     # Gin context → 自訂 context 的轉接
│   │
│   └── utils/
│       ├── excel.go                   # Excel 寫入(xlsx)
│       └── grpc_header.go             # gRPC header 工具
│
├── x_fork.branch-origin.md            # fork 由來說明(main 從 dev 拉出 / master 停滯原因)
└── x_fork.graphify-20260506.md        # graphify session 紀錄(本次 fork 生圖譜的過程)
```

---

## 補充說明

**幾個重要慣例**:

- `*_test.go` 一律是 Go 標準測試檔(同檔案的單元測試 / 整合測試 / 範例)。
- `deprecated.go` 一律是 v1.6 遷移留下的「舊路徑 alias」(zero-cost type alias
  + thin re-export),內容只有 `import` + `type X = realpkg.X`。
  → 這是憲法 Principle IV(Backward Compatibility Within MAJOR)的具體落地。
- `options.go` + `Option func(...)` 是專案通用的 functional options pattern,
  幾乎每個子模組都有自己一份。
- `README.md`(子目錄裡的)通常是該子套件的使用範例,不是英文 / 中文版總 README。
- `x_fork.*` 開頭的檔案都是這份 fork 的 meta 紀錄,不影響任何程式邏輯,
  可安全忽略或刪除(可參考 `x_fork.branch-origin.md` 的尾註)。

**最常被引用的 god nodes**(來自 graphify GRAPH_REPORT):

| 節點 | 所在檔案 | 邊數 |
|---|---|---|
| `Log` | `sdk/pkg/logger/log.go` | 94 |
| `NewLogrusLogger()` | `logger/logrus.go` | 82 |
| `WithLevel()` | `logger/options.go` | 72 |
| `Application` | `sdk/application.go` | 62 |
| `WithOutput()` | `logger/options.go` | 61 |
| `Errorf()` | `logger/level.go` | 44 |
| `New()` | 多處(captcha/errors/...) | 43 |
| `NewSanitizerLogger()` | `logger/sanitizer.go` | 27 |
| `NewAsyncLogger()` | `logger/async.go` | 26 |
| `GinJWTMiddleware` | `jwtauth/jwtauth.go` | 22 |

讀程式碼建議從這幾個入口往外爬,效率最高。

---

*本檔案於 2026-05-07 由 Claude Code 依 `tree` 輸出生成,日期 `20260506`
沿用 fork 的 snapshot 命名慣例(對齊 `x_fork.graphify-20260506.md`)。*
