# 50 — Authorization and Permissions

**Severity:** CRITICAL  
**Activation:** Model Decision

Frontend authorization is a user-experience concern, not the security boundary.

- Render controls based on actual authorization state when known.
- Never rely on hidden buttons, disabled inputs, route guards, or client roles to enforce security.
- Do not manufacture permissions from local storage or URL parameters.
- Handle `401` and `403` distinctly where the product contract requires it.
- Do not leak protected resource details in prefetches, error messages, page metadata, or client state.
- For tenant/workspace/project/ownership features, verify that the server supplies authoritative context.
- Test both allowed and denied flows.

When a permission is missing from the backend contract, surface the gap rather than bypassing it in the UI.
