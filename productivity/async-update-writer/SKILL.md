---
name: async-update-writer
description: >
  Engineering updates, weekly digests, and changelogs. Use this skill whenever the user asks for help with
  anything related to async update writer. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Async Update Writer

## Purpose

Write engineering updates, weekly digests, and changelogs. Output: scannable, factual updates that keep stakeholders informed without meetings. Users: engineers and leads writing team or product updates.

## Inputs to gather

- Update type: weekly digest, sprint summary, incident update, or changelog
- Audience: team, leadership, or external users
- What shipped, what is in progress, what is blocked
- Any decisions made or changed

## Output structure

1. Headline - key outcome or theme of the period
2. Shipped - list of completed items with brief impact note
3. In progress - current work and expected completion
4. Blocked or at risk - what needs attention and from whom
5. Decisions made - any direction changes or resolutions
6. Next up - planned work for next period

## Quality bar

- "Shipped" items describe outcome, not activity ("users can now X" not "we worked on X")
- Blocked items name the blocker and the ask
- Total length under 300 words for weekly updates
- No filler, no preamble - start with the content

## Step-by-step instructions

1. Confirm update type and audience
2. List completed work - extract from PRs, tickets, or notes
3. Write each shipped item as user-facing outcome where possible
4. List in-progress items with owners and expected dates
5. Identify blockers and what is needed to unblock
6. Summarise any decisions or direction changes
7. Add next period preview

## References

- `references/guide.md` - update templates, changelog formats
