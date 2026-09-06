# 280 — Realtime and Background UI

**Severity:** HIGH when applicable

For WebSocket, SSE, polling, notifications, background jobs, or live dashboards:

- Identify the source of truth and lifecycle of the connection/subscription.
- Clean up subscriptions and timers.
- Handle reconnects, disconnects, stale data, duplicate events, and out-of-order updates where relevant.
- Do not assume a successful connection means messages are valid.
- Surface connection state only when it helps users understand behavior.
- Avoid polling intervals that create unnecessary load.
- Test initial connection, reconnect, failure, duplicate event, and stale-data behavior when relevant.

The UI must reflect actual backend/event semantics rather than simulating live behavior with timers or random updates.
