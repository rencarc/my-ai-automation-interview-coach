# Coding And Debugging Interview

Use this for coding, API integration, debugging, and implementation rounds. Tailor exercises to AI automation, full-stack AI apps, workflow connectors, and data/API handling.

## Interaction Contract

Before starting, choose one mode:

- **Chat pseudocode mode**: user explains approach and writes code-like snippets in chat.
- **Live coding simulation**: coach acts like a shared-editor interviewer; user thinks aloud and pastes incremental code.
- **Debugging mode**: coach provides a broken snippet or failure scenario; user asks clarifying questions and diagnoses.

Rules:

- Ask the user to think aloud.
- Do not interrupt during the first implementation attempt unless they are stuck for a long time or violating a core constraint.
- Do not dump the solution.
- Give time checks using `time-control.md` when the user spends too long clarifying or coding.
- After the attempt, score with `calibration-rules.md` and ask for one refactor or one extra test.

## What To Practice

Prioritize realistic coding tasks over abstract puzzle-only prep:

- parse and validate structured intake data,
- design a REST API endpoint,
- implement retry with idempotency,
- transform webhook payloads,
- filter records by user/role,
- implement simple search or ranking,
- write tests for edge cases,
- debug a failing async workflow,
- reason about SQL queries and indexes.

## Mock Flow

1. Clarify input/output and constraints.
2. Propose a simple approach.
3. Identify edge cases.
4. Implement or outline code.
5. Walk through tests.
6. Discuss complexity and maintainability.
7. Refactor or debug if prompted.

## Personalized Practice Problems

1. Given an unstructured request object, return missing required fields and a risk category.
2. Implement an idempotency-key store for webhook calls.
3. Build a retry scheduler with max attempts and dead-letter output.
4. Filter retrieved documents by `user_id`, `tenant_id`, and role.
5. Merge semantic-search results and keyword-search results into one ranked list.
6. Parse Power Automate-style payloads into normalized Dataverse-style records.
7. Given chat history, trim messages to a token budget while keeping recent context.
8. Write a function that detects duplicate workflow submissions.
9. Design SQL tables for cases, approvals, audit logs, and connector executions.
10. Debug why a RAG answer cites a document the user should not access.

## Scorecard

Use the 1-4 scoring scale in `calibration-rules.md`. Score these dimensions:

- Clarification: asks about input shape, constraints, and failure cases.
- Correctness: solves the core case.
- Edge cases: handles empty input, duplicates, auth boundaries, retries, and malformed payloads.
- Complexity: can explain time/space or query cost.
- Code quality: readable naming, small functions, clear tests.
- Debugging communication: narrates hypotheses and checks evidence.

## Strong Signals

- Writes or describes tests before claiming done.
- Handles retries and duplicates explicitly.
- Avoids exposing secrets or calling OpenAI from the client.
- Separates validation, business logic, persistence, and side effects.
- Explains tradeoffs instead of over-engineering.

## Red Flags

- Jumps into code without clarifying data shape.
- Ignores idempotency for external actions.
- Forgets authorization filters in data retrieval.
- Cannot explain why a bug is happening.
- Says "we can just retry" without limits, backoff, or dead-letter handling.
