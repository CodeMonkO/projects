---
name: release-check
description: Determine whether a change is safe and complete enough to release.
---

# Release Check
## Workflow
1. Review the complete release diff.
2. Check relevant build, unit/integration/E2E tests, migrations, configuration, flags, dependencies, API compatibility, observability, and deployment manifests.
3. For migrations check forward/backward compatibility, mixed versions, rollback implications, and large-data behavior.
4. Verify logs, metrics, alerts, and rollback path.
5. Separate **RELEASE BLOCKERS** from **NON-BLOCKING FOLLOW-UPS**. Do not block for cosmetic concerns.

## Output
BUILD · TESTS · MIGRATIONS · CONFIG · COMPATIBILITY · OBSERVABILITY · ROLLBACK · BLOCKERS · FOLLOW-UPS

**VERDICT: GO / NO-GO**
