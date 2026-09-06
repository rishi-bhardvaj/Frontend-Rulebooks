# Human-Made UI

**Severity: CRITICAL for material visual work**  
**Activation:** Always On for UI implementation; apply `.agents/rules/135-visual-inspiration-and-reference-analysis.md` and `.agents/rules/300-design-reference-research.md` for substantial visual work.

The objective is an interface that feels intentionally designed for its product and audience, not an interchangeable AI-generated template.

## Before styling

Inspect the existing brand and design system, typography and spacing conventions, reusable components, imagery and asset treatment, product/domain vocabulary, information architecture, supplied design/reference material, and existing responsive/accessibility behavior.

For a greenfield visual direction, research multiple external references. Use Awwwards, Brandfetch, Godly/Recent, SiteInspire, CSS Design Awards, Mobbin, Page Flows, Behance, Dribbble, Land-book, Lapa Ninja, One Page Love, The FWA, or another appropriate source according to the design problem. Study decisions; do not imitate a particular site.

## Required design behavior

- Establish hierarchy before decoration.
- Use typography intentionally; do not default to fashionable pairings without a reason.
- Use a coherent spacing rhythm and grid.
- Use color to communicate hierarchy, state, brand, or emphasis.
- Prefer real product content and realistic data.
- Make interaction states explicit: hover, focus, pressed, disabled, loading, success, and error where relevant.
- Design for the smallest supported viewport before polishing wider layouts.
- Preserve semantic HTML and accessibility while pursuing visual quality.
- Respect `prefers-reduced-motion` and avoid motion that competes with comprehension.

## Avoid AI-template failure modes

Do not introduce these merely because they make generated screenshots look polished:

- arbitrary purple/blue gradients
- glassmorphism everywhere
- oversized rounded containers
- floating abstract blobs
- random 3D illustrations
- repeated bento/card grids
- fake statistics, testimonials, customer logos, or social proof
- generic startup/AI marketing copy
- excessive pill-shaped controls
- animation without interaction or storytelling value
- shadows on every surface

None of these are categorically forbidden. A product may legitimately use them. The agent must be able to explain the product/design reason.

## Reference discipline

Awwwards can inform craft and interaction ambition; Brandfetch can inform brand-system and asset context; product UI libraries can inform proven interaction patterns. Award-winning or fashionable work is not automatically appropriate for every product.

Do not clone source code, copy protected imagery/illustration, reproduce distinctive branded layouts one-for-one, or reuse site copy. Translate useful principles into a product-specific system.

## Quality bar

A reviewer should be able to answer:

1. Why does this hierarchy exist?
2. Why this type scale?
3. Why these colors?
4. Why this interaction or motion?
5. Why this density/spacing?
6. What product problem does the visual treatment solve?
7. Does it still work with real content, keyboard navigation, narrow screens, and failure states?

If the answers are mostly “because it looks modern,” the design is not finished.
