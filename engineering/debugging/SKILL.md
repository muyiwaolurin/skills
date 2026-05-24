---
name: debugging
description: >
  Systematic root-cause analysis and fix recommendations. Use this skill whenever the user asks for help with
  anything related to debugging. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Debugging

## Purpose

Systematic root-cause analysis for bugs, errors, and regressions. Reproduce first, hypothesise second, fix last. Skip no phases.

## Inputs to gather

- Error message or symptom - exact text, not paraphrase
- Steps to reproduce or last known good state
- Recent changes: code, config, deps, infrastructure
- Environment: local, staging, or prod

## Output structure

1. Reproduction steps confirmed
2. Hypothesis list - ranked by likelihood
3. Instrumentation plan - what to add/check per hypothesis
4. Root cause identified - evidence trail
5. Fix with explanation
6. Regression test added

## Quality bar

- Root cause is a specific line or condition, not "something is wrong with X"
- Fix addresses cause, not symptom
- Regression test prevents reoccurrence
- If root cause not found, explicitly state what was ruled out

## Step-by-step instructions

1. Reproduce the bug - get a fast, deterministic fail signal
2. Narrow scope: isolate to smallest reproducing case
3. List 3-5 hypotheses ordered by likelihood
4. Test top hypothesis: add logging or run targeted check
5. Eliminate and repeat until root cause confirmed
6. Write fix - minimal change that addresses root cause
7. Add regression test covering the exact failure mode

## References

- `references/guide.md` - debugging loops, bisection, instrumentation patterns
