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

1. At the start of any task, pull the latest GitHub state before doing anything else.
2. Check the current latest notes, planner items, and task artifacts so you do not add updates to stale data.
3. Do your work locally in the appropriate workspace folders.
4. If another model pushed overlapping changes, pull, merge, and resolve conflicts instead of overwriting their work.
5. Before pushing, reconcile split or conflicting edits so the repo contains a merged view of all useful work.
6. When a task item is done, push the latest state to GitHub.

The key rule is coordination, not overwrite. If Codex, Cursor, and Claude all work concurrently, each model should pull first, merge thoughtfully, and then push a combined result rather than replacing another model's updates.

## Human handoff

Models should leave short human-readable notes in `humans/` when they complete meaningful work or need to preserve session context for a person.

Examples:
- what task was completed
- what changed
- what still needs attention
- open questions or risks
- links or paths to the relevant notes

If Codex finishes a task, it should add a note for the human with the task name and key details. The same pattern applies to Claude, Cursor, Kimi, and other models.

## Recommended workflow

1. Pull the latest repo state from GitHub.
2. Use Relern to fetch live course context.
3. Review the current repo contents so you are building on the newest task state.
4. Save useful summaries and outputs here.
5. Keep official facts linked back to their source course object.
6. Add a human handoff note in `humans/` when appropriate.
7. Pull again before pushing if needed, merge conflicts carefully, and then push the combined latest state.

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
