# AGENTS.md

<!--
Template — copy this file to the root of a new project and fill in the
placeholders. It tells any AI coding agent how to work in this repo.
Keep it short: agents read it on every task, so only put what changes how they
work. Delete these comments when done.
-->

This is the operating manual for AI agents working in this repository. Read it
fully before starting any task. For the project's purpose and goals, read
`README.md`; for what to do next, read `TODO.md`.

## Workflow (this is a methodology-first repo)

1. **Context first.** Read `README.md` and `TODO.md`, then infer the rest from
   the existing code and neighboring conventions.
2. **No ping-pong.** Don't ask questions one at a time. Resolve unknowns with
   sensible defaults and announce them. If something is genuinely blocking, ask
   all such questions in a single batch, then proceed.
3. **Plan then execute.** Work through `TODO.md` plan by plan, chaining features
   and commits autonomously so the human can do something else meanwhile.
4. **Self-review.** After generating code, run the linter/analyzer (see below),
   fix what it flags, and add or update tests.

## Commands

<!-- Fill these in for the project. -->
- **Install:** `<...>`
- **Run / dev:** `<...>`
- **Build:** `<...>`
- **Test:** `<...>`
- **Lint / format:** `<...>`
- **Static analysis:** SonarQube / SonarScanner (run before closing a plan)

## Conventions

- **Language:** English for code, identifiers, commits and documentation.
  Client-facing UI in another language only when end users require it.
- **Code style:** follow the existing style and the project's linter/formatter.
  No superfluous dependencies.
- **Structure:** `<describe folder layout / entry points>`.
- **Docs:** keep `README.md` accurate; add `ARCHITECTURE.md` when routing or
  data flows need explaining.

## Git

- Atomic commits with clear English messages.
- **Never** add `Co-Authored-By: Claude` or any AI co-author trailer to commits
  or PR descriptions.
- Work on a dedicated branch; do not push to `main` unless asked.

## Quality gate

- Run static analysis (SonarQube) and the linter after generating code.
- Create or update tests for new behavior.
- Don't consider a plan done until analysis is clean and tests pass.

## Do NOT

<!-- Hard guardrails. -->
- Touch confidential/proprietary assets; keep them in a gitignored folder
  (e.g. `data/`, `datas/`) and never commit them.
- `<other project-specific guardrails>`

---

> If you also use Claude Code, point its `CLAUDE.md` at this file
> (e.g. a single line: `See AGENTS.md`) so there's one source of truth.
