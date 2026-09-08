---
name: performance-investigation
description: Diagnose latency, throughput, CPU, memory, GC, queueing, and scalability problems using measurements rather than guesses.
---

# Performance Investigation
## Rule
**MEASURE BEFORE OPTIMIZING.**

## Workflow
1. Define the measurable symptom and establish a baseline.
2. Inspect relevant metrics, profiles, heap/GC data, logs, traces, queue and database statistics.
3. Model input rate, processing rate, concurrency, buffering, memory ownership, I/O, and downstream capacity.
4. Find the bottleneck and distinguish symptom from cause. Example: OOM does not automatically imply a GC problem.
5. For each credible hypothesis define its prediction, required evidence, and experiment. Test highest-value hypotheses first.
6. Fix the bottleneck rather than masking it. Avoid arbitrary heap/thread/timeout/batch/retry tuning without evidence.
7. Compare before vs after and estimate remaining capacity limits.

## Output
SYMPTOM · BASELINE · EVIDENCE · ROOT CAUSE · FIX · BEFORE/AFTER · CAPACITY LIMIT · REMAINING RISKS
