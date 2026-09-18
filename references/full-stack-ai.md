# Full-Stack AI Application Interview

Use this for full-stack AI developer interviews involving Next.js, TypeScript, Supabase, PostgreSQL, OpenAI API, Docker, Azure, Vercel, and API integration.

## Profile Anchors

Projects and experience:

- FlowPilot AI: Next.js, TypeScript, Supabase, OpenAI API, pgvector, RBAC/RLS, connector adapters.
- Gote Note: Next.js, Supabase, PostgreSQL, Prisma, OpenAI API, authenticated note Q&A.
- SAS internship: OpenAI retrieval, Rasa chatbot, Docker, Azure deployment.
- RAG FAQ Assistant: Azure AI Search, Copilot Studio, Power Automate.

## Likely Questions

1. Walk me through the architecture of FlowPilot AI.
2. How do you structure a Next.js app that calls OpenAI securely?
3. How do you manage authentication and authorization with Supabase?
4. How did you use pgvector or embeddings?
5. How do you design API connector adapters?
6. What does idempotency mean, and why does it matter for workflow connectors?
7. How do retry/cancel and failure tracking work in automation systems?
8. How did you containerize and deploy an application with Docker and Azure?
9. How do you handle chat history and contextual workflows?
10. How would you debug a failed AI response in production?

## Strong Answer Pattern

For each project:

```text
User problem:
Architecture:
Frontend:
Backend/API:
Database:
AI integration:
Auth/security:
Reliability:
Tradeoff:
What I would improve next:
```

## Technical Areas To Drill

- server-side API routes vs client-side calls,
- secrets management,
- database schema design,
- vector search and fallback search,
- authentication and user-scoped data,
- error handling and observability,
- Docker/Azure deployment basics,
- connector idempotency and retries.

## Red Flags To Avoid

- Saying "I used OpenAI API" without explaining data flow, prompting, retrieval, or error handling.
- Not distinguishing frontend, backend, database, and AI responsibilities.
- Ignoring auth and privacy in personal knowledge apps.
- Treating deployment as an afterthought.
