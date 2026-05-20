# Nova Obsidian Brain Template

A public-safe starter vault for building a Nova-like Obsidian central brain for AI agents.

Status: local draft v0.1.0-draft. This repository is not published until the owner explicitly creates/pushes a GitHub repo.

## What This Is

This template helps you create a central memory workspace where AI agents can:

- find the right project context quickly;
- keep task boards and checklists readable;
- preserve work before cleanup;
- separate raw sources from processed knowledge;
- stop before risky actions;
- sync completed work back into Obsidian notes.

It is designed for Codex, Claude Code, and similar coding agents that can read and edit local Markdown files.

## What This Is Not

This is not a full copy of anyone's private vault.

It does not include private project notes, runtime logs, secrets, API keys, account automation, OS repair automation, or deployment automation.

## Quick Start

1. Copy `vault-template/` to your own Obsidian vault location.
2. Rename the copied folder to your preferred vault name.
3. Open the copied folder in Obsidian.
4. Read `01_AGENT_START_HERE.md`.
5. Replace placeholder values such as `<VAULT_ROOT>`, `<RUNTIME_ROOT>`, `<PROJECT_NAME>`, and `<TODAY>`.
6. Give your agent the instruction from `AGENTS.md`.

Recommended local layout:

```text
your-workspace/
  obsidian-brain/
  agent-runtime/
```

Keep generated runtime files, external clones, logs, screenshots, caches, and temporary outputs outside the Obsidian vault.

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

## Safety Boundary

Agents should stop before:

- hard delete;
- broad stable-memory rewrite;
- installing unreviewed tools;
- deployment;
- account, auth, payment, or secret handling;
- browser account actions;
- OS repair;
- autonomous recurring edits beyond the user's exact request.

Before publishing your own fork, run `safety/PUBLIC_EXPORT_SCRUB_CHECKLIST.md`.
