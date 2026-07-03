# Agentic AI Systems Guide

## Core Architecture

A serious agentic AI system should have:

- User / API interface
- Orchestrator or Workflow Builder
- Workflow Runner
- Agent Registry
- Tool Registry
- Policy Engine
- Context Engine
- Memory / State Store
- Harness / Validation Engine
- Human Approval Layer
- Evidence / Audit Store
- Observability and Cost Tracking

## Agent Types

Common agent types:

- Orchestrator Agent
- Planner Agent
- Research Agent
- Architect Agent
- Coding Agent
- Review Agent
- Security Agent
- Test Agent
- Release Agent
- Support Agent

Each agent needs:
- purpose
- owner
- input contract
- output contract
- tools
- limits
- validation
- risk level

## Agent Contract

```yaml
agent:
  id:
  purpose:
  owner:
  risk_level:
  allowed_workflows:
  allowed_tools:
  forbidden_tools:
  input_schema:
  output_schema:
  max_iterations:
  max_tool_calls:
  max_cost:
  validation_template:
  human_approval_required:
```

## Workflow Builder / Runner

### Builder
Creates:
- workflow plan
- stage list
- evidence contract
- agent plan
- tool plan
- validation plan
- approval plan

### Runner
Enforces:
- state
- gates
- policy
- budget
- approvals
- evidence collection
- retries
- pause/resume

## Evidence Contract

```yaml
evidence_contract:
  context:
    required_sources:
      - source:
        freshness_required:
        owner_required:
  artifacts:
    required_outputs:
      - artifact_type:
        schema:
  validation:
    required_templates:
      - template:
        min_status:
  approvals:
    required_roles:
      - role:
        condition:
  audit:
    required_fields:
      - model_version
      - prompt_version
      - agent_version
      - tool_calls
      - cost
```

## Agentic AI Risks

- hallucination
- tool misuse
- prompt injection
- data leakage
- runaway loops
- cost explosion
- wrong delegation
- weak context
- self-validation
- hidden unsafe action
- unreviewed production change

## Mitigations

- structured outputs
- policy checks outside LLM
- agent/tool registry
- deterministic workflow runner
- context freshness checks
- harness validation
- human approval
- audit trail
- cost limits
- tool call limits
