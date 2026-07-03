# Security Architecture Guide

## Core Security Questions

- Who is the user?
- What are they allowed to do?
- What data can they access?
- What actions need approval?
- What is audited?
- What happens on misuse?
- How are secrets protected?
- How is least privilege enforced?

## Agentic AI Security

Check:
- prompt injection
- indirect prompt injection
- data leakage
- tool misuse
- over-permissioned agents
- secrets exposure
- untrusted tool output
- backdoor generation
- auth bypass
- hidden network calls
- suspicious dependencies

## Tool Security

Every tool should have:
- owner
- risk class
- read/write/destructive classification
- allowed agents
- required approvals
- audit requirements
- rate limits
- input validation
- output sanitization

## Human Approval Required For

- production release
- DB migration
- auth/authz change
- security exception
- destructive action
- customer-impacting action
- sensitive data export
- policy override
