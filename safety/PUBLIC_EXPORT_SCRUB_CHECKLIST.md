# Public Export Scrub Checklist

Run before publishing.

## Must Be Zero

- real personal email
- private local path
- private project name
- API key or token
- password
- raw log
- private chat transcript
- account identifier
- deployment target
- payment data

## Content Review

- Examples are synthetic.
- Paths use placeholders.
- Risky actions are written as stop rules, not permissions.
- Runtime outputs are excluded.
- Obsidian local workspace files are excluded.

## Suggested Checks

Search the repo content for:

```text
email addresses
drive paths
usernames
api keys
tokens
password
secret
private project names
```
