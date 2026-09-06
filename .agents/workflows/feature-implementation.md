# Frontend Feature Implementation Workflow

Use for substantial UI or product-flow changes.

## 1. Discover

Inspect the repository, framework/version, routes, design system, state/data layers, API clients, auth, tests, environment conventions, and local instructions.

## 2. Map the flow

Write:

`user action → route/screen → component → state → client request/event → backend/external boundary → response → UI state`

List loading, empty, error, permission, responsive, accessibility, and side-effect behavior.

## 3. Plan

Choose the smallest complete implementation. Identify material assumptions and missing contracts. Identify configuration values required.

## 4. Implement

Reuse established components and patterns. Implement real data boundaries. Keep production paths free of temporary mocks and placeholders.

## 5. Configure

For every OAuth/provider/API/integration requirement, use `.agents/rules/195-secrets-and-integration-configuration.md` and prepare an exact configuration handoff.

## 6. Verify

Build/typecheck/lint. Start the application when appropriate. Exercise the real browser flow. Inspect network requests, API responses, state transitions, console/runtime errors, and persistence/side effects. Run relevant automated tests.

## 7. Diagnose

If something fails, reproduce it, identify the failing boundary, fix the root cause, and retest. Do not hide failures with fallback mocks.

## 8. Audit

Check for placeholders, fake data, unsafe secrets, accessibility regressions, responsive failures, dead code, unnecessary dependencies, and unrelated changes.

## 9. Report

State exact changes, commands run, evidence, configuration required, unresolved issues, assumptions, and one of `IMPLEMENTED`, `VERIFIED`, `NOT VERIFIED`, or `BLOCKED`.
