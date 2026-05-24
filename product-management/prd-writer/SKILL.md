---
name: prd-writer
description: >
  Write structured Product Requirement Documents. Use this skill whenever the user asks for help with
  anything related to prd writer. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# PRD Writer

## Purpose

Write structured Product Requirement Documents. Output: a clear, complete spec engineers and designers can build from without constant clarification. Users: PMs defining new features or projects.

## Inputs to gather

- Problem statement: what user pain or opportunity this addresses
- Target users and their context
- Success metrics: how you will know this worked
- Scope boundaries: what is in and explicitly out
- Known constraints: tech, timeline, compliance

## Output structure

1. Problem statement - user pain, business opportunity, evidence
2. Goals and success metrics - measurable outcomes
3. User personas and scenarios - who uses this and how
4. Requirements - functional (must-haves) and non-functional (performance, security)
5. Out of scope - explicit exclusions
6. Open questions - unresolved decisions with owners
7. Dependencies and risks

## Quality bar

- Every requirement is testable: "system must do X when Y"
- Success metrics are measurable and have a target value
- Out of scope section prevents scope creep in review
- No solution prescribing in requirements - what, not how

## Step-by-step instructions

1. Confirm problem statement and evidence (user research, data)
2. Define success metrics with baseline and target
3. Write 2-3 user scenarios showing the feature in context
4. List functional requirements - must, should, could
5. List non-functional requirements: latency, scale, security
6. Write explicit out-of-scope section
7. Capture open questions with owner and deadline

## References

- `references/guide.md` - PRD templates, requirement writing patterns
