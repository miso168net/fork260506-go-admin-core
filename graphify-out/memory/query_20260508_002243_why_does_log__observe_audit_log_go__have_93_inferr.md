---
type: "query"
date: "2026-05-08T00:22:43.387746+00:00"
question: "Why does Log (observe/audit/log.go) have 93 INFERRED edges spanning many communities — real or over-inferred?"
contributor: "graphify"
source_nodes: ["Log", "TestCaptchaCompatibility()", "TestJWTAuthCompatibility()", "TestObserveAuditCompatibility()", "Info()", "Trace()"]
---

# Q: Why does Log (observe/audit/log.go) have 93 INFERRED edges spanning many communities — real or over-inferred?

## Answer

Mostly OVER-INFERRED. The 'Log' node is just a small audit-log interface (Read/Write/Stream methods) in observe/audit/log.go, not an application logger. The high edge count is a false positive: integration_test.go contains 8 Test*Compatibility tests for different packages (captcha/jwtauth/response/casbin/audit/gormlog) all in one file. The semantic subagent saw 'Log' mentioned in that file (via TestObserveAuditCompatibility's 'var _ newaudit.Log') and incorrectly connected Log to ALL Test*Compatibility functions, even those that never touch audit.Log (like TestCaptchaCompatibility which only uses captcha.SetStore/DriverStringFunc/Verify). Real edges from Log: only TestObserveAuditCompatibility (EXTRACTED), plus internal companions Record/Stream/TextFormat/JSONFormat. The Info()/Trace() --calls--> Log edges in Surprising Connections are also false — logger/level.go's level helpers are name-collision matches, not actual callers of the audit interface. True god nodes in this fork are logger.Logger interface, NewLogrusLogger (82 edges), and Application (62 edges).

## Source Nodes

- Log
- TestCaptchaCompatibility()
- TestJWTAuthCompatibility()
- TestObserveAuditCompatibility()
- Info()
- Trace()