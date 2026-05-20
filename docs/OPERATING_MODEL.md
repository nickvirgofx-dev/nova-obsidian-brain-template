# Operating Model

## Six Layers

### 1. Brain / Context

Use the smallest useful context before acting.

Read:

- `01_AGENT_START_HERE.md`
- `_INDEX.md`
- the relevant project `CURRENT_STATE.md`
- the relevant project `TASK_BOARD.md`

### 2. Ingestion / Knowledge

Raw sources go into `50_TASKS/INGESTION/raw/`.

Processed notes go into `50_TASKS/INGESTION/wiki/`.

Read `50_TASKS/INGESTION/index.md` before opening raw or wiki folders.

### 3. Planning / Spec

For large repo/product/game work, create only the planning files that help:

- `PRD.md`
- `SPEC.md`
- `ARCHITECTURE.md`
- `AGENTS.md`
- acceptance criteria

Tiny safe tasks can use a short checklist.

### 4. Task Board / Checklist

Use explicit task IDs such as `T001`.

Each task should include:

- goal
- done condition
- verification
- risk
- recommended intelligence level

### 5. Verification / Risk Gate

Match verification to the task.

Examples:

- docs: targeted text check
- code: test, lint, build, smoke check
- UI/game: runtime or browser proof
- memory: index, retrieval, or audit check
- public repo: privacy and secret scan

### 6. Delivery + Sync Back

When GitHub delivery is in scope, use:

- issue
- branch
- pull request
- review/fix
- merge

After completion, sync:

- result
- decision
- lesson
- bug pattern
- next task
- status/dashboard update

## Compact Path For Small Tasks

For low-risk metadata or docs tasks:

1. read the task;
2. archive first if editing memory;
3. make the smallest change;
4. verify;
5. update checklist and work log.
