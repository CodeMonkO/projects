# Distributed Systems Patterns

## Idempotency

Use when:
- retries are possible
- duplicate events can occur
- payment/order/workflow actions must not duplicate side effects

Implementation:
- idempotency key
- request hash
- result cache
- dedupe table
- safe retry semantics

## Outbox Pattern

Use when:
- writing DB and publishing event must be reliable

Flow:
1. write business data and outbox record in same transaction
2. background publisher sends event
3. mark event as published
4. retry safely

## Saga

Use when:
- multi-step distributed transaction is needed
- each step has compensation

Types:
- orchestration-based saga
- choreography-based saga

## Circuit Breaker

Use when:
- downstream dependency can fail or become slow

States:
- closed
- open
- half-open

## Backpressure

Use when:
- producer can overload consumer

Techniques:
- queue limits
- rate limits
- load shedding
- adaptive concurrency
- priority queues

## Dead Letter Queue

Use when:
- messages repeatedly fail and need manual/automated investigation

Include:
- failure reason
- retry count
- original payload reference
- owner
- replay mechanism

## Bulkhead

Use when:
- one dependency or tenant should not take down the whole system

Techniques:
- separate thread pools
- separate queues
- tenant quotas
- isolated worker pools

## CQRS

Use when:
- read model and write model need different scaling/shape

Avoid if:
- simple CRUD is enough

## Event Sourcing

Use when:
- audit history is core business requirement
- state reconstruction is valuable

Avoid if:
- team maturity is low
- query needs are simple
- operational complexity is not justified
