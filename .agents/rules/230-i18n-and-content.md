# 230 — Internationalization and Content

**Severity:** MEDIUM / HIGH when localization is required

- Inspect existing locale and message infrastructure before adding text.
- Preserve the application's locale ownership and routing model.
- Do not build layouts that assume English-length strings.
- Format dates, numbers, currencies, and times using the established locale utilities.
- Respect right-to-left layout when supported.
- Keep user-facing copy specific to the product and action.
- Do not ship placeholder or developer-facing text in user flows.
- Avoid machine-like filler, vague marketing language, and repetitive generated copy.

Test representative long strings and relevant locales when the feature is localized.
