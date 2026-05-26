# Public Export Scrub Report

Date: 2026-05-26

Scope: public-safe repository draft after Nova v1.8 template alignment.

Status: local scrub passed for v0.2.0-draft preparation; public push/release still blocked until exact user approval.

## Current Boundary

The repository has been published as a public-safe draft. This v0.2.0-draft update is local-only until the owner explicitly approves the exact push.

No release tag, package publication, deployment, account/auth/payment/secret action, MCP registration, hook/global config activation, database/index migration, OS repair action, or private memory export has been performed for this update.

## Required File Check

Required files were present:

```text
README.md
AGENTS.md
LICENSE
VERSIONING.md
CHANGELOG.md
docs/SETUP.md
docs/OPERATING_MODEL.md
docs/PUBLICATION_GUIDE.md
safety/RISK_GATES.md
safety/PUBLIC_EXPORT_SCRUB_CHECKLIST.md
safety/PUBLIC_EXPORT_SCRUB_REPORT.md
vault-template/01_AGENT_START_HERE.md
vault-template/_INDEX.md
vault-template/PROJECT_INTAKE_ROUTER.md
vault-template/03_ACTIVE_PROJECTS.md
vault-template/30_SYSTEMS/NOVA_SERIOUS_WORKFLOW.md
vault-template/50_TASKS/AGENT_WORK_LOG.md
vault-template/50_TASKS/INGESTION/index.md
examples/FIRST_AGENT_PROMPT.md
```

## 2026-05-26 v0.2.0-draft Changes

- Added context contract guidance.
- Added Goal/Rider task shape.
- Added adaptive clarification guidance.
- Added action verdict vocabulary: `allow`, `warn`, `review`, `block`.
- Added retry budget guidance for repeated same-root-cause failures.
- Expanded stop rules for public push, MCP registration, hooks, global config changes, and database/index migrations.

## Privacy And Secret Scan

All targeted patterns returned zero matches in tracked file content:

```text
private email: 0
private local path: 0
private user path: 0
private vault folder name: 0
private runtime folder name: 0
private project name pattern A: 0
private project name pattern B: 0
private project name pattern C: 0
OpenAI-style secret token pattern: 0
API key assignment pattern: 0
password assignment pattern: 0
token assignment pattern: 0
```

2026-05-26 local verification:

```text
git diff --check: PASS with LF/CRLF warnings only
private path scan: 0 matches for the private local path markers listed in the scrub checklist
credential-shaped scan: 0 matches for long OpenAI/GitHub/Slack/AWS/Google key shapes or assignment-shaped password/token/api key/secret values
risk-word scan: matches are in stop rules, release gates, scrub report text, or safety wording
cross-agent smoke review: PASS by static review for AGENTS.md, README.md, and vault-template/30_SYSTEMS/NOVA_SERIOUS_WORKFLOW.md
```

Note: a whole-folder scan can match Git sample-hook text inside `.git/`; the public content scan above uses tracked repository files.

## Remaining Push / Release Gate

Before pushing this v0.2.0-draft update or creating any release:

- review the final local diff;
- confirm the target GitHub repository and branch;
- run the scrub checklist again in the same work session;
- explicitly approve the exact push action;
- do not tag a release, publish a package, deploy, or export private memory without separate explicit approval.
