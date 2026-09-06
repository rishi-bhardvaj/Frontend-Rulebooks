# 30 — API and Data Fetching

**Severity:** CRITICAL  
**Activation:** Model Decision

Use the repository's established API/data layer. Match the real backend contract exactly: method, path, headers, parameters, request body, response envelope, status codes, pagination, sorting, filtering, and error shape.

- Do not hardcode production API responses.
- Do not treat a mock server as proof of production compatibility.
- Keep server data distinct from local UI state where the architecture supports that distinction.
- Define cache ownership and invalidation for mutations.
- Handle retries only when the operation is safe and the repository pattern supports them.
- Prevent stale or duplicated requests when relevant.
- Preserve cancellation/abort behavior where supported.
- Model loading, empty, partial, success, unauthorized/forbidden, validation, network, and server-error states.
- Verify at least one real request for integration work when credentials/environment permit it.

If the real API cannot be reached, report `NOT VERIFIED` or `BLOCKED`; do not silently substitute fake success.
