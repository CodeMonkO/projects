# Output Templates

## Architecture One-Pager

```markdown
# Architecture One-Pager: <System Name>

## Problem
What problem are we solving?

## Goal
What outcome do we want?

## Scope
In scope:
Out of scope:

## Proposed Architecture
Short explanation.

## Components
| Component | Responsibility | Owner |
|---|---|---|

## Key Flows
1.
2.
3.

## Risks
| Risk | Mitigation |
|---|---|

## MVP
What we build first.

## North Star
What this can become.

## Decisions Needed
-
```

## ADR Template

```markdown
# ADR: <Decision>

## Status
Proposed / Accepted / Deprecated

## Context
Why is this decision needed?

## Decision
What are we deciding?

## Options
1.
2.
3.

## Rationale
Why this option?

## Consequences
Positive:
Negative:
Risks:

## Review Date
```

## Risk Register

```markdown
# Risk Register

| Risk | Impact | Likelihood | Owner | Mitigation | Status |
|---|---|---|---|---|---|
```

## Component Contract

```yaml
component:
  name:
  purpose:
  owns:
  does_not_own:
  inputs:
  outputs:
  dependencies:
  data:
  failure_behavior:
  security:
  observability:
  owner:
```
