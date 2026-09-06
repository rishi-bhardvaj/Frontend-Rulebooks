# 40 — Authentication and Sessions

**Severity:** CRITICAL  
**Activation:** Model Decision

Inspect the application's actual authentication model before changing auth UI or client behavior.

- Follow the established OAuth/OIDC/session/token flow.
- Do not invent token storage or refresh behavior.
- Do not put sensitive long-lived credentials in browser storage merely for convenience.
- Never expose client secrets, signing keys, service credentials, or server-only API keys to browser code.
- Handle expired sessions deliberately: refresh, reauthenticate, or redirect according to the existing contract.
- Avoid redirect loops and preserve intended return destinations safely.
- Treat authentication state as untrusted until validated by the server/session mechanism.
- Do not hide authorization failures as generic success.

When adding a provider, use `.agents/rules/195-secrets-and-integration-configuration.md` and report the exact configuration location and key names.
