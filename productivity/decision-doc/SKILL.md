---
name: decision-doc
description: >
  DACI/RACI structured decision documents. Use this skill whenever the user asks for help with
  anything related to decision doc. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Decision Doc

## Purpose

Write structured decision documents using DACI or RACI. Output: a doc that aligns stakeholders and records the decision with its reasoning. Users: leads and PMs driving cross-functional decisions.

## Inputs to gather

- Decision to be made - stated as a question
- Driver (DACI: D), Approver, Contributors, Informed
- Options under consideration
- Deadline for the decision
- Context: why this decision is needed now

## Output structure

1. Decision question - one clear sentence
2. Context and background - why this decision matters now
3. DACI table - Driver, Approver, Contributors, Informed
4. Options considered - each with pros, cons, and key trade-off
5. Recommendation - preferred option with rationale
6. Decision outcome - filled in after approval
7. Follow-up actions with owners and dates

## Quality bar

- Decision question is answerable - not open-ended "what should we do about X"
- Options section shows real trade-offs, not a strawman vs winner
- Recommendation states confidence level and key assumptions
- DACI has exactly one Driver and one Approver

## Step-by-step instructions

1. Write the decision question as a single closed question
2. Write 2-3 sentences of context: what changed, what is at risk
3. Populate DACI roles with names, not team names
4. Write 2-4 options with honest pros and cons
5. State recommendation with top 2-3 reasons
6. Set decision deadline and next review date
7. List follow-up actions post-decision

## References

- `references/guide.md` - DACI vs RACI, decision doc templates
