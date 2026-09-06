# Frontend Rulebooks

A portable operating system for AI coding agents working on frontend applications.

The goal is not to make an agent produce a convincing screen. The goal is to make it behave like a frontend engineer: inspect the existing system, understand product intent, preserve established conventions, implement real behavior, integrate with real boundaries, test meaningful states, verify user flows, diagnose failures, and report evidence.

## Core lifecycle

Understand → Inspect → Plan → Implement → Build → Run → Exercise real UI flows → Test → Verify → Diagnose → Fix → Retest → Audit → Report

## Design principle

The rulebook is stack-agnostic. It adapts to the repository's actual framework, router, rendering model, state management, styling system, package manager, test stack, and deployment model instead of imposing a preferred stack.

## Configuration principle

Whenever a feature requires OAuth credentials, AI API keys, analytics IDs, maps keys, payment configuration, backend URLs, storage configuration, or any other external configuration, the agent MUST inspect the repository's conventions and tell the developer the exact file/path, variable or config key, environment, client/server exposure, source of the value, and verification steps. It must never invent a path or ask the developer to paste secrets into source code or chat.

See `.agents/rules/195-secrets-and-integration-configuration.md` and `.agents/templates/integration-configuration-report.md`.

## Human-made UI principle

The agent must not produce generic AI-looking interfaces merely because they are easy to generate. It must derive the visual language from the product, existing design system, content, domain, and supplied references. Avoid arbitrary gradients, excessive rounded cards, decorative blobs, gratuitous glassmorphism, meaningless animations, fake metrics, generic copy, and template-like layouts unless the product actually calls for them.

See `.agents/rules/130-human-made-ui.md` and `.agents/checklists/ui-quality.md`.

## Rule index

| Area | Rule |
| --- | --- |
| Operating contract | `.agents/rules/00-operating-contract.md` |
| Repository/requirements | `.agents/rules/10-requirements-and-repository-discovery.md` |
| Architecture/components | `.agents/rules/20-architecture-and-components.md` |
| Frontend/backend contract | `.agents/rules/25-frontend-contract-discovery.md` |
| API/data fetching | `.agents/rules/30-api-data-fetching.md` |
| Authentication | `.agents/rules/40-authentication-and-sessions.md` |
| Authorization | `.agents/rules/50-authorization-and-permissions.md` |
| State/URL | `.agents/rules/60-state-and-url.md` |
| Forms | `.agents/rules/70-forms-and-validation.md` |
| System states | `.agents/rules/80-error-and-system-states.md` |
| Security/privacy | `.agents/rules/90-security-and-privacy.md` |
| Testing | `.agents/rules/100-testing.md` |
| Test data | `.agents/rules/110-test-data-and-fixtures.md` |
| Accessibility | `.agents/rules/120-accessibility.md` |
| Human-made UI | `.agents/rules/130-human-made-ui.md` |
| Design system | `.agents/rules/140-design-system.md` |
| Responsive | `.agents/rules/150-responsive.md` |
| Routing | `.agents/rules/160-navigation-and-routing.md` |
| Performance | `.agents/rules/170-performance.md` |
| Integrations | `.agents/rules/180-third-party-integrations.md` |
| Exact configuration | `.agents/rules/195-secrets-and-integration-configuration.md` |
| Mock detection | `.agents/rules/200-mock-detection.md` |
| Browser verification | `.agents/rules/210-visual-verification.md` |
| Code quality | `.agents/rules/220-code-quality.md` |
| i18n/content | `.agents/rules/230-i18n-and-content.md` |
| SEO/metadata | `.agents/rules/240-seo-and-metadata.md` |
| Observability | `.agents/rules/250-observability.md` |
| Dependencies | `.agents/rules/260-dependencies.md` |
| Files/media | `.agents/rules/270-files-and-media.md` |
| Realtime | `.agents/rules/280-realtime-and-background-ui.md` |
| Configuration audit | `.agents/rules/290-configuration-audit.md` |

## Workflows, checklists, and templates

Use `.agents/workflows/feature-implementation.md` for substantial frontend features and `.agents/workflows/frontend-backend-integration.md` for full-stack flows.

Use `.agents/checklists/definition-of-done.md`, `.agents/checklists/accessibility.md`, `.agents/checklists/ui-quality.md`, and `.agents/checklists/testing.md` during review.

Use `.agents/templates/frontend-backend-contract.md` and `.agents/templates/integration-configuration-report.md` for repeatable evidence/configuration handoffs.

## Rule precedence

1. Security, privacy, accessibility, and data-integrity requirements.
2. Explicit user/product requirements.
3. Existing repository architecture and established conventions.
4. Framework and platform documentation matching the installed versions.
5. Applicable rules in this repository.
6. Agent preference.

Existing patterns do not justify preserving a known correctness, security, accessibility, or usability defect.

## Research basis

The rulebook was informed by several public frontend/AI-agent rule collections, including `romanveselovski/agents-frontend-rules`, `h4ckney/frontend-agent-playbook`, `yanhongwang1017/frontend-ai-coding-rules`, and `fribble186/fullstack-cursor-rules`. Their useful patterns were adapted into a verification-first, stack-agnostic system rather than copied as a generic rules dump. See `docs/research-and-influences.md`.

## Status

This is a portable rulebook intended to be copied or referenced from working frontend repositories. Framework-specific official documentation and the target repository remain authoritative for version-specific implementation details.
