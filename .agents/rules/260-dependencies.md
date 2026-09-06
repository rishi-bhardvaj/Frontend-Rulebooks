# 260 — Dependencies and Bundles

**Severity:** HIGH

Before adding a dependency, inspect whether the repository already provides the capability.

For a new package, consider maintenance, bundle/runtime cost, browser support, licensing, security history, tree-shaking, and whether the feature justifies the dependency.

- Do not add large libraries for trivial helpers.
- Do not duplicate existing utilities or design-system components.
- Keep versions compatible with the installed framework/runtime.
- Remove obsolete dependencies after migrations.
- Do not use a dependency merely because an AI agent knows it well.
- Measure meaningful bundle/performance impact when it matters.

Prefer the simplest solution that fits the existing system.
