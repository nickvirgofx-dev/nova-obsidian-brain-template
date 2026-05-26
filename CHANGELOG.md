# Changelog

## 0.2.0-draft - 2026-05-26

Nova v1.8 template alignment.

Added:

- context contract guidance before meaningful edits;
- Goal/Rider task shape;
- adaptive clarification rule for small vs large/risky tasks;
- action verdict vocabulary: `allow`, `warn`, `review`, `block`;
- retry budget guidance for repeated same-root-cause failures;
- expanded stop rules for public push, MCP registration, hooks, global config changes, and database/index migrations;
- updated public-safe workflow template under `vault-template/30_SYSTEMS/NOVA_SERIOUS_WORKFLOW.md`.

Safety:

- no private vault export;
- no runtime logs;
- no private machine paths;
- no secrets;
- no account, deploy, payment, browser-account, MCP, hook, global config, database/index migration, or OS repair automation;
- no commit, push, release tag, package publication, deployment, or private memory export performed.

## 0.1.1-draft - 2026-05-20

Documentation polish after initial public publication.

Changed:

- updated README status from local-only draft wording to public-safe draft wording;
- added a five-minute quickstart;
- added a first-agent prompt;
- clarified what the template includes;
- added a good-first-workflow section for new users.

Safety:

- no private vault export;
- no runtime logs;
- no private machine paths;
- no secrets;
- no account, deploy, payment, browser-account, or OS repair automation;
- no release tag, package publication, deployment, or private memory export performed.

## 0.1.0-draft - 2026-05-20

Initial local draft.

Added:

- public-safe Obsidian vault skeleton
- agent bootstrap guidance
- project intake and active project indexes
- task board, checklist, current state, decision log, and handoff templates
- ingestion raw/wiki structure
- work log and inbox notes
- safety gates and scrub checklist
- synthetic project example

Safety:

- no private vault export
- no runtime logs
- no private machine paths
- no secrets
- no account, deploy, payment, browser-account, or OS repair automation
- no GitHub remote, push, publish, or release performed
