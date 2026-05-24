---
name: testing-strategy
description: >
  Design test plans covering unit, integration, and e2e layers. Use this skill whenever the user asks for help with
  anything related to testing strategy. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Testing Strategy

## Purpose

Design test plans across unit, integration, and e2e layers. Output: test pyramid recommendation, coverage priorities, and tool choices. Users: engineers planning a test suite or filling coverage gaps.

## Inputs to gather

- System type: API, UI, data pipeline, library
- Current test coverage and pain points
- Deployment frequency and risk tolerance
- Language, framework, existing test tooling

## Output structure

1. Test pyramid recommendation - ratio of unit/integration/e2e
2. Coverage priorities - what to test first and why
3. Unit test plan - which modules, what behaviour to assert
4. Integration test plan - which seams, what contracts to verify
5. E2E test plan - which critical user journeys to automate
6. Tool recommendations with rationale
7. What not to test - explicitly scope out

## Quality bar

- Tests verify behaviour through public interfaces, not internals
- Coverage priorities tied to risk: what breaks most, costs most
- No "test everything" - explain trade-offs in what is skipped
- Tool choices match team's existing stack where possible

## Step-by-step instructions

1. Identify the riskiest code paths: payment flows, auth, data writes
2. Map existing coverage: what layers are already tested
3. Design unit tests for pure logic and edge cases
4. Design integration tests for service boundaries and DB interactions
5. Design e2e tests for 2-3 critical user journeys only
6. Recommend test tooling per layer
7. List what to skip and why (trivial getters, third-party code)

## References

- `references/guide.md` - test pyramid, mocking guidelines, coverage targets
