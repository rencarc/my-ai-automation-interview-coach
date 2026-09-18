# Implementation Details

This file documents what was implemented in `my-ai-automation-interview-coach` after reviewing mature external skills and adapting them to Zhen Xu's resume.

## Mature Skill Sources Used

### ftvision/system-design-skill

Adapted ideas:

- strict mock interview phase flow,
- assess-first / teach-in-debrief behavior,
- system design scoring dimensions,
- generated question package structure,
- topic catalog approach,
- back-of-envelope sizing expectations,
- named distributed-systems patterns,
- recurring weakness / drill mindset.

Implemented in:

- `SKILL.md`
- `references/rag-llm-system-design.md`
- `references/question-bank.md`

### borghei/Claude-Skills engineering/interview-system-designer

Adapted ideas:

- interview loop design,
- competency-based scorecards,
- 4-point hiring rubric,
- level calibration,
- bias/process guardrails,
- structured debrief format.

Implemented in:

- `references/interviewer-rubric.md`
- `SKILL.md`

### borghei/Claude-Skills personal-productivity/resume-tailor

Adapted ideas:

- CAR bullet rewrite pattern,
- weak phrase cleanup,
- action-verb framing,
- JD keyword grouping,
- ATS/recruiter skim checklist,
- structured JD match output.

Implemented in:

- `references/resume-jd-ai-automation.md`

### borghei/Claude-Skills pm-interview-prep

Adapted selectively:

- red-flag style coaching,
- avoid rote frameworks,
- require impact in behavioral answers,
- expose tradeoffs and counter-risks,
- avoid bluffing,
- prepare strong final interviewer questions.

Implemented in:

- `references/behavioral-career-stories.md`

## Personalized Resume-Based Additions

The skill was not left generic. It was specialized around the user's CV:

- Insutex: Copilot Studio, SharePoint knowledge structure, website/API integration.
- Akavia: Power Pages, Power Apps, Dataverse, Copilot onboarding workflow, RAG FAQ assistant.
- SAS: OpenAI retrieval, Rasa chatbot, Docker, Azure deployment.
- FlowPilot AI: governed AI intake, risk classification, pgvector RAG, RBAC/RLS, audit logs, connectors.
- Gote Note: authenticated personal-note Q&A with Supabase/PostgreSQL/OpenAI.
- Thesis: hybrid IDS for automotive CAN networks.
- Business operations background: stakeholder process analysis and automation context.

## Files Implemented

### `SKILL.md`

Implemented:

- personalized skill identity,
- target role families,
- mode routing,
- coaching rules,
- default scorecards,
- routing to all reference modules,
- coding/debugging and interviewer-rubric modes.

### `references/ai-automation-interview.md`

Implemented:

- positioning for applied AI automation roles,
- likely interview themes,
- project-specific examples from Insutex, Akavia, and FlowPilot AI,
- AI automation mock questions,
- evaluation bar for strong answers.

### `references/rag-llm-system-design.md`

Implemented:

- RAG design framework,
- full mock interview phase structure,
- hard interviewer rules,
- personalized system design prompts,
- mature topic catalog adapted to RAG/workflow/LLM roles,
- back-of-envelope sizing practice,
- named engineering patterns,
- RAG scorecard,
- generated question package format.

### `references/power-platform-interview.md`

Implemented:

- Power Platform profile anchors,
- common interview questions,
- strong answer pattern,
- tradeoff prompts,
- red flags for low-code interviews.

### `references/governance-security.md`

Implemented:

- AI governance and security profile anchors,
- mock questions,
- strong answer components,
- project mapping to FlowPilot AI, Gote Note, and thesis.

### `references/full-stack-ai.md`

Implemented:

- Next.js/Supabase/PostgreSQL/OpenAI/Docker/Azure interview coverage,
- likely questions,
- project explanation pattern,
- technical drill areas,
- red flags.

