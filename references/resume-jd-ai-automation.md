# Resume And JD Alignment For AI Automation Roles

Use this when tailoring the user's resume or interview positioning to a specific job description.

## Non-Fabrication Rule

When rewriting resume bullets, never add numbers, percentages, scale, outcomes, customers, users, cost savings, latency improvements, or production claims that are not present in `profile.md` or explicitly provided by the user.

If a bullet would be stronger with quantified evidence, use a placeholder instead of inventing:

```text
[needs your data: e.g. time saved, number of users, number of cases, accuracy/quality measure]
```

Ask the user for the missing evidence. Do not "reasonably estimate" it.

This rule also applies to interview positioning and project deep dives. Do not infer exact implementation choices such as embedding model, vector index parameters, production traffic, or internal company process details unless the user provided them.

## Best-Fit Role Families

Prioritize:

- AI Automation Developer
- AI Engineer
- Power Platform Developer
- RAG / LLM Application Developer
- Workflow Automation Engineer
- Full-stack AI Developer
- Junior/Mid Software Developer with AI focus
- Microsoft-focused AI/Automation Consultant

Secondary fits:

- Business Systems Developer
- Solutions Developer
- Technical Consultant
- Junior Cloud/AI Developer
- Security-aware AI application developer

Less ideal unless the JD matches strongly:

- pure ML researcher,
- pure cybersecurity analyst,
- pure backend infrastructure engineer,
- senior platform engineer,
- PM-only roles.

## Keyword Groups

Match the resume to JD terms in these groups:

### AI And RAG

- RAG
- LLM applications
- OpenAI API
- semantic search
- embeddings
- vector database
- pgvector
- Azure AI Search
- grounded answers
- citations
- confidence checks
- fallback
- prompt design

### Automation And Integration

- workflow automation
- Power Automate
- API integration
- REST APIs
- webhooks
- connector adapters
- human-in-the-loop
- escalation
- idempotency
- retry handling

### Microsoft Stack

- Copilot Studio
- Power Platform
- Power Apps
- Power Pages
- Dataverse
- SharePoint
- Azure AI
- Azure
- PL-400
- AI-102

### Full Stack And Data

- Next.js
- TypeScript
- JavaScript
- Python
- SQL
- PostgreSQL
- Supabase
- Prisma
- Docker
- Vercel

### Security And Governance

- RBAC
- Row Level Security
- access control
- audit logs
- AI governance
- risk classification
- information security

## Tailoring Rules

- Lead with AI automation + secure workflow systems.
- Move Power Platform and Copilot Studio higher for Microsoft-heavy JDs.
- Move Next.js/Supabase/OpenAI higher for startup/full-stack AI JDs.
- Move RBAC/RLS/audit logs/thesis higher for security-aware JDs.
- Keep business operations as a differentiator for stakeholder/process roles.

## Resume Bullet Rewrite System

Use compressed CAR:

```text
Improved [system/process/metric] by [specific action], resulting in [outcome] across [scope].
```

Each strong bullet should answer:

- What problem existed?
- What did Zhen personally design/build/improve?
- What changed for users, workflow quality, reliability, security, or maintainability?

Prefer action verbs such as built, shipped, deployed, integrated, automated, designed, structured, architected, scoped, improved, reduced, streamlined, analyzed, identified, coordinated, and aligned.

Avoid weak openers such as responsible for, helped with, worked on, participated in, assisted with, and contributed to.

If exact metrics are unavailable, use credible qualitative landmarks:

- enabled manual escalation for low-confidence answers,
- improved permission-aware information access,
- created a governed approval path for AI-proposed workflow actions,
- connected external intake with internal case handling,
- isolated user-owned notes for authenticated Q&A.

Do not convert these qualitative landmarks into fake numbers.

## ATS / Recruiter Skim Checklist

For every target JD, check:

1. Does the top summary match the role family?
2. Are the top 8-12 JD keywords visible in the first half of the resume?
3. Are Microsoft keywords prominent for Microsoft-stack jobs?
4. Are RAG/LLM keywords prominent for AI app jobs?
5. Are security/governance keywords prominent for regulated workflow jobs?
6. Does each experience show action, system, and outcome?
7. Are projects ordered by relevance to the JD?
8. Does the business background support the role instead of distracting from it?

## Interview Pitch Template

```text
I am an AI automation and full-stack developer with a background in information security and business operations. My recent work focuses on RAG assistants, Copilot Studio workflows, Power Platform systems, and governed AI automation. I am strongest where AI needs to connect with real business workflows, structured data, permissions, fallback handling, and human review.
```

## Resume Review Checklist

Check whether the resume clearly shows:

- target role title alignment,
- AI automation positioning in the summary,
- Microsoft/Power Platform experience,
- RAG and LLM implementation details,
- security/governance differentiator,
- full-stack implementation evidence,
- demos/projects,
- measurable or observable outcomes,
- Swedish market readiness and language progress where useful.

## JD Match Output

When reviewing a JD, produce:

```text
Target role fit:
Fit score:
Top matched evidence:
Missing or weak keywords:
Resume bullets to move higher:
Bullets to rewrite:
Interview risks:
Best positioning sentence:
```
