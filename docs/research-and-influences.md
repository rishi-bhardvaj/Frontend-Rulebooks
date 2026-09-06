# Research and Influences

This rulebook was shaped by reviewing several public frontend/AI-agent rule collections. Their useful ideas were adapted rather than copied wholesale.

## Reviewed repositories

### romanveselovski/agents-frontend-rules

Useful ideas: a drop-in `AGENTS.md` plus modular rules/skills; stack-agnostic guidance; explicit frontend concerns such as components, forms, system states, accessibility, responsive behavior, performance, security/privacy, and avoiding generic AI-generated UI. Its README emphasizes that agents often produce visually plausible but incomplete pages, so the rules force work such as labels, themes, error states, mobile behavior, and real 404 handling.

### h4ckney/frontend-agent-playbook

Useful ideas: evidence-driven judgment, repository/framework inspection before adopting guidance, explicit ownership after AI generation, risk-based rule routing, version-aware adapters, production workflows, and separating diagnosis/verification from simple code generation.

### yanhongwang1017/frontend-ai-coding-rules

Useful ideas: a portable `AGENTS.md`, scenario-specific skills, API integration contract checks, reuse of the real response contract, scope control, and avoiding unnecessary framework mixing or over-engineering.

### fribble186/fullstack-cursor-rules

Useful idea: separate common quality rules from task-specific development workflows rather than making every instruction equally active.

## How this rulebook differs

This repository intentionally combines those ideas with the verification-first operating model used by the companion Backend-Rulebooks repository. The frontend agent is expected to trace real UI behavior through data/API boundaries, exercise the application, diagnose failures, and report evidence.

It also adds two explicit requirements:

1. **Exact integration configuration handoff:** every required key, URL, credential, or provider setting must be reported with the exact repository/deployment path and variable/config name after inspecting the actual project.
2. **Human-made UI gate:** visual output must be grounded in product intent and existing design language rather than generic AI-generated aesthetics. Common generated patterns are not banned, but they must be justified by the product.

## Standards and platform references

For applicable work, agents should consult current official documentation for the installed framework and platform. Accessibility work should use WCAG/WAI-ARIA guidance; performance work should use browser/framework performance guidance; security work should use OWASP and browser security guidance. Version-specific official documentation takes precedence over this repository's generic advice.

## Attribution

This document records conceptual influences only. No source repository is treated as authoritative for another project's architecture, stack, product requirements, or visual identity. The actual target repository remains the primary source of truth.
