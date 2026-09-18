# Weakness Log And Scorecard

Use this when the user wants repeated practice or progress tracking.

## Purpose

Each mock should produce a structured scorecard so future sessions can target recurring weaknesses instead of starting from zero.

## Storage

Actual session data belongs in `logs/`, not in `references/`.

After every scored mock, create or update one Markdown file under:

```text
logs/YYYY-MM-DD_<module>_<short-topic>.md
```

If the environment cannot write files, output the same Markdown in chat and tell the user it should be saved under `logs/`.

## Unified Session File

Use one file per mock/session. Do not maintain separate weakness and continuity files. The same file contains both claims and scores.

## Session Template

```markdown
# Interview Session Log

Date:
Module:
Target role:
Topic:
Language mode:

## Claims Made

| Claim | Source answer | Reuse / verify later |
|---|---|---|
| | | |

## Strengths Shown

-

## Weaknesses Flagged

-

## Scores

| Dimension | Score 1-4 | Evidence | Why not higher |
|---|---:|---|---|
| Problem framing | | | |
| Technical depth | | | |
| Security/governance | | | |
| Reliability/operations | | | |
| Communication | | | |

## Three Specific Deductions

1.
2.
3.

## Best Evidence

-

## Retry Prompts

-

## Next Session Focus

-

## Follow-Up Questions To Reuse

-
```

## Start-Of-Session Use

Before a new mock, if previous logs are available:

1. List recent files under `logs/`.
2. Read the latest 1-3 logs for the same module/project.
2. Identify recurring dimensions scoring 1-2.
3. Start the mock by saying the targeted focus.
4. Choose questions that pressure the recurring weak area.

Example:

```text
Last time your weakest recurring area was evaluation. I will use a RAG prompt today and push specifically on how you prove retrieval improved.
```

## Progress Summary

After several scorecards, summarize:

- average score by dimension,
- recurring weakness,
- strongest module,
- weakest module,
- next three drills.
