# 80 — Error and System States

**Severity:** HIGH

Every meaningful async or data-driven screen should consider the states that users can actually encounter:

- initial/loading
- partial loading where applicable
- success
- empty/no results
- validation failure
- authentication required
- permission denied
- network failure
- server failure
- stale/offline state where relevant
- retry/recovery

Do not use an indefinite spinner as a substitute for error handling. Do not show fake records to hide an unavailable API. Error messages should explain what happened at an appropriate level and provide a safe next action when one exists.

Verify state transitions with real or explicitly controlled test conditions.
