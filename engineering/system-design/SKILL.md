---
name: system-design
description: >
  Produce architecture docs and trade-off analyses. Use this skill whenever the user asks for help with
  anything related to system design. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# System Design

## Purpose

Design scalable systems and produce architecture docs with trade-off analyses. Output: diagrams, component breakdown, decision rationale. Users: engineers, tech leads, architects.

## Inputs to gather

- Problem to solve: scale, domain, constraints
- Non-functional requirements: latency, availability, consistency targets
- Traffic estimates: requests/sec, data volume, growth rate
- Existing systems to integrate with or migrate from

## Output structure

1. Problem restatement - clarify scope and constraints
2. High-level architecture - components and interactions
3. Data model - key entities, storage choices, schema sketch
4. API contract - main endpoints or message schemas
5. Trade-off analysis - options considered and why this was chosen
6. Failure modes and mitigations
7. Open questions and future considerations

## Quality bar

- Every component choice has a stated reason
- Trade-offs are explicit: not "X is better" but "X trades Y for Z"
- Scale numbers are used to justify choices, not decorate them
- Failure modes addressed: what breaks and what the fallback is

## Step-by-step instructions

1. Confirm scope: what is in and out of the design
2. Gather scale numbers - estimate if not given
3. Identify the hardest constraint: throughput, consistency, latency
4. Sketch high-level components and data flow
5. Choose storage: type, schema, access patterns
6. Design APIs or message contracts
7. Enumerate failure modes: network partitions, node failures, bad inputs
8. Write trade-off section: what alternatives were rejected and why

## References

- `references/guide.md` - CAP theorem, common patterns, capacity estimation
