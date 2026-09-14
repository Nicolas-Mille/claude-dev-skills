# Claude Dev Skills

A small skill pack for Claude Code and other agents compatible with the open Agent Skills format.

## Included

- `gestia-dev` — umbrella workflow for the Gestia project
- `feature-dev` — end-to-end feature implementation
- `fastapi-backend` — Python/FastAPI/PostgreSQL backend guidance
- `react-typescript` — React + TypeScript frontend guidance
- `frontend-design` — serious B2B UI guidance
- `security-guidance` — SaaS/API/upload/AI security checks
- `code-review` — correctness/security-first reviews
- `git-workflow` — safe commits, diffs and PR workflow
- `project-context` — read and maintain project context/contracts

## Install with `npx skills`

Install interactively from a public GitHub repository:

```bash
npx skills@latest add Nicolas-Mille/claude-dev-skills -a claude-code
```

Install every discovered skill:

```bash
npx skills@latest add Nicolas-Mille/claude-dev-skills --all -a claude-code
```

Install only the Gestia umbrella skill:

```bash
npx skills@latest add Nicolas-Mille/claude-dev-skills --skill gestia-dev -a claude-code -y
```

List what the repository exposes before installing:

```bash
npx skills@latest add Nicolas-Mille/claude-dev-skills --list
```

After installing in an existing Claude Code session, run:

```text
/reload-skills
```

## About Pyright / TypeScript LSP

Pyright and TypeScript language-server support are external tooling, not `SKILL.md`
files. The backend/frontend skills are written to take advantage of those tools when
they are available, but this repository does not pretend to install an LSP.

## Repository layout

```text
skills/
  gestia-dev/
    SKILL.md
  feature-dev/
    SKILL.md
  fastapi-backend/
    SKILL.md
  react-typescript/
    SKILL.md
  frontend-design/
    SKILL.md
  security-guidance/
    SKILL.md
  code-review/
    SKILL.md
  git-workflow/
    SKILL.md
  project-context/
    SKILL.md
```
