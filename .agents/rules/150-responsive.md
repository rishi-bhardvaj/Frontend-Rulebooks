# 150 — Responsive Design

**Severity:** HIGH

Design from the smallest supported viewport upward, then verify larger layouts.

- Identify supported viewport ranges from the product/repository.
- Avoid fixed dimensions that clip real content.
- Test navigation, forms, tables, dialogs, menus, and dense data on narrow screens.
- Account for long text, dynamic content, zoom/reflow, safe areas, and touch targets where relevant.
- Prefer layout systems that adapt naturally over breakpoint-heavy patches.
- Do not hide important functionality solely because the viewport is small unless that is an intentional product decision.
- Verify both portrait and landscape where the product requires it.

A desktop screenshot is not sufficient evidence of responsive correctness.
