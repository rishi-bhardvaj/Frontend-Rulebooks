# 290 — Configuration Audit

**Severity:** CRITICAL

Before finalizing an integration, search the implementation for configuration reads and compare them with the project's example/deployment configuration.

Check:

- every referenced environment/config key exists in the documented setup
- browser-exposed keys are intentionally public
- server-only values are not imported into client bundles
- required values have clear missing-config errors
- local/test/staging/production setup is distinguished
- redirect URLs, origins, hostnames, and provider identifiers match the environment
- documentation uses the exact variable names actually read by the code

The final report must contain exact paths and key names. Never invent a conventional path if the repository uses another convention.
