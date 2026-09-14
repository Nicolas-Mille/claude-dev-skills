---
name: react-typescript
description: Frontend engineering guidance for React and TypeScript applications consuming an API contract.
---

# React + TypeScript

- Follow the existing component and routing structure.
- Keep API types aligned with the backend contract.
- Separate server data from local UI state.
- Handle loading, empty, error, and success states.
- Never hardcode production data.
- Frontend permission hiding is UX only; backend authorization is authoritative.
- Avoid unnecessary global state.
- Extract reusable components after real reuse appears, not before.
- Keep data transforms explicit and test critical mappings.
- Preserve field names from the API contract unless an intentional adapter exists.

If TypeScript language-server tooling is available, use its diagnostics and
references. Fix errors introduced by the current change without unrelated cleanup.
