# Research and Influences

This rulebook was shaped by reviewing several public frontend/AI-agent rule collections and current design-inspiration sources. Their useful ideas are adapted rather than copied wholesale.

## Reviewed agent/frontend repositories

### romanveselovski/agents-frontend-rules

Useful ideas: a drop-in `AGENTS.md` plus modular rules/skills; stack-agnostic guidance; components, forms, system states, accessibility, responsive behavior, performance, security/privacy, and avoiding generic AI-generated UI.

### h4ckney/frontend-agent-playbook

Useful ideas: evidence-driven judgment, repository/framework inspection before adopting guidance, explicit ownership after AI generation, risk-based rule routing, version-aware adapters, and separating diagnosis/verification from code generation.

### yanhongwang1017/frontend-ai-coding-rules

Useful ideas: portable `AGENTS.md`, scenario-specific skills, API integration contract checks, use of real response contracts, scope control, and avoiding unnecessary framework mixing.

### fribble186/fullstack-cursor-rules

Useful idea: separate common quality rules from task-specific workflows.

## Design inspiration sources

### Awwwards

Use for high-craft websites, composition, art direction, interaction, motion, and ambitious web execution. Do not treat award-winning work as automatic proof of usability or product fit.

### Brandfetch

Use for brand identity research: logos, colors, assets, brand presentation, and brand-system context. Do not copy protected assets or assume another company's identity belongs in the product.

### Godly / Recent

Use for contemporary composition, typography, restrained art direction, and modern landing/product surfaces.

### SiteInspire

Use for broad layout, hierarchy, grid, typography, and content-presentation research.

### CSS Design Awards

Use for frontend craft and interaction references.

### Mobbin / Page Flows

Use for real-world application screens and user-flow patterns such as onboarding, navigation, forms, authentication, search, tables, and settings.

### Behance / Dribbble

Use for visual exploration, case studies, art direction, and component concepts. Treat concepts as inspiration rather than production truth.

### Land-book / Lapa Ninja / One Page Love

Use for landing-page structures, CTA hierarchy, content density, and section composition.

### The FWA

Use for experimental interaction and motion when the product genuinely benefits from storytelling or rich interaction.

## Research rule

Use multiple source types for substantial visual work. A strong default is one high-craft gallery, one broader layout source, and one real product or brand source matched to the task. Study several references and extract principles; never ask the agent to make the product look like one particular site.

The agent must record observed principles separately from inference, state what was adapted, state what was deliberately not copied, and verify the result with real content, responsive behavior, accessibility, performance, and functional states.

## How this rulebook differs

This repository combines those ideas with the verification-first operating model used by the companion Backend-Rulebooks repository. The frontend agent traces real UI behavior through data/API boundaries, exercises the application, diagnoses failures, and reports evidence.

It also requires exact integration configuration handoff: every required key, URL, credential, or provider setting must be reported with the exact repository/deployment path and variable/config name after inspecting the actual project.

## Standards and platform references

For applicable work, agents should consult current official documentation for the installed framework and platform. Accessibility work should use WCAG/WAI-ARIA guidance; performance work should use browser/framework performance guidance; security work should use OWASP and browser security guidance. Version-specific official documentation takes precedence over generic advice in this repository.
