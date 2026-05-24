---
name: tech-debt-assessment
description: >
  Identify, classify, and prioritise technical debt. Use this skill whenever the user asks for help with
  anything related to tech debt assessment. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Tech Debt Assessment

## Purpose

Identify, classify, and prioritise technical debt. Output: ranked debt inventory with business impact and remediation cost. Users: engineering leads and PMs deciding what debt to pay down and when.

## Inputs to gather

- Scope: specific module, service, or whole codebase
- Team velocity impact: how much slower does this debt make the team
- Age and churn rate of affected code
- Known incidents or bugs caused by this debt

## Output structure

1. Debt inventory - list of identified items
2. Classification per item: architectural, code quality, test coverage, dependency, or documentation
3. Business impact: velocity drag, incident risk, onboarding cost
4. Remediation effort estimate: S/M/L or days
5. Priority ranking: impact vs effort
6. Recommended paydown plan with sequencing rationale

## Quality bar

- Every item has a stated business impact - not "it is messy"
- Priority ranking uses impact-effort matrix, not gut feel
- Debt items are specific and actionable, not vague ("the auth module is bad")
- Sequencing accounts for dependencies between items

## Step-by-step instructions

1. Confirm scope and ask what business outcomes matter most
2. Survey the area: read code, check test coverage, review recent bug history
3. List debt items with specific location and symptom
4. Classify each item by type
5. Estimate business impact: velocity, risk, hiring/onboarding cost
6. Estimate remediation effort per item
7. Plot on impact-effort matrix and recommend priority order
8. Write sequencing rationale: which items unblock others

## References

- `references/guide.md` - debt classification taxonomy, impact estimation frameworks
