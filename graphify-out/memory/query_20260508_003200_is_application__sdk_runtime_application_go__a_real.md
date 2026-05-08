---
type: "query"
date: "2026-05-08T00:32:00.882413+00:00"
question: "Is Application (sdk/runtime/application.go) a real god node, or are its 62 edges INFERRED-inflated like Log was?"
contributor: "graphify"
source_nodes: ["Application", "Log", "runtime_application"]
---

# Q: Is Application (sdk/runtime/application.go) a real god node, or are its 62 edges INFERRED-inflated like Log was?

## Answer

Application is a REAL god node — opposite of Log. All 62 direct edges are EXTRACTED, zero INFERRED, zero AMBIGUOUS. The edges are: 1 'contains' from application.go (file→type) plus 61 'method' edges to its struct methods (SetDb/GetDb/SetCasbin/GetCasbin/SetLogger/GetLogger/SetDbByTenant/SetCasbinByTenant/etc). The Application struct has 17 fields each representing a different subsystem entry point (dbs, casbins, engine, crontab, mux, middlewares, cache, queue, locker, memoryQueue, handler, routers, configs, appRouters, casbinExclude, before, defaultTenant, app), so it's a classic service-locator/DI container. The reason BFS shows it spanning many communities is that each method gets clustered with its own callers (not with the struct), so the struct legitimately bridges 60+ communities. Note: sdk/application.go is a different 6-line file that just declares 'var Runtime runtime.Runtime = runtime.NewConfig()' — the real Application is in sdk/runtime/application.go (id runtime_application, community 9). General lesson: don't trust god node edge counts alone — check EXTRACTED vs INFERRED ratio. Application is structural truth; Log was extraction noise.

## Source Nodes

- Application
- Log
- runtime_application