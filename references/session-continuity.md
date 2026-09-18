# Multi-Round Session Continuity

Use this when simulating a full interview process or multiple rounds. Session continuity state must be stored in the same `logs/` session file defined by `weakness-log.md`; do not create a separate state file.

## Purpose

Real interview loops are connected. Later interviewers may test claims from earlier rounds. The coach should track what the user said and check consistency.

## Round State Section

```markdown
## Claims Made

- Project:
- Technical claim:
- Metric/outcome:
- Risk/tradeoff mentioned:

## Strengths Shown

-

## Weaknesses Flagged

-

## Threads To Revisit

-
```

## How To Use

During later rounds, ask follow-ups like:

- "In the previous round you said FlowPilot uses idempotency for connectors. Walk me through exactly where the idempotency key is generated and stored."
- "Earlier you mentioned low-confidence fallback. How would you measure whether fallback is triggered too often?"
- "You said Power Platform is sometimes better than custom code. Give me the decision rule."

## Consistency Checks

Flag:

- changed project scope,
- invented metrics,
- inconsistent technology claims,
- claiming production scale not in profile,
- overclaiming ownership.

When inconsistency appears, ask the user to repair the answer truthfully.
