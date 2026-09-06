# 220 — Code Quality

**Severity:** HIGH

- Prefer clear names and small functions/components.
- Keep types meaningful; avoid broad escape hatches such as `any` when a precise type is practical.
- Respect lint, formatting, typechecking, and compiler settings already in the repository.
- Avoid premature abstraction and speculative flexibility.
- Remove unused imports, variables, dependencies, styles, and dead components introduced or made obsolete by the change.
- Keep effects and asynchronous control flow understandable.
- Do not suppress lint/type errors without documenting a concrete reason.
- Keep the diff focused on the requested behavior.

Quality is judged by correctness and maintainability, not by line count or novelty.
