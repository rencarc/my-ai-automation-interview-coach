# Interviewer Rubric And Loop Design

Use this to reverse-engineer interviewer expectations, design mock loops, generate scorecards, or calibrate whether an answer is junior, mid, or senior-leaning.

## Mature Loop Templates For This Profile

### AI Automation / Power Platform Developer

| Round | Time | Competencies |
|---|---:|---|
| Recruiter / motivation screen | 30 min | role fit, communication, career switch narrative |
| Power Platform / automation case | 60 min | Power Apps, Power Automate, Dataverse, Copilot Studio, workflow design |
| RAG / AI assistant design | 60 min | retrieval, grounding, fallback, evaluation, permissions |
| Coding / API integration | 45-60 min | TypeScript/Python, REST APIs, webhooks, idempotency, testing |
| Behavioral / stakeholder round | 45 min | ambiguity, ownership, business process understanding, collaboration |

### RAG / LLM Application Developer

| Round | Time | Competencies |
|---|---:|---|
| Technical screen | 45 min | LLM app basics, API usage, data flow |
| RAG system design | 60 min | ingestion, chunking, hybrid retrieval, citations, evaluation |
| Full-stack implementation | 60 min | Next.js, Supabase/PostgreSQL, auth, backend API design |
| Governance/security | 45 min | access control, audit logs, human review, sensitive data |
| Behavioral | 30-45 min | communication, learning speed, project ownership |

### Full-stack AI Developer

| Round | Time | Competencies |
|---|---:|---|
| Coding | 60 min | correctness, edge cases, API design, maintainability |
| System design | 60 min | AI app architecture, auth, data model, reliability |
| Project deep dive | 45 min | FlowPilot AI or Gote Note technical decisions |
| Cloud/deployment | 30-45 min | Docker, Azure/Vercel, CI/CD, secrets, monitoring |
| Behavioral | 30 min | ownership, stakeholder communication, tradeoffs |

## 4-Point Hiring Rubric

- **1 - Does not meet**: significant gaps, cannot explain core decisions, misses security or workflow basics.
- **2 - Partial**: some relevant experience, but answers are tool-listing or need heavy guidance.
- **3 - Meets**: solid role fit, explains data flow, tradeoffs, security, and failure handling.
- **4 - Exceeds**: strong beyond level, connects business process, architecture, governance, metrics, and operations.

Use this 4-point rubric directly. Do not translate it into a 1-5 scale.

## Level Calibration For Zhen's Target Roles

| Competency | Junior signal | Mid signal | Senior-leaning signal |
|---|---|---|---|
| AI automation | Can explain tools used | Designs end-to-end flows with fallback | Chooses automation boundaries, risk gates, ownership, and measurable value |
| RAG/LLM | Knows embeddings and vector search | Designs retrieval + grounding + citations | Discusses evaluation, permission filtering, failure modes, and operations |
| Power Platform | Names components | Explains Power Pages/Apps/Automate/Dataverse data flow | Discusses governance, environment strategy, ALM, licensing/maintainability tradeoffs |
| Full-stack | Builds frontend + API + DB | Handles auth, data model, deployment | Designs reliability, observability, idempotency, and secure data boundaries |
| Security | Mentions RBAC | Applies RLS/access control correctly | Defines blast radius, auditability, abuse cases, and approval boundaries |
| Communication | Explains what was built | Explains why decisions were made | Frames business problem, tradeoffs, stakeholder impact, and what changed |

## Candidate-Side Coaching Ladder

When preparing the user, move answers up this ladder:

1. Tool names
2. Data flow
3. Decision rationale
4. Failure handling
5. Security/governance
6. Business impact
7. Tradeoffs and what would be improved next

If the user stops at one layer, probe the next.

## Bias And Process Checks

Use these to explain what interviewers may penalize:

- halo effect: one strong tool answer should not cover weak fundamentals,
- similarity bias: career-switch background must be framed as evidence, not apology,
- over-indexing on one project: prepare at least three project stories,
- vague scorecards: convert answers into competencies,
- trivia questions: redirect to job-relevant design and implementation,
- unstructured debriefs: insist on dimension-by-dimension feedback during mocks.

## Structured Debrief Template

Use after full mocks:

```text
Round:
Target role:
Overall signal:

Scores:
- Technical depth:
- Role-specific competency:
- Security/governance:
- Reliability/operations:
- Communication:

Hire signal:
Main concern:
Evidence from answer:
What a stronger answer would include:
Next drills:
```
