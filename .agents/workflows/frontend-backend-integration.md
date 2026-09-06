# Frontend ↔ Backend Integration Workflow

Use whenever a UI feature consumes or mutates backend data.

1. Inspect frontend API clients/hooks and existing backend contract if available.
2. Map every user action to the exact request/event and response shape.
3. Compare expected fields, IDs, enums, nullable values, pagination, errors, auth, and permissions.
4. Identify missing or incompatible endpoints before writing workaround code.
5. Implement the frontend against the real contract.
6. Use deterministic fixtures only for tests or explicitly isolated development scenarios.
7. Start the application and exercise the real request when the environment permits it.
8. Verify request headers/auth, status handling, response parsing, cache/state updates, optimistic behavior, and visible failure states.
9. Test unauthorized/forbidden and malformed/error responses where relevant.
10. Diagnose the full chain if it fails:

`UI → client → network → route → middleware → handler/service → database/external service → response → client state → UI`

11. Report any boundary that could not be verified.

Never declare a frontend feature complete because a mocked client or static JSON makes the screen render.
