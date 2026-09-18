# RAG And LLM App System Design

Use this for RAG, knowledge assistants, LLM applications, semantic search, retrieval quality, grounded answers, and system design interviews tailored to the user's profile.

## Core Narrative

The user has hands-on RAG experience across:

- Azure AI Search and Copilot Studio in RAG FAQ Assistant.
- Supabase pgvector, semantic embeddings, citations, and keyword fallback in FlowPilot AI.
- OpenAI API and authenticated personal-note retrieval in Gote Note.
- OpenAI retrieval and Rasa chatbot integration at SAS.

## Design Framework

For any RAG system design answer, guide the user through:

1. Use case and users
2. Knowledge sources and permissions
3. Ingestion and chunking
4. Embeddings and indexing
5. Retrieval strategy
6. Reranking or filtering
7. Prompt construction
8. Citation and answer grounding
9. Confidence checks
10. Fallback and escalation
11. Evaluation
12. Security, privacy, and audit logs

## Full Mock Interview Flow

Use this when the user asks for a realistic mock. The interviewer should assess first and coach only in the debrief.

| Phase | Time | What to test |
|---|---:|---|
| Setup | 1-2 min | Confirm prompt, target role, level, and whether the system is Microsoft-stack, custom-stack, or hybrid. |
| Requirements | 5-8 min | Users, knowledge sources, data sensitivity, latency, answer quality, scale, ownership, compliance, and success metrics. |
| High-level design | 10-15 min | Ingestion, storage, indexing, retrieval, generation, citations, UI/workflow, auth, observability. |
| Deep dive | 15-20 min | Pick the weakest or most relevant area: chunking, hybrid search, permission filtering, confidence/fallback, evaluation, or connector reliability. |
| Tradeoffs | 5-8 min | Azure AI Search vs pgvector, Copilot Studio vs custom app, semantic vs keyword fallback, automation vs human approval. |
| Debrief | 5-10 min | Score by dimensions, quote the user's strongest and weakest moments, give 2-3 next drills. |

Hard rules:

- Do not design the system for the user during the mock.
- Reject vague phrases like "use a vector database" unless the user explains indexing, filtering, retrieval, and evaluation.
- If the user skips access control, push immediately: "Can every user retrieve every document?"
- If the user skips fallback, ask: "What happens when retrieval is empty or low quality?"
- If the user skips evaluation, ask: "How would you know this assistant improved?"

## Topics To Probe

### Retrieval Quality

Ask:

- How do you know the retrieved context is relevant?
- What happens if retrieval returns nothing useful?
- How do you combine semantic search and keyword fallback?
- How would you evaluate retrieval quality?

Strong answer signals:

- separates retrieval quality from generation quality,
- mentions citations or source grounding,
- discusses fallback and manual escalation,
- understands access control at retrieval time.

### Permissions

Ask:

- How do you prevent users from retrieving documents they should not see?
- Where should authorization happen: before retrieval, after retrieval, or both?
- How did Gote Note ensure users only queried their own notes?

Strong answer signals:

- row-level security or user-scoped filtering,
- authenticated retrieval,
- document-level permissions,
- audit trail for sensitive workflows.

### Hallucination And Confidence

Ask:

- How do you reduce hallucinations in a RAG assistant?
- What should the assistant do when confidence is low?
- How do you design fallback messages?

Strong answer signals:

- grounded prompts,
- source citation,
- thresholding or confidence checks,
- "I don't know" behavior,
- human escalation.

## Personalized System Design Prompts

Use these instead of generic system design prompts:

1. Design an internal RAG FAQ assistant for HR/IT support.
2. Design a governed AI intake system that classifies risk and detects missing information.
3. Design a personal knowledge assistant where each user can query only their own notes.
4. Design an AI workflow platform that proposes automations but requires human approval.
5. Design a Copilot-style assistant connected to SharePoint and Dataverse.
6. Design a retrieval system with citations, semantic search, keyword fallback, and manual escalation.
7. Design an LLM application observability flow for failed or low-confidence answers.

## Mature System Design Topics Adapted To This Profile

Use these instead of generic prompts when possible:

| Topic | What it stresses | Personal evidence to use |
|---|---|---|
| Internal RAG FAQ assistant | retrieval quality, fallback, escalation | Akavia RAG FAQ Assistant |
| Governed AI intake platform | risk classification, human review, audit logs | FlowPilot AI |
| Personal knowledge assistant | user-scoped retrieval, auth, note search | Gote Note |
| Multi-tenant LLM gateway | quotas, routing, caching, fallback | OpenAI API + governance experience |
| Workflow connector platform | idempotency, retries, failure tracking | FlowPilot connector adapters |
| Copilot over SharePoint/Dataverse | permissions, enterprise knowledge, low-code tradeoffs | Insutex and Akavia |
| LLM evaluation pipeline | golden sets, retrieval metrics, regression checks | RAG answer quality work |

## Back-Of-Envelope Numbers To Practice

Use approximate numbers and state assumptions. Strong candidates do not say "fast" or "scalable" without sizing.

- Seconds per day: about 86,400.
- Same-datacenter round trip: sub-millisecond order of magnitude.
- Cross-region synchronous calls often add tens to hundreds of milliseconds.
- Redis-like cache: think 100k+ ops/sec per instance order of magnitude.
- PostgreSQL single primary: think tens of thousands of simple writes/sec order of magnitude before sharding discussions.
- RAG cost drivers: embedding refresh volume, retrieval latency, model tokens, reranking, and human escalation rate.

Practice formulas:

```text
avg_qps = daily_requests / 86,400
peak_qps = avg_qps * peak_factor
tokens_per_day = requests_per_day * avg_prompt_and_completion_tokens
storage_growth = documents_per_day * avg_document_size * retention_days
```

## Named Patterns To Reach For

- **Transactional outbox** for reliably publishing workflow events after database writes.
- **Idempotency key** for external workflow/API actions that may be retried.
- **Dead-letter queue** for failed automations that require investigation.
- **Hybrid retrieval** for semantic + keyword fallback.
- **Permission-filtered retrieval** for user/role/document scoped RAG.
- **Human approval gate** for high-risk AI-generated actions.
- **Audit log** for who asked, what was retrieved, what AI proposed, and what action was taken.
- **Single-flight/request coalescing** for repeated expensive retrieval/model calls.
- **Tenant isolation with RLS** for multi-tenant workflow systems.

## Scorecard

Use the 1-4 scoring scale in `calibration-rules.md`. Score these dimensions:

- Requirements and user scope
- Knowledge/data modeling
- Retrieval and grounding quality
- Security and permissions
- Fallback/evaluation/operations
- Communication and tradeoffs

## Question Package Generator

When the user asks for a generated system design practice package, create exactly four sections or files:

1. `question`: one-paragraph interviewer prompt with no solution hints.
2. `assumptions`: concrete DAU/QPS/data size/latency/security assumptions.
3. `interviewer-notes`: clarifying questions, deep-dive targets, failure modes, and 10x follow-ups.
4. `rubric`: observable scoring criteria for the target level and one level above.

For this user, bias generated packages toward RAG, workflow automation, Power Platform integration, governed AI actions, and full-stack AI apps.
