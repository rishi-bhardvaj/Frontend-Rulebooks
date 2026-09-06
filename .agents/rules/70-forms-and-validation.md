# 70 — Forms and Validation

**Severity:** CRITICAL

Forms must behave correctly, not merely look complete.

- Give every input an accessible name, label, and useful description where needed.
- Client validation improves feedback but does not replace server validation.
- Match the real API's constraints and field-level error contract.
- Preserve entered values when submission fails unless clearing is intentional.
- Prevent accidental duplicate submission.
- Provide pending, success, validation-error, permission-error, and unexpected-error states as applicable.
- Make errors discoverable without relying on color alone.
- Handle files, dates, numbers, enums, nullable values, and locale-specific input carefully.

Test valid, invalid, boundary, empty, duplicate, interrupted, permission-denied, and server-rejected submissions where relevant.
