# 25 — Frontend Contract Discovery

**Severity:** CRITICAL  
**Activation:** Model Decision when backend/API context, designs, screenshots, API clients, or an existing frontend are supplied.

Treat the frontend as a source of observable product requirements, not as authority over server security.

Inspect routes, pages, forms, tables, filters, pagination, search, sorting, uploads/downloads, dashboards, notifications, dialogs, and state transitions. Inspect API clients/hooks/fetch/axios/GraphQL/WebSocket/SSE/generated clients and hardcoded URLs.

Record for each relevant interaction:

`UI action → client call/event → method/path or event → request shape → response shape/status → state update → persistence/side effect → error handling → tests`

Also inspect headers, cookies/tokens, query/path parameters, multipart bodies, retries/polling, optimistic updates, IDs, timestamps, nullable fields, enums, permissions, tenant/workspace/project context, and ownership assumptions.

Classify findings as `Observed`, `Inferred`, `Assumed`, or `Missing`. Never make the frontend's client-supplied user/role/tenant/ownership values a substitute for server authorization.

If the frontend expects an endpoint that is absent or incompatible, surface the contract gap and coordinate the smallest correct change. Do not weaken security or silently fabricate a backend.
