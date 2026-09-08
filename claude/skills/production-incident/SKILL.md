---
name: production-incident
description: Investigate and mitigate active production incidents while prioritizing service restoration and evidence preservation.
---

# Production Incident
## Priority
1. Protect users/data
2. Stabilize service
3. Preserve evidence
4. Determine root cause
5. Prevent recurrence

## Workflow
1. Determine impact, scope, start time, affected users/services, data-integrity risk, and trajectory.
2. Stabilize using the lowest-risk mitigation: rollback, disable feature, reduce traffic, isolate dependency, or restore known-good config as appropriate.
3. Avoid risky architectural changes during the incident.
4. Build a timeline correlating deployments, config/traffic/dependency changes, metrics, and logs.
5. Separate trigger, root cause, contributing factors, and blast-radius amplifiers.
6. Verify recovery and data integrity.
7. Separate follow-ups into immediate, short-term, and structural actions.

## Output
IMPACT · TIMELINE · MITIGATION · ROOT CAUSE · CONTRIBUTING FACTORS · RECOVERY STATUS · FOLLOW-UP ACTIONS
