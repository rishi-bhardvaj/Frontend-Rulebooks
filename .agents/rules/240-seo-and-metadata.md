# 240 — SEO and Metadata

**Severity:** MEDIUM / HIGH for public-facing sites

Apply SEO behavior only where the page is intended to be discoverable.

- Set accurate title and description metadata from real page content.
- Preserve canonical URLs and routing semantics.
- Do not generate structured data for content that is not actually represented on the page.
- Keep public and authenticated/internal application routes appropriately separated from indexing concerns.
- Verify redirects, not-found responses, sitemap/robots behavior, and social metadata where relevant.
- Do not make SEO changes that alter authenticated application behavior without a product requirement.

SEO claims should be checked against the rendered page and deployed routing model, not inferred from source alone.
