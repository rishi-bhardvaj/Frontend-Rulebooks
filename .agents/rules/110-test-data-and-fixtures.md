# 110 — Test Data and Fixtures

**Severity:** HIGH

Use deterministic, realistic fixture data for component, integration, and E2E testing where needed.

Fixtures should reflect actual response shapes, required fields, enums, relationships, nullable values, pagination, and lifecycle states. Include useful cases such as normal data, empty data, long text, boundary values, invalid values, duplicate/conflict responses, expired sessions, permission-denied responses, network failures, and deleted/inactive records where relevant.

Do not use real credentials, API keys, private tokens, or unnecessary personal data.

Keep factories/builders/fixtures reusable and isolated from production configuration. Fixtures must not conceal broken APIs or missing integrations.
