---
name: git-workflow
description: Safe Git workflow for status checks, diffs, commits, branches, pull requests, and release-ready handoff.
---

# Git Workflow

Before committing:
- inspect `git status`
- inspect the diff
- ensure no secrets/local artifacts are included
- avoid unrelated formatting churn
- run relevant checks

Commit messages should be concise and behavior-oriented, for example:
- `feat: add document confirmation endpoint`
- `fix: enforce tenant scope on suggestions`
- `refactor: isolate extraction validation`

Do not push, merge, delete branches, or open PRs unless the user asks or the
environment explicitly authorizes the action.

For PRs summarize:
- problem
- solution
- notable implementation choices
- validation performed
- known limitations
