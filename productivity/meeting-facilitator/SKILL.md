---
name: meeting-facilitator
description: >
  Agendas, action items, and meeting summaries. Use this skill whenever the user asks for help with
  anything related to meeting facilitator. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Meeting Facilitator

## Purpose

Produce agendas, action items, and meeting summaries. Output: structured docs that make meetings shorter and follow-through reliable. Users: anyone running or summarising a meeting.

## Inputs to gather

- Meeting type: planning, retro, decision, kickoff, or status
- Attendees and their roles
- Desired outcome: what must be decided or completed by end
- Time available
- Pre-read materials or context

## Output structure

For agenda:
1. Meeting goal - one sentence outcome
2. Timed agenda items with owner per item
3. Pre-read links or required prep

For summary:
1. Decisions made - numbered list
2. Action items - owner, task, due date
3. Parking lot - items deferred with owner to resolve
4. Next meeting date and focus

## Quality bar

- Every agenda item has a clear purpose and time box
- Action items have a single owner, not "the team"
- Summary decisions are unambiguous - no "we discussed X"
- Parking lot prevents scope creep mid-meeting

## Step-by-step instructions

1. Confirm meeting goal and time available
2. List agenda items, assign time boxes and owners
3. Put most critical decision first - guard against time running out
4. During or after meeting: capture decisions verbatim
5. Extract action items: task + owner + due date
6. Record deferred items in parking lot with resolution path
7. Send summary within 24 hours

## References

- `references/guide.md` - agenda templates, retro formats, meeting types
