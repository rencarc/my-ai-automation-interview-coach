# Skill Eval Cases

Use this to test whether the skill follows its own rules after edits.

Only read this file when the user explicitly asks to run a self-test/eval.

## Output Format

For each case, output:

```text
Case N: PASS/FAIL - one-sentence reason
```

End with:

```text
Total: X/10
Fixes needed:
-
```

## Eval 1: Refuse Standard Answer During Mock

Input:

```text
Just tell me the perfect answer for designing a RAG assistant.
```

Expected:

- refuses to give full answer,
- gives 2-3 hints,
- asks user to try first.

## Eval 2: Weak Answer Gets 2/4

Input:

```text
I would use pgvector and OpenAI. It should work because vector search finds similar documents.
```

Expected:

- score 2/4, not 3/4,
- says missing chunking, permissions, fallback, evaluation,
- asks retry.

## Eval 3: Thin Routing

Input:

```text
Do a RAG mock.
```

Expected:

- loads profile, calibration-rules, rag-llm-system-design only,
- does not pull every reference,
- asks one first mock question.

## Eval 4: Project Deep Dive

Input:

```text
Deep dive FlowPilot AI.
```

Expected:

- uses profile and project-deep-dive-ladders,
- asks one question at a time,
- does not provide project answer.

## Eval 5: English Mode

Input:

```text
I will answer in English. Score content and English separately.
```

Expected:

- content score uses 1-4,
- English feedback separated,
- corrected phrasing offered after scoring, not before answer.

## Eval 6: Sweden Localization

Input:

```text
Prepare me for a Stockholm consulting company interview.
```

Expected:

- uses Sweden market module,
- mentions consulting/client-facing expectations,
- advises calm collaborative style,
- does not invent salary numbers.

## Eval 7: Power Platform Freshness

Input:

```text
Tell me exact current Copilot Studio licensing limits.
```

Expected:

- states product details may change,
- recommends checking official Microsoft docs,
- avoids confident stale claims.

## Eval 8: Weakness Log

Input:

```text
End this mock and create a scorecard.
```

Expected:

- outputs scorecard Markdown,
- includes scores, three deductions, next focus,
- uses 1-4 scoring.

## Eval 9: Live Coding

Input:

```text
Give me a coding round.
```

Expected:

- establishes interaction mode,
- asks user to think aloud,
- does not dump solution.

## Eval 10: Offer

Input:

```text
I got an offer in Stockholm. Should I negotiate?
```

Expected:

- asks for offer details,
- discusses salary plus benefits,
- uses Swedish collaborative tone,
- does not invent market salary.
