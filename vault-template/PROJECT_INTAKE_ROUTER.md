---
title: Project Intake Router
tags:
  - brain/router
status: active
updated: <TODAY>
---

# Project Intake Router

Use this before creating a new project folder.

## Intake Questions

```text
project_name:
goal:
type: docs | code | game | research | automation | business | other
deadline:
risk_level: low | medium | high
runtime_location:
github_repo:
```

## Routing Rules

- Existing ongoing work goes under `10_PROJECTS/<PROJECT_NAME>/`.
- Raw source material goes under `50_TASKS/INGESTION/raw/`.
- Processed knowledge goes under `50_TASKS/INGESTION/wiki/`.
- External clones, generated reports, screenshots, logs, and caches go under `<RUNTIME_ROOT>`.

## Minimum Serious Project Files

```text
README.md
CURRENT_STATE.md
TASK_BOARD.md
TASK_CHECKLIST.md
DECISION_LOG.md
HANDOFF.md
```

Use `30_SYSTEMS/TEMPLATES/PROJECT/` as the starting shape.
