# 170 — Performance

**Severity:** HIGH

Performance work must be evidence-driven.

- Measure before optimizing when a claim about performance is material.
- Avoid unnecessary client JavaScript and browser-only work.
- Load expensive features lazily when the user flow supports it.
- Avoid waterfalls in data fetching and rendering.
- Keep images appropriately sized and use modern loading/responsive mechanisms supported by the stack.
- Watch bundle size, third-party scripts, hydration/rendering cost, and repeated work.
- Preserve caching semantics and invalidation correctness while optimizing.
- Do not sacrifice accessibility, correctness, or maintainability for an unmeasured micro-optimization.

Use the project's existing performance tooling first. Record what was measured, what changed, and what evidence improved.
