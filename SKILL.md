---
name: universal-anti-slop
description: Review AI-generated prose, code, UI/design, presentations, spreadsheets, and images for formulaic or low-quality results while preserving facts, functionality, and user requirements. Do not automatically apply to research documents or factual and technical investigation notes.
---

# Universal Anti-Slop — cross-medium quality gate

## Purpose
Improve specificity and craft, not conceal AI authorship. Never claim that a result is human-written, guaranteed undetectable, original, or free from all AI patterns. Do not reduce every output to the same minimalist aesthetic. Keep useful patterns when their function justifies them.

## Activation and scope
- **Local default:** Automatically apply to AI-generated prose, code, UI/design, presentations, spreadsheets, and image creation. Select checks appropriate to each medium. For existing prose, do not infer AI authorship from stylistic patterns.
- Do not automatically apply to research documents, investigation reports, factual answers, source summaries, support/capability assessments, or technical verification notes, even if AI writes them. Continue normal accuracy and evidence checks without invoking this style-review workflow.
- Apply the relevant cross-medium references and asset-first gate when appropriate for code or visual deliverables. The research-document exclusion remains in force.
- An explicit user request for Anti-Slop or prose editing may override these default exclusions, only within the requested scope.
- For qualifying new prose: use **create -> audit -> revise -> verify** with `references/common.md` and `references/writing.md`.
- For qualifying existing prose: use **audit -> revise -> verify**, only editing within the requested scope. For critique only, audit without modifying files.
- Preserve facts, sources, quotations, voice, and the distinction between verified findings and experimental candidates. Limit broad revision cycles to two by default.
## Priority order
1. User's explicit requirements, purpose, audience, supplied references, and voice.
2. Truth, correct numbers, citations, semantics, and safety/accessibility constraints.
3. Usability and platform/format requirements.
4. Clarity, distinctiveness, visual polish.
5. Personal aesthetic preferences and anti-slop heuristics.

Never alter source facts, numbers, legal language, citations, formulas, user-provided quotes, or technical behavior solely to sound less AI-like. If an improvement conflicts with higher-priority requirements, preserve the requirement and flag the tradeoff.

## Universal workflow
1. **Identify the artifact.** Write down medium(s), target audience, core message/job, constraints, reference style, and protected information. Infer what is obvious; do not interrupt the user for nonessential details.
2. **Set a concrete quality target.** Define three to five observable criteria for this specific artifact. Avoid generic targets such as 'make professional'.
3. **Create or inspect a baseline.** Read the source fully when accessible. Preserve backups and original files unless the user asked for overwriting. For slides/UI/graphics, inspect the rendered artifact, not just text/code, when tools allow.
4. **Perform a common audit.** Load `references/common.md`. Find evidence of boilerplate, repetition, hollow claims, weak hierarchy, decorative excess, unnecessary complexity, and loss of user voice.
5. **Perform medium audit.** Load only the matching files:
   - Prose / scripts / translations / labels: `references/writing.md`
   - Slides / presentations: `references/presentations.md`
   - Websites / desktop / mobile / vehicle UI: `references/interfaces.md`
   - Source code / automation: `references/code.md`
   - Illustrations / graphics / media: `references/visuals.md`
   - Reports / spreadsheets / charts: `references/data-documents.md`
   - **Asset-first gate (conditional, all visual media):** if imagery is needed for identity, product character, explanations, status, or atmosphere, also load `references/asset-first.md`. Do not substitute emoji, generic stock icons, basic shapes, or text-only placeholders for an asset that should be designed for this artifact. Create and integrate the required asset files using available tools; a list of ideas or prompts alone is not a completed visual deliverable. Preserve standard functional icons where they improve recognition and accessibility.
6. **Prioritize defects.** P0 = broken facts/function/safety or missing core requirement; P1 = confusing or visibly generic; P2 = optional polish. Fix P0 first; never conceal a P0 behind cosmetic polish.
7. **Make targeted edits.** Prefer small justified changes. Preserve meaning, source assets, product identity, references, and intentional stylistic choices. Do not add random quirks to look human.
8. **Verify the actual output.** Recheck content, text overflow, layout/contrast, citations, equations, file integrity and functional behavior as relevant. If rendering/execution is unavailable, state the unverified area. Do not invent successful tests.
   For newly created visual assets, additionally confirm the files exist, are placed in the intended screens/slides, and render correctly at their actual display size. If asset generation is unavailable, report the missing assets explicitly rather than silently replacing them with emoji or claiming completion.
9. **Stop deliberately.** Stop when the output satisfies the artifact's purpose, remaining edits are subjective, or further edits would harm specificity, correctness, or voice. At most two broad aesthetic cycles by default; fix concrete remaining defects regardless of count.

## Quick mode / deep mode
- **Quick:** inspect and fix the three most consequential supported issues; keep changes localized; output revised artifact and short rationale.
- **Deep:** full cross-medium audit, explicit P0/P1/P2 list, 1–2 alternative directions if useful, revision, render/run validation, and unresolved caveats.
- Default to Quick for minor rewrites and single-slide tweaks. Default to Deep for decks, public-facing UI, codebases, consequential reports, or a request for redesign.

## Reporting contract
When useful, report only: `Changed`, `Why`, `Verified`, `Unverified` (not a long self-congratulatory checklist). Do not invent numeric scores, source references, tests, or screenshots. In audit-only mode, give precise examples and recommended fixes; do not silently change files.

## Suggested external skill composition
- Writing: optionally use `blader/humanizer` or `petergyang/no-ai-slop` as reference material; retain fact/voice safeguards here.
- Web and app UI: use the globally installed `impeccable` skill for interface design and review alongside this skill when applicable. Follow user scope, preserve existing functionality and identity, and retain the research-document exclusion. If unavailable, report it rather than claiming it ran. `Leonxlnx/taste-skill` remains optional.
- Presentation and document generation: let the native authoring tool generate/edit the file, then apply this audit as a separate pass.
- Other referenced skills are optional and must be evaluated before installation.

## Key rule
**Anti-slop is a context-aware editing method, not a ban list or AI-detector.**
