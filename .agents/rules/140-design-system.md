# 140 — Design System and Styling

**Severity:** HIGH

- Discover the existing design tokens and component primitives before adding styles.
- Reuse existing buttons, inputs, dialogs, tables, typography, spacing, colors, icons, and layout primitives.
- Keep variants explicit and composable.
- Avoid one-off values when an existing token represents the same intent.
- Keep responsive behavior intentional rather than patching individual breakpoints reactively.
- Preserve theme behavior and contrast.
- Keep component styling close to the repository's established styling mechanism.
- Do not introduce a second UI library for one feature without a documented reason.
- Remove obsolete styles and duplicate components after migrations.

Visual changes should be checked against neighboring screens to prevent design-system drift.
