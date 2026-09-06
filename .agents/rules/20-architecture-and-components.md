# 20 — Architecture and Components

**Severity:** HIGH  
**Activation:** Model Decision

- Preserve the repository's existing architectural boundaries.
- Keep page/route orchestration separate from reusable UI primitives and domain behavior where the stack supports it.
- Components should have a clear responsibility and predictable inputs/outputs.
- Prefer composition over giant conditional components.
- Do not introduce a state-management library, UI framework, design system, or abstraction layer without evidence that it solves a real problem.
- Reuse existing primitives before creating visually or behaviorally duplicate components.
- Keep browser-only behavior out of server-rendered boundaries where the framework requires it.
- Respect the installed framework/version rather than relying on patterns from a different major version.
- Delete obsolete code when replacement is complete; do not leave parallel implementations without a reason.

For substantial changes, record the affected routes, components, state ownership, data dependencies, and verification plan before editing.
