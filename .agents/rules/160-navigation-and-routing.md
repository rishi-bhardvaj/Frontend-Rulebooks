# 160 — Navigation and Routing

**Severity:** HIGH

- Follow the repository's router and framework conventions.
- Preserve direct navigation, refresh, back/forward, deep links, and intended redirects.
- Treat URL parameters as untrusted input.
- Encode query/path values correctly.
- Keep browser history behavior intentional for modal, filter, search, and multi-step flows.
- Protect authenticated routes using the application's real session mechanism, not only client state.
- Provide meaningful not-found and error routes where the framework supports them.
- Do not create dead links, redirect loops, or routes that work only after navigating from the home page.

Test important routes directly and after a full refresh.
