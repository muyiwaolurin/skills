---
name: refactoring
description: >
  Plan and document safe refactoring strategies. Use this skill whenever the user asks for help with
  anything related to refactoring. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Refactoring

## Purpose

Plan and execute safe refactoring strategies. Output: step-by-step plan that keeps tests green throughout. Users: engineers improving code structure without changing behaviour.

## Inputs to gather

- Code to refactor: module, function, or system boundary
- Goal: readability, performance, testability, or reducing coupling
- Existing test coverage level
- Risk tolerance: can this block the team if it breaks

## Output structure

1. Refactoring goal - what improves and why it matters
2. Risk assessment - what could break, how to detect it
3. Prerequisites - tests to write before starting
4. Step-by-step plan - small, independently deployable moves
5. Verification checklist per step
6. Rollback plan

## Quality bar

- Each step leaves code in a working, deployable state
- No step mixes structural change with behaviour change
- Tests added before any structural move - never after
- Rollback plan exists for each step

## Step-by-step instructions

1. Confirm refactoring goal: what specifically improves
2. Assess coverage: which paths have tests, which do not
3. Write missing tests before touching structure
4. Plan moves in smallest safe increments: rename, extract, inline, move
5. Apply one move at a time - run tests after each
6. Review: does the new structure achieve the stated goal
7. Update any documentation that describes the old structure

## References

- `references/guide.md` - refactoring patterns, safe move catalogue
