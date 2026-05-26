---
title: Nova Serious Workflow
tags:
  - system/workflow
status: active
updated: <TODAY>
---

# Nova Serious Workflow

Use this for serious work that needs context, tasks, verification, safe delivery, and sync-back.

## Context Contract

Before meaningful edits, state:

```text
user_goal:
project:
primary_state_files:
exact_source_files:
runtime_or_repo_evidence:
verification_target:
excluded_context:
stop_rules:
```

Use the smallest useful context. Do not scan the whole vault when indexes, current state, board, checklist, or handoff are enough.

## Six-Layer Stack

1. Brain / Context
2. Ingestion / Knowledge
3. Planning / Spec
4. Task Board / Checklist
5. Verification / Risk Gate
6. Delivery + Sync Back

Small tasks can use a compact path. Large repo or game tasks should use more of the stack.

## Task Rule

Every serious task should have:

- task ID;
- Goal;
- Rider;
- Done when;
- Verification;
- Stop rule;
- Recommended intelligence;
- final result.

## Action Verdicts

Before meaningful actions, use one verdict:

```text
allow: in scope, low risk, reversible, or already approved
warn: bounded but noisy; state risk and verification first
review: ambiguous, broad, or user-impacting; ask or narrow first
block: not approved; do not execute
```

If the same root cause fails twice, stop and report the exact command/action, error, evidence checked, and next safer check.

## Stop Rules

Stop before:

- hard delete;
- broad rewrite;
- deploy;
- account/auth/payment/secret work;
- OS repair;
- browser account actions;
- public push;
- MCP registration, hooks, global config changes;
- database/index migrations;
- risky recurring automation.

## Handoff Shape

```text
completed:
files changed:
task updated:
intelligence used:
verification:
not tested:
risks:
next:
```
