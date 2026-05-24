---
name: metrics-analysis
description: >
  Interpret product data and write insight narratives. Use this skill whenever the user asks for help with
  anything related to metrics analysis. Trigger even on casual phrasing — if the
  intent matches, load this skill.
---

# Metrics Analysis

## Purpose

Interpret product data and write insight narratives. Output: clear analysis with a "so what" recommendation. Users: PMs, analysts, and stakeholders who need data to drive decisions.

## Inputs to gather

- Metric name and time range
- Baseline or target to compare against
- Business context: what decision does this data inform
- Data source and any known quality issues

## Output structure

1. Metric summary - what it measures and current value
2. Trend analysis - direction, magnitude, anomalies
3. Segmentation - which cohorts or dimensions drive the change
4. Root cause hypotheses - top 2-3 explanations
5. Recommendation - what to do next, with confidence level
6. Data caveats - limitations to flag

## Quality bar

- Every insight tied to a business decision or action
- Correlation vs causation flagged explicitly
- Confidence level stated for each recommendation
- No "the number went up" without explaining why it matters

## Step-by-step instructions

1. Confirm what decision this analysis should inform
2. Summarise the metric: current value, period, comparison point
3. Identify trend direction and rate of change
4. Segment by relevant dimensions: user type, region, feature flag
5. Generate root cause hypotheses, ranked by likelihood
6. Recommend next action: ship, investigate further, or revert
7. Flag data quality issues or confounders

## References

- `references/guide.md` - analysis frameworks, common metric pitfalls
