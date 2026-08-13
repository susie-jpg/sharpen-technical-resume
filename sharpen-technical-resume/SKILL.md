---
name: sharpen-technical-resume
description: Rewrite and strengthen Chinese or English technical resumes into concise, high-density, evidence-backed, results-oriented narratives. Use for resume/CV polishing, project-experience rewriting, AI/LLM/Agent/software-engineering resumes, extracting resumes from text, screenshots, PDF, DOCX, Markdown, or links, tailoring a resume to a job description, or turning loose project notes into credible resume bullets. Preserve facts, expose missing evidence, and never invent metrics, ownership, titles, technologies, awards, or business impact.
---

# Sharpen Technical Resume

Turn raw experience into a recruiter-scannable technical narrative: context and goal, personal scope, architecture or execution chain, measured outcome, and proof. Match the source language unless the user asks otherwise.

## Workflow

1. Read every supplied page or image before rewriting. For PDF, DOCX, or image input, use the relevant document/image tooling to extract both text and layout cues.
2. Identify the target role, seniority, language, page limit, and job description from the request or source. If absent, infer conservatively from the strongest experience and state the assumption briefly.
3. Build a private fact ledger for each experience:
   - organization, product, dates, role, team context;
   - problem, users, constraints, and baseline;
   - exact personal decisions, implementation, and ownership boundary;
   - architecture, workflow, interfaces, scale, and hard technical difficulty;
   - outcome metrics, comparison basis, measurement window, and evidence links;
   - claims that are ambiguous, unsupported, confidential, or still missing.
4. Separate claims into `verified`, `plausible but needs confirmation`, and `do not use`. Never silently promote an uncertain claim.
5. Prioritize experiences by relevance and evidence strength. Compress routine implementation; expand distinctive systems, decisions, scale, and outcomes.
6. Rewrite each substantial project using the pattern library in [references/patterns.md](references/patterns.md). Do not force every heading when a compact bullet is stronger.
7. Run the quality gate below. Revise until the resume is dense but readable.
8. Deliver the polished resume plus a short `待确认项 / Items to verify` section outside the resume. When useful, include a concise change rationale, but do not bury the usable output under commentary.

## Truth And Attribution

- Preserve the difference between led, owned, co-built, implemented, contributed, and supported.
- Use `项目 owner`, `从 0 到 1`, `主导`, `核心作者`, or equivalent only when the source establishes that scope.
- Do not invent numbers. If a metric would materially improve a bullet, insert an explicit placeholder such as `[请补充：耗时从 X 降至 Y]` in a draft, or ask for it in `待确认项`.
- Qualify causality. Prefer `上线后观察到`, `使...降低`, or `贡献于` according to the evidence; do not claim sole causation from correlation.
- Do not expose confidential internals. Generalize sensitive names, volumes, or topology while retaining technical substance.
- Keep links only when they substantiate a claim: repository, paper, demo, award, article, or product.

## Rewrite Rules

- Lead with the strongest signal, not a task inventory.
- Use a project title that communicates product/system and technical theme.
- Establish `背景/目标` in one concise bullet when context is not obvious.
- State personal scope before deep technical detail.
- Show end-to-end chains with compact arrows when sequence matters, for example `ingest -> validate -> plan -> execute -> evaluate`.
- Name technologies only when they explain a decision, constraint, interface, or result. Avoid keyword walls.
- Prefer concrete mechanisms: scheduling policy, fallback path, evaluation rubric, cache boundary, failure recovery, data flow, concurrency model, or protocol.
- Attach numbers to a defined object and unit: users, requests/month, latency P95, success rate, cost/run, throughput, conversion, test coverage, or benchmark delta.
- Include baseline and measurement window when available. `提升 30%` alone is weaker than `SWE-bench 通过率由 40% 提至 52%（n=200）`.
- Keep bullets parallel and front-load bold labels only when they improve scanning.
- Remove self-evaluation, inflated adjectives, redundant background, repeated tech stacks, and low-information verbs such as `负责`, `参与`, `熟悉` without a concrete object.
- Optimize for the target role. For AI/Agent roles, foreground model/tool orchestration, context engineering, evaluation, failure recovery, data synthesis, inference cost, and reproducibility. For general software roles, foreground system boundaries, reliability, performance, data contracts, and delivery impact.

## Output Modes

- `Polish`: preserve sections and facts; rewrite wording and ordering.
- `Rebuild`: redesign hierarchy and condense weak content around the target role.
- `Tailor`: map verified evidence to a supplied job description without copying its wording or fabricating fit.
- `Audit`: return claim risks, missing metrics, vague bullets, and recommended questions before rewriting.

If the user does not choose, use `Rebuild` for loose notes or visibly weak structure, otherwise use `Polish`.

## Quality Gate

Score the draft using [references/quality-gate.md](references/quality-gate.md). Require all of the following:

- Every major claim traces to source text or a clearly marked user-confirmation item.
- The first half-page surfaces role, strongest evidence, and target-role relevance.
- Each major project communicates problem, personal contribution, mechanism, and outcome when the facts permit.
- Metrics have objects and units; comparisons have baselines where available.
- Bullets distinguish individual contribution from team output.
- Technical density does not destroy readability: one primary idea per bullet, no unnecessary nesting, and no unexplained acronym pileups.
- Repetition and generic claims are removed.

## Handling Missing Information

Do not block initial progress. Produce the strongest truthful draft from current evidence, then list at most 5 high-value questions ranked by expected resume impact. Ask about ownership, baseline/result, scale, hard constraint, and public proof before asking cosmetic questions.
