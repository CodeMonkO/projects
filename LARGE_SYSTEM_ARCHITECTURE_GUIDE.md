# Large System Architecture Guide

## 1. Start With the Problem

Before designing, write:

- What problem are we solving?
- Who has the problem?
- Why does it matter now?
- What happens if we do nothing?
- What is the success measure?

## 2. Define Scope

### In scope
What this system must own.

### Out of scope
What this system should not own.

### Open questions
What must be clarified before implementation.

## 3. Define System Boundaries

For each major component:

```yaml
component:
  name:
  owns:
  does_not_own:
  inputs:
  outputs:
  dependencies:
  data_owned:
  operational_owner:
  failure_behavior:
```

## 4. Choose Architecture Style

Common choices:

| Style | Use when | Avoid when |
|---|---|---|
| Modular monolith | team is small, domain still evolving | scaling or ownership boundaries are clear |
| Microservices | independent ownership and scaling are needed | boundaries are unclear |
| Event-driven | async decoupling and high throughput needed | strong consistency and simple flow needed |
| Workflow orchestration | long-running, multi-step process needed | simple request-response is enough |
| Data pipeline | batch/stream transformation needed | direct API is simpler |
| Agentic workflow | reasoning/planning needed | deterministic logic is enough |

## 5. Design Data Flow

For each data flow:

- source
- destination
- sync or async
- data schema
- owner
- retry behavior
- idempotency key
- failure behavior
- observability

## 6. Design for Failure

List:

| Failure | Impact | Detection | Mitigation | Owner |
|---|---|---|---|---|

Examples:
- API timeout
- duplicate event
- partial write
- DB migration failure
- queue backlog
- model provider outage
- wrong agent output
- permission denial
- bad deployment

## 7. Define NFRs

- latency
- throughput
- availability
- durability
- consistency
- data retention
- security
- privacy
- compliance
- cost
- observability
- operability

## 8. Define MVP

MVP should include:
- narrow use case
- one or two workflows
- minimal integration
- manual approval where needed
- clear success metric
- no unnecessary platform build

## 9. Define North Star

North Star should include:
- mature component model
- ownership model
- scale model
- governance model
- migration path
- extension points

## 10. Decision Log

Every major decision should have:
- context
- decision
- options considered
- tradeoffs
- risks
- owner
- review date
