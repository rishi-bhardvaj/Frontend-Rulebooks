# 195 — Secrets and Integration Configuration

**Severity:** CRITICAL

**Activation:** Model Decision whenever implementation requires OAuth, AI APIs, analytics, maps, payments, email, storage, backend URLs, webhooks, feature flags, certificates, third-party APIs, or any credential/configuration value.

The agent MUST give the developer an exact configuration handoff. “Add the API key to your env file” is insufficient.

## Required procedure

1. Inspect the actual repository for `.env*`, config modules, framework conventions, deployment manifests, secret-manager usage, CI/CD configuration, and existing variable names.
2. Reuse the established mechanism unless there is a documented reason not to.
3. For every required value, identify:
   - exact file/path or deployment setting
   - exact variable/config key
   - environment (local/test/staging/production)
   - browser-exposed or server-only
   - required vs optional
   - where the developer obtains the value
   - whether a restart/rebuild is required
   - how to verify it
4. Add or update a safe example configuration when the repository convention supports it.
5. Validate missing configuration with a clear error rather than failing mysteriously at runtime.

## Exposure rules

A browser-exposed value is public by definition. Client-safe IDs may be exposed only when the provider requires it. Secrets, private keys, service credentials, privileged tokens, and signing material must remain server-side or in the deployment secret store.

Never print secrets in logs, commit them, hardcode them, put them in screenshots, or ask the developer to paste them into chat.

## Provider examples

For OAuth, distinguish client/public identifiers from client secrets and redirect URI configuration. For AI APIs and other privileged APIs, keep secret keys on a trusted server boundary unless the provider explicitly defines a safe browser credential model. For maps/analytics/public SDKs, document which key is intentionally public and what domain restrictions apply.

## Final handoff

Include a `Configuration Required` section using `.agents/templates/integration-configuration-report.md`. It must state exact paths, exact names, source of values, environment, exposure, restart/reload needs, and verification commands.

Never invent a path. Inspect the actual project first.

If required credentials or external services are unavailable, implementation may be prepared but the integration status must be `NOT VERIFIED` or `BLOCKED`. Never claim that it works without evidence.
