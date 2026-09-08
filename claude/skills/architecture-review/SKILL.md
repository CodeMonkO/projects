---
name: architecture-review
description: Evaluate system or feature architecture and produce evidence-based architectural recommendations.
---

# Architecture Review
## Objective
Determine whether the architecture is the simplest robust design for the actual requirements. Do not redesign merely because another design is possible.

## Workflow
1. Identify business objective, functional requirements, quality attributes, constraints, expected scale, and ownership boundaries.
2. Inspect current architecture and map components, dependencies, data/control flow, trust boundaries, state ownership, and external systems.
3. Evaluate relevant dimensions: coupling, cohesion, scalability, availability, failure isolation, consistency, security, observability, operability, cost, and maintainability.
4. Analyze realistic failures: timeout, retry, duplicate, partial execution, concurrency, backpressure, stale state, partition, dependency outage.
5. Compare only meaningful alternatives, including benefits, cost, complexity, and risks.
6. Recommend one approach, explain why, and identify assumptions that could invalidate it.
7. Separate **NEEDED NOW** from **POSSIBLE LATER**.

## Output
CONTEXT · CURRENT STATE · REQUIREMENTS · KEY RISKS · OPTIONS · RECOMMENDATION · TRADE-OFFS · FAILURE MODES · EVOLUTION PATH · DECISIONS REQUIRED
