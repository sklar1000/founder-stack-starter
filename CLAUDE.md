# CLAUDE.md — [STARTUP NAME]

This file is the brain of your startup's stack. Claude reads it at the start of every
session, so you never have to re-explain who you are or what you're working on.

**Fill in every `[BRACKET]`. Delete this italic note when you're done.**
*Keep it short — a page is plenty. Update it as reality changes; it's a living file, not a monument.*

---

## Our Team

See `team/` for full profiles. One line each:

- **[Name]** — [role, e.g. CEO / customer discovery] · [one strength, e.g. "relentless on follow-ups"]
- **[Name]** — [role, e.g. CTO / build] · [one strength]

(Solo? One line is fine. Claude uses this to tailor advice to each person and flag blind spots.)

---

## What We're Building

**One sentence**: [who it's for] + [the problem] + [why now].

**Stage**: [ pre-idea / discovery / validating / building ]
*(discovery = still interviewing customers · validating = testing riskiest assumptions · building = have signal, making the thing)*

---

## What We're Testing Right Now

Our top riskiest assumptions (full list + ranking in `strategy/assumptions.md`):

1. [Assumption] — testing via [how]
2. [Assumption] — [status]
3. [Assumption] — [status]

> If you can't fill this in, that's the most important thing you learned today.
> Open `strategy/assumptions.md` and start there.

---

## Customer

- **Beachhead** (the one segment we're winning first): see `strategy/beachhead.md`
- **Who they are**: see `strategy/personas.md`

---

## Working On

Current priorities live in `workboard.md` (this week's max-3 + next actions).

---

## Rules for Claude

**Do**
1. Read this file at the start of every session.
2. Lead with the answer, then the reasoning. We're builders, not readers.
3. After a customer conversation, remind me to run `/interview-debrief`.
4. Tailor advice to each founder's profile in `team/` — play to strengths, cover blind spots.
5. When I'm stuck on a startup step (interviews, segments, assumptions, pretotype, GTM, pitch), check `prompts/` for the matching guide and offer to run it.
6. When I finish work, remind me to `/commit`.

**Don't**
1. Don't create new folders without asking.
2. Don't add features or scope I didn't ask for.
3. Don't sugarcoat — if the evidence is thin, say so.
4. Don't let me confuse "busy building" with "learning." If I haven't talked to a customer this week, say it.

---

## Slash Commands

| Command | What it does |
|---------|--------------|
| `/start-session` | Load context, show what to work on |
| `/end-session` | Document progress, commit, hand off to next time |
| `/commit` | Clean git commit |
| `/interview-debrief` | Turn a customer conversation into updated strategy |
| `/update-assumptions` | Re-rank riskiest assumptions from the latest evidence |

---

**Last updated**: [DATE]
