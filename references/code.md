# Source code / automation / architecture

## Detect
- Unnecessary abstraction layers, boilerplate wrappers, invented helpers and dependencies.
- Comments that simply restate code, fake TODO completions, dead code, unused imports.
- Demo data or hard-coded successes presented as real implementation.
- Missing error paths, secret leakage, unhandled I/O, unnecessary network operations.
- Rewriting a functional subsystem only to improve formatting or perceived elegance.
- Over-architecting a local task; adding unrelated frameworks.

## Revise
- Keep behavior, public interfaces, state names, tests and integration contracts unless change was requested.
- Prefer smallest maintainable implementation; isolate reusable code only when there is proven reuse.
- Explicitly handle failures and platform constraints; no fabricated test results.
- Use stable naming and comments describing 'why' rather than paraphrasing 'what'.
- For user-facing apps, combine with interfaces.md. For document/code-generation pipelines, combine with matching medium reference.

## Verify
Run available tests and linters when appropriate; report exact commands/results. Where runtime access is missing, describe the untested path without claiming production readiness. Do not install unreviewed packages or change machine permissions without authorization.
