# Founder's Stack

A folder of markdown files that turns Claude Code into a co-founder who actually
remembers your startup — your customers, your assumptions, your decisions, your team.

**Intelligence is a commodity. Memory is the asset.**

Most founder tools are knowledge management — a place to put stuff. This is different.
It's built so one move pays off over and over: *talk to a customer → Claude updates your
whole strategy from what you heard.* The folders exist so that move works.

---

## What you need

- A computer + [Claude Code](https://claude.ai/code) installed (`curl -fsSL https://claude.ai/install.sh | bash`)
- Git
- 15 minutes
- A startup idea (even a rough one)

No Python. No database. No new app to learn. Just markdown in a folder.

---

## Quickstart (15 min)

```bash
# 1. Clone and make it yours
git clone [REPO-URL] my-startup
cd my-startup
rm -rf .git && git init        # start your own history

# 2. Open Claude Code
claude
```

Then, inside Claude:

1. **Fill in `CLAUDE.md`** — who you are, what you're building, what you're testing. (Claude can interview you: *"Help me fill in CLAUDE.md."*)
2. **Fill in `team/`** — one file per founder: major, experience, PrinciplesYou, strengths.
3. **Run `/start-session`** — Claude loads your context and shows what to work on.
4. **Run `/commit`** — your first breadcrumb in git history.

That's it. You have a co-founder with a memory.

---

## The map

Six layers. Same shape as a serious operator's vault, founder-sized:

| Layer | Where | What it holds |
|-------|-------|---------------|
| **Who we are** | `team/` | Per-founder profiles + roles |
| **Capture** | `inbox.md` | Dump anything here; sort it on Fridays |
| **What customers said** | `customers/` | Interview notes (raw evidence — never rewrite these) |
| **What we believe** | `strategy/` | Segments, beachhead, persona, **riskiest assumptions** (living — rewrite as you learn) |
| **What we're doing** | `workboard.md` + `experiments/` | This week's work + assumption tests |
| **What we decided** | `product/decisions/` | Why we chose X (so you don't relitigate it) |

The brain that ties it together is **`CLAUDE.md`** at the root.

---

## The one loop that matters

After every customer conversation:

1. Drop your notes in `customers/interviews/YYYY-MM-DD-name.md`
2. Run **`/interview-debrief`**
3. Claude reads what they said and proposes updates to your assumptions, persona, and beachhead.

Your strategy stops being a doc you wrote once and forgot. It becomes the running output
of every conversation you have.

---

## The prompt library

The hard parts of building a startup — running good interviews, picking a beachhead, finding
your riskiest assumption, designing a pretotype — each have a battle-tested prompt in
`prompts/`, organized by stage (Discover → Define → Decide → Deploy). They're adapted from the
**New Enterprises** course at Rice and wired to your files: each one reads `customers/` and
`strategy/` so the output is about *your* venture.

Stuck on a step? Just ask — *"run the interview coach,"* *"help me pick a beachhead,"*
*"surface my riskiest assumptions."* See `prompts/README.md` for the full index and which to
reach for when. Start with the three marked **★**.

---

## Don't over-build it

You're a developer. You will want to add tags, a database, a graph, seventeen folders.
**Don't.** The rule from the operator this is based on:

> *Question every requirement. Delete the step. If you don't end up putting back at least
> 10% of what you deleted, you didn't delete enough.*

Start with `CLAUDE.md` + `inbox.md` + `strategy/assumptions.md`. Add the rest when you
feel the friction, not before. The system grows with you.

---

*Based on the Personal Stack by [Michael Sklar](https://michaelsklar.ai) — and the
New Enterprises method taught at Rice: customers before code, evidence over opinion.*
