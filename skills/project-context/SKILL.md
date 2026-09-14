---
name: project-context
description: Keep engineering work grounded in the repository's durable project context, API contract, schema, and current decisions.
---

# Project Context

When working in a repository with project context files:

1. Read `PROJECT_CONTEXT.md` before architectural or product decisions.
2. Read `API.md` before changing request/response behavior or frontend data usage.
3. Read `schema.sql` before changing persistence, reporting, financial logic, or tenancy.
4. Treat these documents as authoritative unless the user explicitly asks to revise them.
5. Inspect current code because implementation may have advanced since the docs were written.

When a durable decision changes:
- update the relevant existing section
- store decisions/current state, not chat transcripts
- do not store secrets
- do not update context for trivial implementation details
