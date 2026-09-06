# Frontend Rulebooks

A portable operating system for AI coding agents working on frontend applications.

The goal is not to make an agent produce a convincing screen. The goal is to make it behave like a frontend engineer: inspect the existing system, understand product intent, preserve established conventions, implement real behavior, integrate with real boundaries, test meaningful states, verify user flows, diagnose failures, and report evidence.

## Core lifecycle

Understand → Inspect → Plan → Implement → Build → Run → Exercise real UI flows → Test → Verify → Diagnose → Fix → Retest → Audit → Report

## Design principle

The rulebook is deliberately stack-agnostic. It adapts to the repository's actual framework, router, rendering model, state management, styling system, package manager, test stack, and deployment model instead of imposing a preferred stack.

## Configuration principle

Whenever a feature requires OAuth credentials, AI API keys, analytics IDs, maps keys, payment configuration, backend URLs, storage configuration, or any other external configuration, the agent MUST inspect the repository's conventions and tell the developer the exact file/path, variable or config key, environment, client/server exposure, source of the value, and verification steps. It must never invent a path or ask the developer to paste secrets into source code or chat.

## Human-made UI principle

The agent must not produce generic AI-looking interfaces merely because they are easy to generate. It must derive the visual language from the product, existing design system, content, domain, and supplied references. Avoid arbitrary gradients, excessive rounded cards, decorative blobs, gratuitous glassmorphism, meaningless animations, fake metrics, generic copy, and template-like layouts unless the product actually calls for them.

## What this repository contains

- `AGENTS.md` — portable entry point for coding agents.
- `.agents/rules/` — modular rules, ordered by concern.
- `.agents/workflows/` — repeatable implementation and verification workflows.
- `.agents/checklists/` — concise completion and review checklists.
- `.agents/templates/` — reusable task, contract, and configuration reports.
- `.agents/examples/` — examples of evidence-based frontend work.

## Rule precedence

1. Security, privacy, accessibility, and data-integrity requirements.
2. Explicit user/product requirements.
3. Existing repository architecture and established conventions.
4. Framework and platform documentation matching the installed versions.
5. Applicable rules in this repository.
6. Agent preference.

Existing patterns do not justify preserving a known correctness, security, accessibility, or usability defect.
