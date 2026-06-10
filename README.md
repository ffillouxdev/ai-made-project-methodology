# ai-project-method

This is my go-to starter repository for projects built with AI help.
It contains a README.md (for your own project), that's where the AI understands
what you want (the global context).

## Why?

I always create README.md and TODO.md files when I start a project where AI
helps me build it. I used to use AI CLIs like a chatbot, and I felt like I was
getting dumber. By following this README + TODO method, I think much more about
the project's design up front — even drawing diagrams on paper and I know 
exactly what I want.

## Principles

- A README that gives the context to any AI.
- A TODO so the AI can chain features, commits, etc., which lets me do something
  else while it works.
- I always set up a linter or a code analyzer (personally: SonarQube) before my
  Plan 1, so the AI keeps coding and correcting the way it writes my project,
  this makes sure it follows good practices.

So the principle is: Design / Planning / Methodology (Human) -> Context
refinement (AI) -> Execution (AI) -> Code review and tests (AI).
