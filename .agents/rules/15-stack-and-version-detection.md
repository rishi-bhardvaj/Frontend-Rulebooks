# 15 — Stack and Version Detection

**Severity:** CRITICAL

Never assume React, Next.js, Vue, Angular, Svelte, Astro, or any other framework from the task wording alone.

Inspect package manifests, lockfiles, source conventions, build scripts, router setup, rendering mode, compiler/transpiler configuration, and installed versions before choosing implementation patterns.

- Use official documentation matching the installed major/minor version when behavior is version-sensitive.
- Do not introduce APIs from a newer framework version without checking compatibility.
- Preserve the repository's package manager and scripts.
- If a migration is requested, separate migration work from feature work and verify each boundary.
- Do not convert server-rendered code to client-only code merely to avoid understanding the existing rendering model.

When framework behavior is uncertain, verify it from the installed source/documentation or a minimal repository-native reproduction instead of guessing.
