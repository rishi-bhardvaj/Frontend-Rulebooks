# 270 — Files and Media

**Severity:** HIGH when applicable

- Inspect the real upload/download contract before building file UI.
- Validate file type, size, count, and required metadata at the appropriate boundaries.
- Show progress, pending, success, failure, cancellation, and retry states where relevant.
- Do not assume a browser-visible filename or MIME type is trustworthy.
- Avoid loading unnecessarily large media into memory.
- Use the application's real storage/download mechanism rather than embedding fake URLs.
- Handle expired/private download URLs and permission failures intentionally.
- Provide meaningful previews and accessible alternative text where applicable.

Test large files, unsupported files, cancellation, failure, permission denial, and repeated upload behavior when relevant.
