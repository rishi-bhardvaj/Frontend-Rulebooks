# 120 — Accessibility

**Severity:** CRITICAL

Target the accessibility level required by the product and applicable standards; default to WCAG 2.2 AA principles for general web work.

- Prefer semantic HTML before ARIA.
- Every interactive control needs an accessible name and keyboard operation.
- Preserve visible, usable focus states.
- Maintain logical focus order and meaningful landmarks/headings.
- Associate form labels, descriptions, and errors programmatically.
- Do not use color as the only indicator of meaning.
- Respect reduced-motion preferences for nonessential animation.
- Dialogs must manage focus and dismissal correctly.
- Images need appropriate alternative text; decorative images should not create noise.
- Check zoom/reflow and touch interaction where relevant.

Test with keyboard navigation and an accessibility checker when available. Do not claim accessibility compliance from visual inspection alone.
