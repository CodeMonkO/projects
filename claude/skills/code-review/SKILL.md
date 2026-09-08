---
name: code-review
description: Review code changes for correctness, regressions, architecture, security, performance, and maintainability.
---

# Code Review
## Objective
Find meaningful production-impacting problems, not stylistic noise.

## Workflow
1. Understand the intent and relevant requirements.
2. Review every changed file and the surrounding implementation.
3. Trace affected callers, consumers, interfaces, state and data flows.
4. Evaluate correctness, boundaries, error handling, concurrency, data integrity, compatibility, security, performance, observability, and tests where relevant.
5. Verify tests cover behavior rather than merely implementation details.
6. Classify credible findings as BLOCKER, HIGH, MEDIUM, or LOW. Do not inflate severity.

## Finding Format
SEVERITY · LOCATION · PROBLEM · FAILURE SCENARIO · RECOMMENDED FIX

Finish with: **REVIEW VERDICT: APPROVE / CHANGES REQUIRED**
