# 250 — Observability and Client Failures

**Severity:** HIGH

- Use the repository's existing error reporting and telemetry mechanism.
- Capture actionable failures without collecting unnecessary sensitive data.
- Preserve useful context such as route, operation, request correlation ID, and safe error category where available.
- Do not log tokens, credentials, personal data, or full sensitive responses.
- Make user-visible failures recoverable where possible.
- Distinguish expected user errors from unexpected application failures.
- Avoid duplicate telemetry caused by multiple rendering/effect paths.

Observability must help diagnose a real failure without becoming a privacy leak.
