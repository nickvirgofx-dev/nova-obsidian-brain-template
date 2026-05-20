---
title: Ingestion Rules
tags:
  - ingestion/rules
status: active
updated: <TODAY>
---

# Ingestion Rules

## Atomization Rule

When raw input is placed in `raw/`, process it into clean, small, cross-linked Markdown files in `wiki/`.

## Token-Budget Rule

Do not scan the entire `raw/` or `wiki/` directories.

Read `index.md` first and open only targeted files.

## Evidence Rule

Keep source references and distinguish:

- verified facts;
- assumptions;
- decisions;
- stale items that need recheck.
