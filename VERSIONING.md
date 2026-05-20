# Versioning

Use semantic versions:

```text
MAJOR.MINOR.PATCH
```

Draft releases may use:

```text
0.1.0-draft
```

## Current Line

```text
0.1.x: public-safe Obsidian brain starter vault
```

Current draft:

```text
0.1.1-draft: public README/quickstart polish after initial publication
```

## Upgrade Rule

When the template changes, update:

1. `VERSIONING.md`
2. `CHANGELOG.md`
3. affected files under `vault-template/`
4. affected docs under `docs/`
5. `safety/PUBLIC_EXPORT_SCRUB_REPORT.md` before release

Do not publish private memory, runtime logs, machine-specific paths, account material, or secrets as part of any version update.
