# Claude Engineering Skills Pack

Ready-to-copy reusable engineering skills for Claude Code.

## Install

Copy `.claude/skills/` into the root of your repository.

If your repository does not already have a `CLAUDE.md`, you may also copy the included starter `CLAUDE.md`.
If you already have one, merge the useful general engineering rules instead of overwriting project-specific knowledge.

## Included Skills

- bug-hunt
- code-review
- feature-build
- architecture-review
- qa-e2e
- security-review
- performance-investigation
- production-incident
- release-check
- handoff

## Suggested separation

- `CLAUDE.md`: persistent engineering/project instructions
- `docs/`: architecture, decisions, system facts and constraints
- `.claude/skills/*/SKILL.md`: task-specific reusable procedures
- prompt: the concrete work to perform now

## Examples

Use the relevant skill for tasks such as:

- Bug: investigate an STT regression using `bug-hunt`.
- Feature: implement workflow cancellation using `feature-build`.
- Architecture: assess orchestrator state ownership using `architecture-review`.
- Pre-merge: use `code-review`, then `qa-e2e`.
- Deployment: use `release-check`.
- Long session: use `handoff` to preserve continuation context.

Keep project-specific Orbit/Astra, Gargi, or other domain knowledge out of these generic skills.
