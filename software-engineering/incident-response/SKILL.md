---
name: incident-response
description: >
  Runbooks, on-call guidance, and post-mortem templates. Use this skill whenever the user asks for help with
  anything related to incident response. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Incident Response

## Purpose

Generate runbooks, on-call guidance, and post-mortem templates. Output: actionable docs that reduce MTTR and prevent repeat incidents. Users: on-call engineers, SREs, and team leads.

## Inputs to gather

- Incident type: outage, data issue, security event, or performance degradation
- Systems involved: services, databases, third-party dependencies
- Severity level: P1/P2/P3 or equivalent team definition
- For post-mortems: timeline of events and contributing factors

## Output structure

For runbook:
1. Symptom description and detection signal
2. Immediate mitigation steps - numbered, executable
3. Root cause investigation steps
4. Escalation path with contacts
5. Recovery verification checklist

For post-mortem:
1. Incident summary - what happened, when, impact
2. Timeline - key events with timestamps
3. Root cause analysis
4. Contributing factors
5. Action items - owner, task, due date
6. What went well

## Quality bar

- Runbook steps are executable without prior knowledge of the system
- Post-mortem is blameless: actions target systems and processes, not people
- Every action item has a single owner and due date
- Impact is quantified: users affected, error rate, duration

## Step-by-step instructions

1. Confirm doc type: runbook, on-call guide, or post-mortem
2. For runbook: write detection criteria first, then mitigation steps
3. Test mitigation steps for completeness - can someone follow them at 3am
4. For post-mortem: write timeline before analysis to separate facts from interpretation
5. Identify root cause and contributing factors separately
6. Write action items targeting systemic fixes, not one-off patches
7. Add "what went well" to reinforce good practices

## References

- `references/guide.md` - incident severity definitions, post-mortem templates
