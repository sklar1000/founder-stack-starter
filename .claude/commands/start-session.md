---
description: Load startup context and show what to work on
---

Load my context and show what to work on today.

## Steps

1. Get today's date.
2. Read `CLAUDE.md` — team, what we're building, what we're testing, the rules.
3. Read `team/` — so you know who you're working with and can tailor advice.
4. Read `workboard.md` (this week's priorities) and the top of `strategy/assumptions.md` (what we're testing).
5. Check recent git history:

```bash
git log --oneline -3 2>/dev/null || echo "No git history yet"
```

## Output Format

```
SESSION READY — [Day, Date]

TEAM:        [names + roles, one line]
BUILDING:    [one-sentence what + stage]
TESTING NOW: [top riskiest assumption from assumptions.md]

THIS WEEK:
  - [up to 3 from workboard.md]

RECENT:
  [last 3 commits, if any]

---
What's the focus today?
```

## After Startup

Wait for my answer, then help me with whatever I choose. If I haven't talked to a customer
this week (no new files in `customers/interviews/`), gently say so — discovery is the job.
