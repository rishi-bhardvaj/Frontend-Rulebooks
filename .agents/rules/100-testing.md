# 100 — Testing

**Severity:** CRITICAL

Testing should reflect risk and user behavior.

Use the repository's existing layers as appropriate:

- unit tests for pure domain/utility logic
- component tests for interaction and state behavior
- integration tests for API/data boundaries
- E2E/browser tests for critical user journeys

For a feature, cover the main success path plus relevant validation, loading, empty, error, permission, navigation, responsive, accessibility, and retry/recovery states.

Tests must use deterministic data and realistic contracts. Do not change production code merely to satisfy an unrealistic test. Do not treat snapshots as sufficient behavioral verification.

Run the real project commands. Record failures accurately. A test file that was created but not executed is not a passing test.
