# 90 — Security and Privacy

**Severity:** CRITICAL

- Treat all server responses, URL parameters, storage values, and third-party data as untrusted input.
- Prevent XSS; avoid unsafe HTML injection and unsafe URL construction.
- Do not put secrets, private keys, service credentials, or privileged tokens in browser bundles or public environment variables.
- Minimize sensitive data retained in local/session storage, IndexedDB, caches, logs, analytics, and error reports.
- Do not send sensitive fields to analytics or third-party scripts without an explicit product/privacy requirement.
- Use secure cookie/session mechanisms provided by the backend architecture.
- Do not weaken CSP, CORS assumptions, origin checks, or browser security controls just to make development convenient.
- Review third-party scripts, SDKs, iframes, redirects, uploads, downloads, and generated HTML as security boundaries.

Security fixes must be tested against the relevant abuse case, not only the happy path.
