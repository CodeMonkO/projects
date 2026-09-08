# Engineering Instructions

## Principles
Understand before modifying.
Read relevant code before making claims about implementation.
Prefer the smallest design that completely solves the requirement.
Follow existing architecture and conventions unless there is a concrete reason to change them.
Do not create abstractions for hypothetical future requirements.
Do not hardcode behavior merely to satisfy tests.
Tests verify correctness; they do not define correctness.

## Changes
Keep changes scoped to the objective.
Avoid unrelated refactoring.
When modifying an interface, inspect its consumers.
When changing persistent state or public contracts, consider backward compatibility.

## Boundaries
Validate external input and external system responses.
Trust established internal invariants unless evidence shows otherwise.

## Verification
Never claim something works merely because the implementation looks correct.
Use available tests, builds, type checks, linting, and runtime verification.

## Architecture
For significant architectural decisions:
understand requirements → identify constraints → inspect current architecture → evaluate realistic alternatives → document trade-offs → choose the simplest adequate solution.

## Autonomy
Investigate information available in the repository before asking the user.
Ask when a decision genuinely requires product/business intent that cannot be inferred safely.

## Definition of Done
Work is complete when:
- requested behavior is implemented
- relevant tests pass
- important failure paths are handled
- no known regression was introduced
- final diff has been reviewed
