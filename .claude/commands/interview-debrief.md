---
description: Turn a customer conversation into updated strategy
---

This is the most important command in the stack. It runs the loop the whole system exists
for: **a customer told you something → your strategy updates to reflect it.**

Run it right after a customer conversation (once the notes are saved).

## Steps

### 1. Find the interview

Read the newest file in `customers/interviews/` (or the one I name). If notes are still in
my head or in `inbox.md`, help me get them into a proper interview file first, using
`customers/interviews/_TEMPLATE.md`.

### 2. Extract the signal

Pull out, quoting verbatim where possible:
- **Pains** — what hurts, in their words
- **The job** they're trying to get done (functional / emotional / social)
- **Segment signals** — which segment they belong to; does it strengthen or weaken our beachhead?
- **Current workaround** — what they do today
- **Surprises** — anything that contradicts what we believed
- **Buying signals** — did they ask to keep talking, try it, pay, or refer someone?

### 3. Propose updates (don't write yet)

Based on the signal, propose specific edits to:
- **`strategy/assumptions.md`** — change a status (⬜→🔴→✅/❌) or confidence; add this interview as evidence; flag any *new* assumption this surfaced.
- **`strategy/personas.md`** — sharpen with a real quote, or flag where reality diverges from the persona.
- **`strategy/beachhead.md`** — does this support or weaken the beachhead pick?
- **`customers/debriefs.md`** — append a one-line pattern entry (and note if this makes 3+ on the same theme).

Show the proposed edits as a clear before/after diff.

### 4. Confirm, then write

Ask: "Apply these updates? [Y/edit/n]". Only write on confirmation.

### 5. Close the loop

If this interview *killed or validated* a top assumption, say so plainly — that's a real
result. Suggest the next assumption to test, and whether it's worth an `experiments/` card.

## Tone

Be honest. If the interview was thin (I pitched instead of listened, or it was a friend
being nice), tell me — a polite non-signal is worse than a clear no.