### `references/behavioral-career-stories.md`

Implemented:

- career-switch narrative,
- story bank,
- STAR plus reflection,
- mature answer checks,
- behavioral red flags,
- strong end-of-interview questions.

### `references/resume-jd-ai-automation.md`

Implemented:

- best-fit role families,
- keyword groups,
- tailoring rules,
- CAR bullet rewrite system,
- ATS/recruiter skim checklist,
- pitch template,
- resume review checklist,
- structured JD match output.

### `references/coding-debugging-interview.md`

Implemented:

- coding/debugging mock flow,
- personalized coding tasks,
- implementation scorecard,
- strong signals,
- red flags.

### `references/interviewer-rubric.md`

Implemented:

- mature mock loop templates for three target role families,
- 4-point hiring rubric,
- level calibration matrix,
- coaching ladder,
- bias/process checks,
- structured debrief template.

### `references/question-bank.md`

Implemented:

- AI automation question bank,
- RAG/LLM question bank,
- Power Platform question bank,
- governance/security question bank,
- full-stack AI question bank,
- behavioral question bank,
- four-week practice plan,
- final readiness checklist.

## What This Skill Can Now Do

It can now support:

- full mock interviews,
- RAG/LLM system design practice,
- Power Platform case interviews,
- AI automation workflow interviews,
- coding/API/debugging rounds,
- governance/security rounds,
- project deep dives,
- behavioral storytelling,
- resume/JD tailoring,
- question bank generation,
- four-week practice planning,
- interviewer-style scoring and debriefs.

## Version 1.1 Structural Improvements

Implemented after structural review:

- **Thin router**: `SKILL.md` now only routes to the necessary 1-2 references and explicitly says not to pre-read all references.
- **Single scoring source**: `references/calibration-rules.md` is now the only scoring truth.
- **Unified 1-4 scale**: removed competing 1-5 scoring language from active modules.
- **Few-shot calibration**: added transcripts showing weak answer -> hint -> retry, refusal to give standard answers, and an explicit wrong-coach example.
- **No-answer-completion rule**: strengthened with concrete examples.
- **Profile source of truth**: added `references/profile.md` so resume facts are maintained in one place.
- **Weakness log**: added `references/weakness-log.md` for cross-session scorecards and progress tracking.
- **Time control**: added `references/time-control.md` for behavioral, system design, and coding pacing.
- **Session continuity**: added `references/session-continuity.md` for multi-round interview loops and consistency checks.
- **Reverse questions**: added `references/reverse-questions.md` for hiring manager, teammate, and HR questions.
- **Failure postmortem**: added `references/failure-postmortem.md` for rejection/weak-interview diagnosis.
- **Sweden offer negotiation**: added `references/sweden-offer-negotiation.md` for offer analysis beyond salary expectation.
- **Live coding contract**: added interaction rules to `coding-debugging-interview.md`.
- **Power Platform freshness rule**: added explicit caution about changing Microsoft product capabilities and licensing.
- **Skill eval cases**: added `tests/eval-cases.md` to test the skill behavior after edits.

## What Was Intentionally Not Fully Copied

Not fully copied:

- original state-file tracking from `system-design-skill`,
- voice/TTS support,
- exact external scripts from `interview-system-designer`,
- exact resume matcher script,
- full PM interview question bank,
- product research/customer interview modules.

Reason:

The target is not a generic mega-skill. It is a focused personal interview coach for AI automation, RAG, Power Platform, secure workflows, and full-stack AI roles.

## Suggested Next Enhancements

1. Add `scripts/jd_keyword_matcher.py` for automatic JD/resume keyword scoring.
2. Add `assets/story-bank-template.md` for filling in behavioral stories.
3. Add `assets/mock-scorecard-template.md` as a reusable file version of `weakness-log.md`.
4. Add optional practice state tracking similar to `system-design-skill`.
5. Add 3 complete scripted mock sessions.
