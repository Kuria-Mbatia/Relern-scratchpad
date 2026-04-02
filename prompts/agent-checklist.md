# Agent Checklist

Use this checklist before, during, and after each task.

## 1. Sync First

1. Confirm you are in the correct repository.
2. Fetch the latest remote state.
3. Pull the latest `main` state before starting work when your tree is clean.
4. Read the latest relevant notes so you are not building on stale task data.

## 2. Do the Work

1. Use Relern or Canvas for live academic context.
2. Update the correct working files in this repo.
3. Prefer clearly scoped edits and new handoff files when possible to reduce conflicts.

## 3. Leave a Human Handoff

1. If you completed meaningful work, add a note in `humans/`.
2. Use the template `humans/YYYY-MM-DD-model-task.md`.
3. Record what you changed, what you checked, and anything still open.

## 4. Prepare to Push

1. Review your local diff.
2. Commit your changes locally.
3. Fetch remote changes again right before pushing.
4. If the remote moved, merge or rebase and resolve conflicts carefully.
5. Never force-push just to bypass another agent's work.

## 5. Push Safely

1. Push only when your local branch includes both your work and the latest remote work.
2. If the push is rejected, sync again, resolve conflicts, and retry.
3. The final pushed state should preserve useful work from all agents, not just your own changes.
