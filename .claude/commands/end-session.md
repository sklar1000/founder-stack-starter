---
description: Close the session — document, update the board, commit
---

Wrap up. Document what happened, update the board, commit.

## Steps

### 1. Summarize

```
SESSION SUMMARY
Worked on: [what]
COMPLETED: [what got done]
IN PROGRESS: [what remains]
FILES CHANGED: [list]
```

### 2. Update the living files

- Move finished items to `## Done` in `workboard.md`.
- If I learned something about a customer or assumption, remind me to update `strategy/` (or offer to do it).
- Update the "Last updated" date in `CLAUDE.md` if it changed.

### 3. Commit

```bash
git status
git diff --stat
```

Propose a commit message, ask me to confirm, then commit. Warn me if any personal files
(`team/` profiles, anything with PrinciplesYou data) are about to be committed to a repo
that might be public.

### 4. Handoff

```
NEXT SESSION
Priority: [the one thing to do next]
Context: [key thing to remember]
Resume with: /start-session
```

### 5. Offer push

If a git remote is set, ask: "Push? (y/n)"
