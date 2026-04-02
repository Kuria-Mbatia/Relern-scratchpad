# Relern Workspace

**This repository is an agent-first academic scratchpad for models working across Codex, Cursor, Claude, Kimi, and similar tools.**

**It exists so models can interact with classes through Relern/Canvas, keep working notes, leave structured handoffs, and collaborate through Git without losing context.**

This is not primarily a human notebook. Humans should understand that the repo is meant for agents to read from, write to, and coordinate through while supporting coursework.

Use it as a writable workspace for:
- course summaries
- assignment breakdowns
- study guides
- draft messages
- planning notes
- model handoff context
- human-facing task summaries

Relern and Canvas remain the source of truth for live academic data. This repo is a working memory layer, not the canonical record for deadlines, grades, or official course content.

## Recommended setup

1. Fork this repository into your own GitHub account.
2. Open the fork in Codex, Cursor, Claude Code, or another agent-enabled workspace.
3. Connect the Relern MCP in your tool of choice.
4. Use this repo as the shared scratchpad while Relern provides live course context.

## Agent operating rules

1. At the start of any task, sync the latest GitHub state before doing anything else.
2. Check the current latest notes, planner items, and task artifacts so you do not add updates to stale data.
3. Do your work locally in the appropriate workspace folders.
4. Prefer new handoff files or clearly scoped updates so concurrent agents are less likely to collide on the same text.
5. If another model pushed overlapping changes, pull, merge, and resolve conflicts instead of overwriting their work.
6. Before pushing, reconcile split or conflicting edits so the repo contains a merged view of all useful work.
7. Never force-push or discard another model's valid work just to get a push through.
8. When a task item is done, push the latest state to GitHub.

The key rule is coordination, not overwrite. If Codex, Cursor, and Claude all work concurrently, each model should pull first, merge thoughtfully, and then push a combined result rather than replacing another model's updates.

## Human handoff

Models should leave short human-readable notes in `humans/` when they complete meaningful work or need to preserve session context for a person.

Use the naming pattern `humans/YYYY-MM-DD-model-task.md`.

Examples:
- what task was completed
- what changed
- what still needs attention
- open questions or risks
- links or paths to the relevant notes

If Codex finishes a task, it should add a note for the human with the task name and key details. The same pattern applies to Claude, Cursor, Kimi, and other models.

## Recommended workflow

1. Start with a clean working tree and sync the latest remote state.
2. Review the current repo contents so you are building on the newest task state.
3. Use Relern to fetch live course context.
4. Save useful summaries and outputs here.
5. Keep official facts linked back to their source course object.
6. Add a human handoff note in `humans/` when appropriate.
7. Commit your work locally.
8. Fetch the latest remote state again before pushing.
9. If remote changes appeared, merge or rebase carefully and resolve conflicts without dropping useful work from other agents.
10. Push only after local work and remote work are fully combined.

See `prompts/agent-checklist.md` for the operational checklist agents should follow.

## Folder layout

- `courses/`: per-course working notes
- `notes/`: general study notes and quick captures
- `planner/`: planning artifacts and upcoming work summaries
- `memory/`: durable context across sessions
- `drafts/`: unfinished outputs
- `prompts/`: reusable prompts and operating instructions
- `humans/`: model-to-human status notes, task handoffs, and session summaries

## Important rule

If there is a conflict between this repo and live data from Relern/Canvas, trust Relern/Canvas.
