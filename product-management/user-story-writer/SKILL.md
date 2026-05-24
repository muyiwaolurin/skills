---
name: user-story-writer
description: >
  Generate acceptance-criteria-ready user stories. Use this skill whenever the user asks for help with
  anything related to user story writer. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# User Story Writer

## Purpose

Generate user stories with acceptance criteria ready for sprint planning. Output: stories a developer can pick up without clarification. Users: PMs and leads writing backlog items.

## Inputs to gather

- Feature or capability to write stories for
- Target user persona
- Definition of done for the team
- Edge cases or constraints already known

## Output structure

Per story:
1. Story title
2. Story format: "As a [user], I want [action] so that [outcome]"
3. Acceptance criteria - Given/When/Then or checklist format
4. Out of scope notes
5. Dependencies or blockers

## Quality bar

- Each story is independently deliverable - no implicit dependencies
- Acceptance criteria are testable: a QA engineer can write a test from them
- No story covers more than one user goal
- Edge cases captured in acceptance criteria, not left to imagination

## Step-by-step instructions

1. Identify distinct user goals in the feature request
2. Write one story per goal - split if two goals are bundled
3. Write acceptance criteria: cover happy path, error states, and edge cases
4. Add explicit out-of-scope to prevent gold-plating
5. Flag dependencies on other stories, services, or teams
6. Estimate complexity if asked: S/M/L or story points

## References

- `references/guide.md` - story splitting patterns, AC writing guide
