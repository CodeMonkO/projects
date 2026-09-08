---
name: qa-e2e
description: Validate functionality end-to-end from requirements through real user journeys and system boundaries.
---

# End-to-End QA
## Objective
Determine whether functionality actually works as intended and is safe to progress toward production. Passing unit tests alone is insufficient.

## Workflow
1. Extract explicit acceptance criteria and identify ambiguity.
2. Identify real user journeys and test through public boundaries when practical.
3. Validate the happy path end-to-end.
4. Test relevant boundaries: empty/invalid values, limits, duplicates, concurrency, and state transitions.
5. Test realistic failures: network/dependency failure, timeout, partial completion, invalid external response, restart/retry.
6. Where relevant verify persistence: write, read, update, restart, retry, duplicate handling.
7. Verify affected component contracts without mocking away the behavior under test.
8. Validate relevant auth, authorization, tenant isolation, input validation, and sensitive data handling.
9. Run relevant regression suites and inspect neighboring functionality.
10. Base conclusions on observed behavior, code inspection, or test evidence.

## Output
TEST SCOPE · TESTS EXECUTED · PASSED · FAILED · DEFECTS · REGRESSION RISK · UNTESTED AREAS · RELEASE CONFIDENCE · GO / NO-GO
