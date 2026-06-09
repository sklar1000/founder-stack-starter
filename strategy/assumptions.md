# Riskiest Assumptions

**This is the most important file in your stack.** Every startup is a stack of beliefs that
might be wrong. This is where you list them, rank them, and test the deadly ones *before*
they kill you.

> **New Enterprises method (Riskiest Assumption Testing):** List 20-30 assumptions your
> venture rests on. Rank by **risk × uncertainty** — how badly it hurts if you're wrong,
> times how unsure you are. Test the top 1-3 with the cheapest experiment that could prove
> you wrong. A killed assumption isn't failure — it's a $10K lesson you got for the price
> of a conversation.

This is a **living** file. Rewrite it as evidence comes in. Run `/update-assumptions`
after a batch of interviews to re-rank.

---

## The list

`Status`: ⬜ untested → 🔴 testing → ✅ validated → ❌ killed

| # | Assumption | Risk | Confidence | Status | Evidence |
|---|-----------|------|-----------|--------|----------|
| 1 | *(example)* Solo founders feel this pain at least weekly | HIGH | LOW | 🔴 testing | exp-001 |
| 2 | *(example)* They'll pay $30/mo to make it go away | HIGH | LOW | ⬜ untested | — |
| 3 | *(example)* We can reach them through founder Slack groups | MED | MED | ✅ validated | 4 interviews |
| 4 | *(replace these examples with your real assumptions)* | | | ⬜ | |

---

## What we're testing next

**[Assumption #__]** — because it's the highest risk × uncertainty and everything else
depends on it. Test: [the experiment]. Tracked in `experiments/`.

---

**Ask Claude:** *"Given my interviews in `customers/interviews/`, re-rank these by risk ×
uncertainty, update the status column based on what I've actually heard, and tell me the
single cheapest experiment to test my #1."*
