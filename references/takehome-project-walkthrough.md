# Take-Home Strategy And Project Walkthrough

Use this for take-home assignments and 10-15 minute project presentations.

## Take-Home Strategy

Before building, clarify:

- expected time box,
- evaluation criteria,
- must-have requirements,
- optional requirements,
- delivery format,
- whether AI tools are allowed.

## Time Allocation

For a 4-hour take-home:

- 30 min: understand requirements and define scope,
- 2 hours: implement core flow,
- 45 min: tests, error states, security basics,
- 30 min: README and tradeoffs,
- 15 min: final cleanup.

Do not spend all time on UI polish if the role is backend/workflow-heavy.

## README Structure

```text
# Project

## What I built
## How to run
## Architecture
## Key decisions
## Tradeoffs
## Security / error handling
## What I would improve next
```

Strong take-homes explicitly explain tradeoffs and TODOs. A thoughtful TODO is better than hidden unfinished work.

## What To Leave As TODO

Acceptable TODOs:

- deeper observability,
- more exhaustive tests,
- production deployment hardening,
- more advanced ranking/evaluation,
- admin UI,
- full CI pipeline.

Risky TODOs:

- authentication,
- basic validation,
- core happy path,
- obvious security issue,
- app cannot run.

## 15-Minute Project Walkthrough

Use this structure:

1. Problem and users: 1 minute
2. Architecture overview: 2 minutes
3. Key technical decisions: 4 minutes
4. Hardest tradeoff or bug: 2 minutes
5. Security/reliability: 2 minutes
6. Outcome and demo: 2 minutes
7. What I would improve next: 2 minutes

## FlowPilot AI Walkthrough Angle

Lead with:

- internal requests are often unstructured,
- AI can help structure and classify,
- governance is needed before actions execute,
- human review, policies, audit logs, RBAC/RLS make it safe.

## Gote Note Walkthrough Angle

Lead with:

- personal notes become queryable,
- authentication and user-scoped retrieval are central,
- RAG is useful only if it respects data boundaries.

## Common Mistakes

- spending 10 minutes on background before architecture,
- listing technologies without decisions,
- hiding limitations,
- no demo path,
- no security or error handling,
- no clear "what I would improve next."
