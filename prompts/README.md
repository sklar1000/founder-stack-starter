# Prompt Library

Battle-tested prompts for the hard parts of building a startup — customer interviews,
market segmentation, riskiest assumptions, pretotypes, go-to-market. Adapted from the
**New Enterprises** course at Rice (MGMT 621) and wired to *your* stack.

These aren't generic. Each one reads the real files in your repo (`customers/`, `strategy/`)
and updates them — so the output is about *your* venture, not a hypothetical.

---

## How to use a prompt

**In Claude Code** (recommended): just say what you want — *"run the interview coach,"*
*"analyze my interviews,"* *"help me pick a beachhead."* Claude opens the prompt, reads your
files, and runs it. No copy-paste.

**In ChatGPT / Claude.ai**: open the prompt file, copy everything below the `---` line, and
paste your own content where it says `[paste …]`.

---

## The library, by stage

Your venture moves through four stages. Pull the prompt that matches where you are.
**★ = start here** (the three most first-timers need first).

### 1 · Discover — understand the problem
| Prompt | Use it when | Touches |
|--------|-------------|---------|
| ★ `discover/interview-coach.md` | Before your first real interview — practice on a simulated customer | `team/`, `strategy/beachhead.md` |
| ★ `discover/analyze-interviews.md` | After a batch of interviews — find themes, contradictions, the 4 buckets | reads `customers/`, writes `strategy/` |

### 2 · Define — narrow your target
| Prompt | Use it when | Touches |
|--------|-------------|---------|
| ★ `define/segment-and-beachhead.md` | You have interview signal and need to pick ONE segment to win first | writes `strategy/segments,beachhead,personas` |
| `define/jobs-to-be-done.md` | To understand what customers are really "hiring" a solution for | writes `strategy/jobs-to-be-done.md` |

### 3 · Decide — design the solution
| Prompt | Use it when | Touches |
|--------|-------------|---------|
| `decide/solution-to-mvbp.md` | Problem is validated — generate solutions, narrow to a minimum viable business proposal | writes `product/`, `strategy/` |
| ★ `decide/riskiest-assumptions.md` | To surface what must be true, rank by risk × uncertainty, and sharpen into testable hypotheses | writes `strategy/assumptions.md` |
| `decide/interrogate-thesis.md` | To stress-test your thesis the way a skeptical investor would (4 adversarial moves) | reads everything |

### 4 · Deploy — test and decide
| Prompt | Use it when | Touches |
|--------|-------------|---------|
| `deploy/design-pretotype.md` | To design the cheapest experiment that tests your #1 assumption — then read the results | writes `experiments/` |
| `deploy/gtm-map.md` | To map your venture against 30 go-to-market motions and pick the top 3 | writes `product/decisions/` |
| `deploy/pitch-coach.md` | To sharpen your positioning + executive summary before you pitch | reads `strategy/` |

---

## How this relates to the two commands

You already have two slash commands for the **daily loop**:
- `/interview-debrief` — quick: turn one interview into strategy updates (run after *every* call)
- `/update-assumptions` — quick: re-rank your assumptions from the latest evidence

The prompts above are the **deeper, episodic tools** — you reach for them once per stage, not
every day. The commands keep your stack current; the prompts move you to the next stage.

---

## The golden rule (from the NE course)

> **AI proposes, customer evidence decides.** Don't ask AI to do something until you have
> enough real data to feed it. More interviews in = better output out. If AI lands on the same
> answer you did, that's a signal your discovery is on track — not permission to skip the work.

---

*Adapted from `NE-Canon/08-ai-prompts/` and `12-foundation-wiki/` — Michael Sklar, Rice University.*
