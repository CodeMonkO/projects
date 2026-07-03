# System Design Review Checklist

## Problem
- Is the problem clear?
- Is the business value clear?
- Are users/stakeholders clear?
- Is success measurable?

## Scope
- What is in scope?
- What is out of scope?
- What assumptions exist?
- What decisions are still open?

## Architecture
- Are system boundaries clear?
- Are responsibilities clear?
- Is there a control plane/data plane split if needed?
- Is there any God service?
- Is the architecture understandable?

## APIs
- Are APIs well-defined?
- Are schemas versioned?
- Is backward compatibility addressed?
- Are error responses clear?
- Are timeouts/retries defined?

## Data
- What is source of truth?
- Who owns the data?
- What is read/write pattern?
- What is consistency requirement?
- Is retention defined?
- Is migration plan defined?

## Reliability
- What can fail?
- How is failure detected?
- How is failure mitigated?
- Are retries idempotent?
- Is rollback possible?
- Is there a fallback?

## Performance
- What is latency target?
- What is expected QPS?
- What is peak load?
- Where are bottlenecks?
- What is cached?

## Security
- Authentication?
- Authorization?
- Data sensitivity?
- Secrets handling?
- Audit requirements?
- Abuse/misuse cases?

## Observability
- Logs?
- Metrics?
- Traces?
- Dashboards?
- Alerts?
- Runbooks?

## Cost
- What drives cost?
- What can explode with scale?
- Are budgets/limits needed?
- What can be cached or batched?

## Delivery
- MVP?
- Rollout plan?
- Migration plan?
- Rollback plan?
- Ownership?
- Support model?
