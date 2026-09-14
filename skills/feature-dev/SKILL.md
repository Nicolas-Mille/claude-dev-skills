---
name: feature-dev
description: Implement software features end to end with repository exploration, a small plan, scoped implementation, validation, and concise handoff.
---

# Feature Development

Use this workflow for non-trivial features.

## Understand
- Identify the exact user-visible behavior.
- Locate existing routes, components, models, schemas, tests, and utilities.
- Check current contracts before inventing new ones.
- Prefer the smallest vertical slice that delivers value.

## Plan
Keep the plan short:
- files likely to change
- API impact
- database impact
- UI impact
- security/tenancy risks
- validation needed

## Implement
- Follow existing project patterns.
- Avoid unrelated rewrites.
- Avoid abstractions created only for hypothetical future reuse.
- Prefer simple, reversible choices.

## Verify
Run what is relevant:
- tests
- type checks
- linters
- frontend build
- critical manual flow

Also check authorization, tenant isolation, error behavior, and API compatibility.

## Finish
Report:
1. what changed
2. files/areas changed
3. checks run
4. remaining risks or follow-ups
