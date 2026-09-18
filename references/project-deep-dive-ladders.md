# Project Deep-Dive Ladders

Use this when an interviewer asks about a resume project. The goal is to test whether the user can go three layers deeper than the resume bullet.

Use `profile.md` as the source of truth. If an implementation detail is not in `profile.md` and the user has not supplied it, ask for it instead of inventing it. This is especially important for metrics, embedding models, vector index settings, production scale, internal company systems, and confidential workflow details.

## FlowPilot AI Ladder

Start:

- "Walk me through FlowPilot AI."

Deep-dive chain:

1. What problem did it solve, and who is the user?
2. How does unstructured intake become a structured case?
3. What fields are extracted, and how is missing information detected?
4. How does risk classification work?
5. What policies are used for RAG grounding?
6. How are embeddings stored in Supabase pgvector?
7. How do citations get attached to risk explanations?
8. How do RBAC and RLS work together?
9. What goes into the audit log?
10. How do connector adapters handle idempotency, retry, cancel, and failure tracking?
11. What would break first with 10x usage?
12. What would you improve next?

Pass signal:

- Can explain data model, AI boundary, approval flow, access control, connector reliability, and failure handling.

## Gote Note Ladder

1. Why build a personal knowledge assistant?
2. What is the data model for notes/users?
3. How is authentication handled?
4. How do you ensure users retrieve only their own notes?
5. What does the Q&A flow look like?
6. Did you use semantic retrieval, keyword search, or both?
7. How do you handle empty or irrelevant retrieval?
8. How do you protect OpenAI API calls and secrets?
9. How would you evaluate answer quality?
10. What would you add for production readiness?

Pass signal:

- Can explain authenticated retrieval and data isolation clearly.

## Akavia RAG FAQ Assistant Ladder

1. What was the FAQ assistant supposed to solve?
2. What knowledge sources were used?
3. How did Azure AI Search fit in?
4. What did Copilot Studio handle?
5. What did Power Automate orchestrate?
6. How were retrieval quality signals handled?
7. What counted as low confidence?
8. What fallback message was shown?
9. When was manual escalation triggered?
10. How would you measure whether the assistant worked?

Pass signal:

- Can separate retrieval, answer generation, fallback, and escalation.

## Akavia IT Case / Onboarding Workflow Ladder

1. What was the intake flow?
2. Why Power Pages for intake?
3. Why Power Apps for internal handling?
4. Why Dataverse for structured case data?
5. What did the Copilot onboarding workflow collect?
6. How were account setup and role-based notifications triggered?
7. What could fail in the workflow?
8. How would you monitor failed requests?
9. What access-control risks existed?
10. How would you improve maintainability?

## Insutex Ladder

1. What did the Copilot Studio agent do?
2. What internal knowledge did it query?
3. How did SharePoint structure affect answer quality?
4. What permissions mattered?
5. How did website/API integration connect external input to internal automation?
6. What was the hardest integration risk?
7. How would you evaluate whether the agent helped employees?

## SAS Ladder

1. What was the full-stack app?
2. How did OpenAI retrieval fit in?
3. What did Rasa handle?
4. How was chat history stored and used?
5. What were dynamic cards?
6. Why Docker?
7. How was it deployed to Azure?
8. What would you monitor in production?

## Thesis Ladder

1. What problem exists in automotive CAN security?
2. What is rule-based detection good at?
3. What is supervised learning good at?
4. What is anomaly detection good at?
5. Why use a hybrid/fusion strategy?
6. How did you preprocess CAN data?
7. What features were engineered?
8. How did known attacks vs unknown attacks differ?
9. What does cross-vehicle evaluation test?
10. How does this thesis influence your AI governance thinking?

## Drill Rule

If the user cannot answer layer 4 or deeper, stop and build that project story before doing more generic question practice.
