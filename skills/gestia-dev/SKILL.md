---
name: gestia-dev
description: Main engineering workflow for the Gestia repository. Use for non-trivial implementation, architecture, debugging, backend/frontend integration, database changes, security-sensitive work, reviews, and releases.
---

# Gestia Dev

Before non-trivial work:

1. Read `PROJECT_CONTEXT.md`.
2. Read relevant parts of `API.md` when touching backend/frontend contracts.
3. Inspect `schema.sql` when touching persistence, reporting, tenancy, payments, or migrations.
4. Inspect existing code before designing new abstractions.

Preserve project rules unless the user explicitly changes them:

- Gestia is focused cost control, not a general ERP.
- AI proposes; a human confirms consequential actions.
- `empresa_id` isolation is mandatory.
- Entity and cost center are separate dimensions.
- Financial totals are deterministic code/SQL, never authoritative LLM arithmetic.
- Uploaded documents belong in object storage, not PostgreSQL.
- Raw model extraction should remain auditable.
- Prefer boring infrastructure and configuration over customer-specific code.

For implementation:

- Make the smallest end-to-end change that solves the task.
- Keep API behavior aligned with `API.md`.
- Keep database invariants in PostgreSQL when possible.
- Run relevant tests/type checks/builds.
- Review tenancy, auth, error paths, and accidental unrelated changes.
- Summarize what changed, checks run, and remaining risks.

Use the more specialized skills in this repository when relevant:
`feature-dev`, `fastapi-backend`, `react-typescript`, `frontend-design`,
`security-guidance`, `code-review`, `git-workflow`, and `project-context`.
