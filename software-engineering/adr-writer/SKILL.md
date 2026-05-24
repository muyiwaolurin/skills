---
name: adr-writer
description: >
  Write Architecture Decision Records with context and consequences. Use this skill whenever the user asks for help with
  anything related to adr writer. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# ADR Writer

## Purpose

Write Architecture Decision Records that document why a decision was made, not just what was decided. Output: a durable record future engineers can read to understand the codebase. Users: engineers and architects logging significant technical choices.

## Inputs to gather

- Decision to record - the choice that was made
- Context: what problem or constraint forced this decision
- Alternatives that were considered
- Consequences: what this decision makes easier or harder

## Output structure

1. Title - ADR-NNN: [short present-tense statement of decision]
2. Status - proposed, accepted, deprecated, or superseded
3. Context - forces at play that required a decision
4. Decision - what was decided and who decided it
5. Consequences - positive and negative outcomes of this choice
6. Alternatives considered - each with why it was rejected

## Quality bar

- Title states the decision, not the problem ("Use PostgreSQL" not "Database Selection")
- Context explains constraints without justifying the choice yet
- Consequences are honest: list downsides, not just benefits
- Alternatives section shows the decision was reasoned, not arbitrary

## Step-by-step instructions

1. Confirm the decision being recorded and its status
2. Write context: what changed, what constraint exists, what was unclear
3. Write the decision statement in present tense
4. List consequences: what gets easier, what gets harder, what is now locked in
5. Write 2-3 alternatives with honest rejection reasons
6. Assign ADR number and link to superseded ADR if replacing one

## References

- `references/guide.md` - ADR numbering, status lifecycle, templates
