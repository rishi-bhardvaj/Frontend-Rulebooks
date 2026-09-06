# 60 — State Ownership

**Severity:** HIGH  
**Activation:** Model Decision

For each state value, identify its owner and lifecycle before introducing or moving it.

Possible ownership includes server/cache state, URL state, form draft state, local component state, shared client state, optimistic state, persisted local state, or hydrated server state.

- Keep one authoritative source where possible.
- Do not copy server state into global state without a reason.
- Put shareable/filterable navigation state in the URL when the product requires deep links.
- Preserve form drafts when validation or navigation semantics require it.
- Reconcile optimistic updates with server responses and failures.
- Avoid effects that merely synchronize duplicated state when derivation is sufficient.
- Consider reload, back/forward, multiple tabs, offline, and stale-data behavior where relevant.

Document the state transition for material features before implementation.
