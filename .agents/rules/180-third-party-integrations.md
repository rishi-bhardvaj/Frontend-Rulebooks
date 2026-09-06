# 180 — Third-Party Integrations

**Severity:** CRITICAL

For OAuth, AI, analytics, maps, payments, storage, chat, monitoring, feature flags, or other third-party services:

1. Inspect the provider SDK/version and the repository's existing integration pattern.
2. Identify whether the integration belongs in browser code, server code, or both.
3. Identify required configuration and exact exposure boundaries.
4. Implement the real integration rather than a fake success path.
5. Handle unavailable credentials or services explicitly.
6. Test success and provider failure behavior.
7. Document exact setup and verification instructions.

Do not expose provider secrets in browser bundles. Do not silently replace a required integration with a mock, local-only implementation, or hardcoded response.

Use `.agents/rules/195-secrets-and-integration-configuration.md` for configuration handoff.
