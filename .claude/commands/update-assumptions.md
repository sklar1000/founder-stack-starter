---
description: Re-rank riskiest assumptions from all evidence, pick the next test
---

Step back and re-rank the whole assumption list against everything you've learned. Run this
after a batch of interviews or experiments — weekly is a good rhythm.

## Steps

### 1. Read the evidence

- All files in `customers/interviews/`
- `customers/debriefs.md`
- Any results in `experiments/`

### 2. Re-rank `strategy/assumptions.md`

For each assumption:
- Update **Confidence** based on what the evidence now says.
- Update **Status** (⬜ untested → 🔴 testing → ✅ validated → ❌ killed).
- Update the **Evidence** column with the interview/experiment that moved it.
- Re-sort by **risk × uncertainty** (highest first).

Surface any **new** assumptions the recent evidence revealed — these are often the most
dangerous, because you didn't know to list them before.

### 3. Pick the next test

Name the single highest risk × uncertainty assumption that's still unresolved. Propose the
**cheapest experiment** that could prove it wrong, and offer to stub an `experiments/` card
for it from `experiments/_TEMPLATE.md`.

### 4. Confirm, then write

Show the re-ranked table as a before/after. Ask "Apply? [Y/edit/n]". Write only on confirm.

## The discipline

If most assumptions are still ⬜ untested after weeks of work, say so directly — it means
we're building or theorizing instead of testing. The point of this file is to keep us
honest about what we actually know vs. what we hope.
