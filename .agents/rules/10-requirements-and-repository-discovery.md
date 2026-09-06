# 10 — Requirements and Repository Discovery

**Severity:** CRITICAL  
**Activation:** Model Decision

Before implementation, inspect:

- source tree and module boundaries
- package manager and scripts
- framework and versions
- routing and rendering model
- component/design-system primitives
- styling and theme conventions
- state and data-fetching layers
- API clients and generated types
- auth/session handling
- tests and test commands
- environment/configuration files
- existing instructions and local conventions

Translate the request into observable behavior: actors, entry points, user actions, data, states, validation, permissions, navigation, side effects, errors, accessibility, responsive behavior, and external dependencies.

Classify important findings as `Observed`, `Inferred`, `Assumed`, or `Missing`. Material missing decisions must be surfaced instead of silently invented.

Prefer the smallest change that completes the requested behavior without unnecessary architecture churn.
