---
name: security-review
description: Review code or architecture for exploitable security weaknesses and unsafe trust assumptions.
---

# Security Review
## Objective
Find credible security risks and recommend proportionate mitigations.

## Workflow
1. Establish users, services, external systems, privileged components, stores, and trust boundaries.
2. Review relevant authentication, authorization, tenant isolation, input validation, injection, secrets, sensitive data, logging, file/network access, deserialization, dependencies, and destructive operations.
3. Never treat authentication as authorization; verify permission for the specific resource/action.
4. Treat external input as untrusted and validate at system boundaries.
5. For destructive actions inspect safeguards, recoverability, bulk behavior, and privilege.
6. Report credible issues only.

## Finding Format
SEVERITY · ATTACK/FAILURE SCENARIO · AFFECTED COMPONENT · EVIDENCE · MITIGATION

Finish with: **SECURITY VERDICT**
