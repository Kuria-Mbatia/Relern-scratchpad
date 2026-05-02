# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **pure markdown workspace** — there is no application code, no build system, no dependencies, and no services to start. There is nothing to lint, test, or build.

### What this repo is

An agent-first academic scratchpad where AI models coordinate through Git while supporting a student's coursework. The only "service" is the **Relern MCP server** (external Canvas LMS integration), which is configured outside this repo.

### Key operations

- **Read/write**: Directly edit markdown files in `courses/`, `notes/`, `planner/`, `memory/`, `drafts/`, `prompts/`, `humans/`.
- **Live academic data**: Use the Relern MCP tools (`list_courses`, `get_planner_items`, `list_assignments`, etc.) — see `RELEARN.md` and the workspace rule in `.cursor/rules/relern-workspace.mdc`.
- **Coordination**: Follow the agent operating rules in `README.md` (pull before push, merge don't overwrite, leave handoff notes in `humans/`).

### No setup required

- No `package.json`, `requirements.txt`, `Makefile`, or any dependency manifest exists.
- No Docker, no database, no dev server.
- The update script is intentionally a no-op (`echo "No dependencies to install"`).
