# Universal Anti-Slop (custom skill, v0.2)

A format-aware review workflow for eliminating **generic AI-output patterns**, not a guarantee of human authorship or an AI-content detector.

## Contents
- `SKILL.md`: shared lifecycle, safeguards, and routing
- `references/common.md`: common audit
- `references/writing.md`: prose, translations, copy
- `references/presentations.md`: presentations
- `references/interfaces.md`: web, Windows, Android, vehicle UI
- `references/code.md`: source code and automation
- `references/visuals.md`: illustrations and media
- `references/asset-first.md`: original asset planning, creation, integration, and verification (conditional for visual deliverables)
- `references/data-documents.md`: reports, spreadsheets, accounting charts
- `AGENTS.snippet.md`: optional global automation policy

## Install in Codex CLI (PowerShell on Windows)
1. Download `universal-anti-slop.zip` and navigate to the folder containing it.
2. Run:

```powershell
New-Item -ItemType Directory -Force "$HOME\.agents\skills" | Out-Null
Expand-Archive -LiteralPath ".\universal-anti-slop.zip" -DestinationPath "$HOME\.agents\skills" -Force
```

3. Codex should find `$HOME\.agents\skills\universal-anti-slop\SKILL.md`. Restart Codex if it is not listed.
4. Explicit: `Use $universal-anti-slop to review this deliverable in deep mode.`
5. For routine application to deliverables, append the contents of `AGENTS.snippet.md` to `$HOME\.codex\AGENTS.md`; **append, do not replace** an existing file. Existing instructions may take precedence. Confirm the skill was actually applied.

## Quick one-shot prompt (any model)

```text
다음 결과물을 Universal Anti-Slop 방식으로 검수해.
1. 매체(글/PPT/보고서/웹/앱/차량 UI/코드/이미지)를 먼저 식별해.
2. 원래 목적, 독자, 사실, 숫자, 인용, 기능, 사용자 문체를 보존해.
3. 획일적인 구성, 상투적 표현, 과도한 장식, 근거 없는 주장, 불필요한 복잡성을 탐지해.
4. 문제의 구체적인 위치와 수정 이유를 제시하고 중요한 문제부터 수정해.
5. 수정 후 의미·기능·시각적 결과를 검증해. 검증하지 못한 부분은 명시해.
6. AI가 자주 쓰는 요소라는 이유만으로 무조건 삭제하지 마.
결과물 유형에 맞는 규칙만 적용해. 필요 없으면 과도하게 손대지 마.
```

## Source inspirations (not dependencies)
- https://github.com/blader/humanizer
- https://github.com/pbakaus/impeccable
- https://github.com/Leonxlnx/taste-skill
- https://github.com/petergyang/no-ai-slop
- https://learn.chatgpt.com/docs/build-skills

This is an original standalone workflow. None of the external skills is installed or imported into this bundle.
