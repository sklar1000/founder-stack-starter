# Build Your Team Co-Pilot — an AI that knows your whole team

Instructions to build a **Custom GPT (ChatGPT) or Project (Claude)** that knows each founder —
your personalities, experience, and roles — and helps you *navigate working together*: divide
labor by strength, cover each other's blind spots, translate communication styles, make
decisions, and handle friction before it festers.

> Founding teams rarely fail on talent. They fail on **ambiguity and friction** — who owns what,
> why two people keep clashing, what nobody's saying. A co-pilot that knows everyone's wiring is
> a neutral third party you can ask *"who should take this?"* / *"why do we keep getting stuck?"*
> / *"what am I not seeing?"*

**You already have most of the inputs** — they're in your `team/[name].md` files and `team/roles.md`.

*(In Claude Code you can already just ask Claude — it reads `team/`. But a standalone GPT/Project
is **shareable** — every teammate uses the same one — and works outside this repo. Build it once,
all of you use it.)*

---

## Step 1 — Gather the inputs (one block per founder)

For each person on the team, pull together (most is already written in `team/`):
- **PrinciplesYou** results — top archetypes + 2-3 standout scales. (Any profile works: CliftonStrengths, DISC, Enneagram.)
- **Resume / LinkedIn** — paste 3-5 highlights.
- **Role + what they own** — from `team/roles.md`.
- **Strengths + blind spots** — the ones you each named in your profile.

## Step 2 — Create the co-pilot

**Claude Project** (recommended — you're already in the Claude world):
1. claude.ai → **Projects** → **New Project**, name it "Team Co-Pilot."
2. Paste the system prompt below into **Project instructions**.
3. Add each member's profile (and PrinciplesYou PDF) as **Project knowledge**.

**ChatGPT Custom GPT:**
1. ChatGPT → **Explore GPTs** → **Create**.
2. Paste the system prompt into **Instructions**.
3. **Upload** each member's PrinciplesYou results + resume.

## Step 3 — The system prompt (copy this whole block)

```
# Team Co-Pilot — [Startup Name]

## Your role
You are our founding team's co-pilot. You know each of us — our personalities, experience,
and roles. Your job is to help us work together well: divide labor by strength, cover each
other's blind spots, navigate disagreements, make decisions, and communicate across our
different styles. You are a neutral third party who wants the TEAM to succeed — never any
single person over the others.

## Who we are
[Paste one block per founder:]
- Name + role:
- PrinciplesYou (top archetypes + standout traits):
- Experience (resume / LinkedIn highlights):
- Strengths:
- Blind spots:
- Working style (how they like to communicate / decide):

## How to help us
- When we ask "who should own X?", recommend based on strengths + role + current load — and say WHY.
- When two of us disagree or keep clashing, name the likely personality / working-style root
  (e.g., one is high-Structured and one improvises; one is direct and one seeks harmony) and
  suggest how EACH of us can flex. Be fair to both. Never take a side.
- When one of us has a blind spot relevant to a decision, gently flag it.
- Translate between styles: help a blunt founder and a harmony-seeking founder actually hear each other.
- When we're deciding something, ask who owns the call (per our roles), surface what each
  person's wiring would push them toward, then help us commit and move on.
- Be direct AND kind. We're a team under stress — tell us the truth, but assume good intent in each of us.

## How to respond
- Start by clarifying what we're really asking and who's involved.
- Ground every answer in our ACTUAL profiles above, not generic personality theory.
- Keep it short — we're builders.
- End with a concrete next step or a question that moves us forward.
```

## Step 4 — Ask it real things

- "We have to run a customer-interview push AND build the landing page this week. Who takes which, and why?"
- "[A] and [B] keep stalling on decisions together. What's going on, and how do we unstick it?"
- "I'm about to give [co-founder] some hard feedback. Given how they're wired, how should I frame it so they hear it?"
- "What's a blind spot our *whole team* shares that could bite us?"
- "We disagree about whether to pivot. Walk each of us through how our wiring is coloring this call."

## Keep it alive

Update it when roles change, someone retakes an assessment, or you add a teammate. Re-read it
right before a hard conversation — that's when it earns its keep.

---

## Advanced — make it a skill in your stack

If you're building in Claude Code (like this repo), you don't need a separate GPT at all — make
the co-pilot a **slash command** that reads your `team/` files live. **This Founder Stack already
ships one:**

- **`/team-copilot`** (`.claude/commands/team-copilot.md`) — reads `team/roles.md` + every
  `team/[name].md`, then answers the same team-navigation questions, grounded in your *current*
  profiles. No copy-paste, no re-uploading when someone updates theirs.

**To build your own** (the pattern for any system like this):
1. Create `.claude/commands/<name>.md` with a `description:` line and step-by-step instructions.
2. Make step 1 of the instructions *"read the files that hold the context"* (here, `team/`).
3. The rest is the behavior — the same rules as the system prompt above.
4. It runs as `/<name>` and always reads the latest files. **The skill is thin; the data is the asset.**

**Skill vs. standalone GPT — when to use which:**
- **Skill / command** (Claude Code): always-current (reads live files), nothing to re-upload — best for whoever is building *in* the repo.
- **Standalone GPT / Claude Project**: shareable with teammates who don't use Claude Code, works anywhere — but you re-paste profiles when they change.

Build both if you want — same brain, two front doors.

---

*Adapted from the New Enterprises "load your resume + PrinciplesYou, then ask" GPT pattern
(Rice MGMT 621), extended from the individual to the whole founding team. The goal isn't to let
AI decide for you — it's a neutral mirror that helps you see each other clearly and move faster.*
