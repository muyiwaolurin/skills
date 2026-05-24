---
name: code-review
description: >
  Review code diffs with severity tagging and actionable feedback. Use this skill whenever the user asks for help with
  anything related to code review. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Code Review

## Purpose

Review code diffs and PRs. Flag bugs, security issues, and design problems with severity. Output: structured findings the author can act on immediately.

## Inputs to gather

- Diff or PR link
- Context: what the change is supposed to do
- Review scope: full review, security-only, or quick sanity check
- Language and framework

## Output structure

1. Summary - one sentence on overall quality
2. Critical findings - bugs, security issues, data loss risks (must fix)
3. Major findings - design problems, performance issues (should fix)
4. Minor findings - style, naming, missing tests (consider fixing)
5. Positives - what was done well

## Quality bar

- Every finding includes: file, line, problem, and fix suggestion
- No vague feedback - say exactly why and what to change
- Critical vs minor clearly separated
- If nothing critical found, say so explicitly

## Step-by-step instructions

1. Read the diff top to bottom
2. Identify intent: what problem is this change solving
3. Check correctness: does the logic do what it claims
4. Check security: injection, auth bypasses, exposed secrets, improper input handling
5. Check edge cases: nulls, empty inputs, concurrent access
6. Check tests: present and covering critical paths
7. Group findings by severity, write each with file + line + fix

## References

- `references/guide.md` - severity definitions, common bug patterns
