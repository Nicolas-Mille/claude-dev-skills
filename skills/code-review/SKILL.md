---
name: code-review
description: Review code, commits, branches, and pull requests for correctness, security, data integrity, API compatibility, concurrency, and maintainability.
---

# Code Review

Prioritize findings in this order:

1. correctness / data corruption
2. tenant isolation and security
3. authorization
4. financial calculation errors
5. API/schema contract breakage
6. transactions/concurrency
7. error handling
8. realistic performance problems
9. maintainability
10. style

For each meaningful issue include:
- severity
- file/location
- why it matters
- concrete fix

Do not manufacture issues just to appear thorough. If the change is good, say so.
Distinguish blockers from optional improvements.
