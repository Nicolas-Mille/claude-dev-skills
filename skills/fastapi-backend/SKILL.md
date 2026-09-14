---
name: fastapi-backend
description: Backend engineering guidance for Python, FastAPI, Pydantic, PostgreSQL, APIs, transactions, validation, and external model integrations.
---

# FastAPI Backend

- Use explicit Pydantic request/response schemas.
- Keep route handlers small; move reusable or genuinely complex domain logic out.
- Use database constraints for invariants that must never be violated.
- Use transactions when multiple writes form one logical operation.
- Return deliberate HTTP status codes and useful error bodies.
- Avoid broad exception swallowing.
- Validate all external API/model responses before persistence.
- Treat model output as untrusted input.
- Never use an LLM as the source of truth for financial arithmetic.
- Prefer deterministic parsers for fixed-format documents.
- Keep tenant scoping explicit and centralized.
- Do not trust IDs from clients without authorization checks.
- Keep secrets out of source, logs, examples, and committed env files.

If Python language-server/type-checker tooling is available, use it to inspect
new diagnostics and symbol references. Do not perform unrelated repo-wide cleanup.
