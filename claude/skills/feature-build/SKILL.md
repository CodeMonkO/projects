---
name: feature-build
description: Implement a feature end-to-end while respecting existing architecture and minimizing unnecessary complexity.
---

# Feature Build
## Objective
Deliver the requested capability completely using the smallest appropriate design.

## Workflow
1. **Understand objective** — outcome, acceptance criteria, constraints, and out-of-scope behavior.
2. **Discover existing system** — inspect relevant modules, patterns, interfaces, tests, config, and architecture docs before designing.
3. **Determine impact** — identify only affected UI/API, domain, storage, events, external systems, security, observability, and tests.
4. **Design** — choose the simplest design satisfying current requirements. Prefer established patterns; avoid hypothetical future architecture.
5. **Implement** — work incrementally and keep changes cohesive.
6. **Test** — happy path, important boundaries, failures, and integration behavior.
7. **Verify** — run relevant tests/build/lint/type checks and review the final diff.
8. **Acceptance check** — map implementation to every acceptance criterion.

## Output
IMPLEMENTATION SUMMARY · DESIGN DECISIONS · FILES CHANGED · TESTS · ACCEPTANCE CRITERIA · KNOWN LIMITATIONS
