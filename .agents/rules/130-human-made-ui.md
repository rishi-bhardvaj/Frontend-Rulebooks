# 130 — Human-Made UI

**Severity:** CRITICAL

The interface must look and behave like a deliberate product design, regardless of which AI coding agent generated it.

## Design before decoration

- Identify the product's visual thesis, audience, domain, content hierarchy, and existing design language before inventing new UI.
- Reuse existing tokens, typography, spacing, components, icons, and interaction patterns.
- If references/designs exist, reproduce their intent rather than substituting a generic dashboard template.
- If no design exists, make restrained decisions grounded in the product's domain and content.

## Avoid default AI aesthetics

Do not add these merely because they are common in generated UI:

- purple/blue gradient hero backgrounds
- gratuitous glassmorphism
- excessive rounded cards
- decorative blobs or floating shapes
- repeated card grids for unrelated information
- giant marketing headings with vague claims
- fake statistics or invented testimonials
- unnecessary badges and pills
- excessive shadows
- decorative animation without interaction purpose
- generic copy such as “Unlock the future” or “Revolutionize your workflow”

These patterns are not forbidden when the product genuinely calls for them. The rule is: **justify visual decisions by product intent, not by generation convenience.**

## Content and polish

Use real product terminology and realistic content. Account for long names, empty states, localization, errors, loading, and awkward data. Avoid placeholder copy surviving into production.

Before finishing, inspect the complete screen at realistic viewport sizes and compare it with the surrounding product. The result should look like it belongs in the same product, not like a newly generated template.
