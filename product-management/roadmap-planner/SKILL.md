---
name: roadmap-planner
description: >
  Quarterly roadmap planning with prioritisation frameworks. Use this skill whenever the user asks for help with
  anything related to roadmap planner. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Roadmap Planner

## Purpose

Build quarterly roadmaps with prioritised initiatives. Output: theme-based plan with rationale, trade-offs, and capacity fit. Users: PMs and team leads planning a quarter or half.

## Inputs to gather

- Time horizon: quarter, half-year, or annual
- Available initiatives or backlog items
- Team capacity in eng-weeks or headcount
- Strategic goals or OKRs for the period
- Constraints: dependencies, deadlines, tech debt budget

## Output structure

1. Strategic context - goals and themes driving the roadmap
2. Prioritised initiative list - ranked with rationale
3. Capacity allocation - initiatives mapped to capacity
4. Trade-offs - what was deprioritised and why
5. Risks and dependencies
6. Success metrics per initiative

## Quality bar

- Every initiative tied to a strategic goal or OKR
- Trade-off reasoning is explicit: why X beats Y this quarter
- Capacity is realistic - no roadmap that needs 130% of team
- Risks named with owner and mitigation

## Step-by-step instructions

1. Confirm strategic goals and available capacity
2. List candidate initiatives with rough effort estimates
3. Apply prioritisation framework: impact vs effort vs strategic alignment
4. Allocate initiatives to capacity, leaving 20% buffer
5. Write trade-off section: what was cut and the rationale
6. Identify cross-team dependencies and flag blockers
7. Define one success metric per initiative

## References

- `references/guide.md` - RICE scoring, OKR alignment, roadmap formats
