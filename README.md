# Nova Obsidian Brain Template

A public-safe starter vault for building a Nova-like Obsidian central brain for AI agents.

Status: public-safe draft v0.2.0-draft prepared locally. This template is meant to be copied, renamed, and adapted before real use.

## What This Is

This template helps you create a central memory workspace where AI agents can:

- find the right project context quickly;
- keep task boards and checklists readable;
- preserve work before cleanup;
- separate raw sources from processed knowledge;
- stop before risky actions;
- ask the right amount of clarification for task size/risk;
- use a compact context contract before meaningful edits;
- frame serious work with Goal and Rider;
- classify meaningful actions as allow/warn/review/block;
- sync completed work back into Obsidian notes.

It is designed for Codex, Claude Code, and similar coding agents that can read and edit local Markdown files.

## What This Is Not

This is not a full copy of anyone's private vault.

It does not include private project notes, runtime logs, secrets, API keys, account automation, OS repair automation, or deployment automation.

## Quick Start

### Use In 5 Minutes

1. Copy `vault-template/` to your own Obsidian vault location.
2. Rename the copied folder to your preferred vault name.
3. Open the copied folder in Obsidian.
4. Read `01_AGENT_START_HERE.md`.
5. Replace placeholder values such as `<VAULT_ROOT>`, `<RUNTIME_ROOT>`, `<PROJECT_NAME>`, and `<TODAY>`.
6. Give your agent the instruction from `AGENTS.md`.
7. Create your first project through `PROJECT_INTAKE_ROUTER.md` instead of dropping notes into the vault root.

Recommended local layout:

```text
your-workspace/
  obsidian-brain/
  agent-runtime/
```

Keep generated runtime files, external clones, logs, screenshots, caches, and temporary outputs outside the Obsidian vault.

## First Agent Prompt

Paste this into Codex, Claude Code, or another local coding agent after you copy the template:

```text
Use this Obsidian vault as my AI agent brain.
Read AGENTS.md first, then 01_AGENT_START_HERE.md.
Do not scan every file. Open only the files needed for my current task.
Do not delete or overwrite memory. Archive or propose cleanup first.
Create or update project notes, task boards, checklists, decisions, and handoffs using the template rules.
Stop before secrets, accounts, payments, deploys, OS repair, or broad memory rewrites.
```

## What You Get

- a small Obsidian vault skeleton;
- project routing and active-project indexes;
- task board, checklist, current-state, decision-log, and handoff templates;
- raw-to-wiki ingestion space;
- concise work-log structure;
- risk gates for public/private boundaries;
- synthetic examples that do not include private memory.

## Repository Layout

```text
vault-template/          reusable Obsidian vault skeleton
docs/                    setup and operating guides
safety/                  public-safe risk gates and scrub checklist
examples/                synthetic examples only
CHANGELOG.md             version history
VERSIONING.md            version rules
AGENTS.md                agent bootstrap instruction
LICENSE                  MIT license
```

## Core Idea

The brain has six practical layers:

1. Brain / Context
2. Ingestion / Knowledge
3. Planning / Spec
4. Task Board / Checklist
5. Verification / Risk Gate
6. Delivery + Sync Back

Small tasks can use a compact path. Large repo or game tasks should use more of the stack.

For serious work, use the v1.8 task shape:

```text
Goal:
Rider:
Done when:
Verification:
Stop rule:
Recommended intelligence:
```

Before meaningful edits, ask the agent to state a compact context contract:

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

## Safety Boundary

Agents should stop before:

- hard delete;
- broad stable-memory rewrite;
- installing unreviewed tools;
- deployment;
- account, auth, payment, or secret handling;
- browser account actions;
- OS repair;
- MCP registration, hooks, global config changes, or database/index migrations;
- autonomous recurring edits beyond the user's exact request.

Before publishing your own fork, run `safety/PUBLIC_EXPORT_SCRUB_CHECKLIST.md`.

## Good First Workflow

1. Put ideas and source material in the right project or `50_TASKS/INGESTION/raw/`.
2. Ask the agent to create one `T###` task with a checkbox, done condition, risk, and verification.
3. Let the agent work on one task at a time.
4. Require a short handoff after completion.
5. Run the scrub checklist before sharing anything publicly.
