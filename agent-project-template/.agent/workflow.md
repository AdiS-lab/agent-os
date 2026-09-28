# workflow.md

How an agent should run a task in this repo.

## Start

1. Read `AGENTS.md`.
2. Read `.agent/context.md`.
3. Read `TASK.md`. If status is `done`, stop and wait for a new task.
4. If the task needs product or stack context, read `PROJECT.md`.
5. If the change might conflict with prior choices, read `DECISIONS.md`.
6. Set `TASK.md` status to `in_progress` and write a short plan if it is empty.

## Implement

1. Change only what the task requires.
2. Prefer existing patterns in the repo over new abstractions.
3. After each meaningful step, update `TASK.md` notes (what changed, what remains).
4. If you discover a durable design choice, append an entry to `DECISIONS.md`.
5. If blocked, set status to `blocked`, write the blocker, and stop.

## Finish

1. Follow `.agent/verification.md`.
2. Update acceptance criteria checkboxes in `TASK.md`.
3. Write verification commands and results in `TASK.md`.
4. Set status to `done` only if verification passed and criteria are met.
5. Summarize the outcome for the human: what changed, how to verify, what was left out.
