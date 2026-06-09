---
description: Smart git commit with auto-generated message
---

Create a clean git commit.

## If I provide a message

`/commit fix: typo in beachhead`  → use it directly:

```bash
git add .
git commit -m "fix: typo in beachhead"
```

## If no message

1. Check what changed:

```bash
git status
git diff --stat
```

2. Propose a message:

```
[type]: [short description]
- [change 1]
- [change 2]
```

3. Ask: "Commit with this? [Y/edit/n]"
4. On confirm, commit.

## Commit types

`feat:` new content/feature · `fix:` correction · `docs:` docs only · `chore:` maintenance · `refactor:` restructuring

## Rules

- Never force push.
- **Warn loudly** if `team/` profiles, `.env`, or anything with personal data (PrinciplesYou
  scores, etc.) is staged — confirm I actually want that in the history, especially if the
  repo is public.
- After commit, offer to push if a remote is configured.
