# 200 — Mock and Placeholder Detection

**Severity:** CRITICAL

Before declaring completion, inspect the change and affected paths for:

- TODO / FIXME / HACK markers added for unfinished work
- placeholder copy
- fake records or fake metrics
- mocked API calls left in production paths
- stubbed event handlers
- hardcoded success/error responses
- temporary bypasses
- disabled validation
- skipped tests
- dead branches and unreachable fallback behavior

Mocks are acceptable inside explicitly scoped tests and development tooling when they are clearly isolated. They are not evidence that a required production integration works.

If a placeholder is intentionally retained, explain why, who owns the follow-up, and why the feature is still considered complete or incomplete.
