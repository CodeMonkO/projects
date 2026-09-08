---
name: bug-hunt
description: Systematically investigate and fix bugs, regressions, crashes, incorrect behavior, and failing tests.
---

# Bug Hunt
## Objective
Find the actual root cause and implement the smallest safe fix. Never start by changing code.

## Workflow
1. **Understand** — establish expected vs actual behavior, reproduction steps, environment, and whether it is a regression.
2. **Reproduce** — reproduce whenever possible and capture errors, logs, traces, failing tests, or incorrect state.
3. **Investigate** — read relevant implementation and trace symptom → entry point → execution path → failing component → triggering condition → root cause. Do not speculate about uninspected code.
4. **Check history** — when useful inspect git diff, recent commits, dependencies, config, and migrations.
5. **Fix** — make the smallest root-cause fix. Avoid unrelated refactoring, speculative abstractions, exception suppression, weakened tests, and hardcoded workarounds.
6. **Verify** — rerun the reproduction, relevant unit/integration tests, build, typecheck, and lint as appropriate.
7. **Regression analysis** — check neighboring behavior and boundaries.

## Output
ROOT CAUSE · EVIDENCE · FIX · FILES CHANGED · VERIFICATION · REGRESSION RISK · REMAINING CONCERNS
