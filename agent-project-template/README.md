# Agent Project Template

Fork/clone this repository as the starting point for a new project.

## First setup

1. Rename the repository.
2. Fill out `project.md`.
3. Replace `task.md` with the first concrete task.
4. Leave `AGENTS.md` stable unless you discover a genuinely reusable rule.
5. Use `.agent/state.md` for multi-turn working state.
6. Record durable architecture choices in `.agent/decisions.md`.
7. Record verified external facts in `.agent/knowledge.md`.

## Design principle

Keep the always-loaded contract small. Put task-specific and workflow-specific information in the files that actually apply.

## Compatibility

- Codex: root `AGENTS.md`
- Claude Code: root `CLAUDE.md` imports `AGENTS.md`
- GitHub Copilot: `.github/copilot-instructions.md` imports `AGENTS.md`
- Cursor: root `AGENTS.md` is supported; use `.cursor/rules/` for path-scoped rules when needed
