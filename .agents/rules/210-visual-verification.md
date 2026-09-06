# 210 — Visual and Browser Verification

**Severity:** CRITICAL for UI changes

When the environment permits browser execution, verify the actual rendered application rather than relying only on source inspection.

Check the requested flow at representative viewport sizes and inspect:

- initial render and hydration/runtime errors
- navigation and direct URLs
- loading, empty, success, and error states
- forms and keyboard interaction
- API/network requests and response handling
- authenticated and denied states where relevant
- images/fonts/assets loading
- responsive layout
- focus and accessible names
- dialogs/menus/overlays
- console errors and unexpected warnings relevant to the change

For visual work, compare against supplied references and surrounding product screens. Do not use a screenshot as proof of backend correctness or accessibility compliance.

Record what was actually exercised and what could not be tested.
