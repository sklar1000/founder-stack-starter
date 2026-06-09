# Analyze Interviews — turn a stack of conversations into real signal

**Stage**: Discover · **Adapted from**: NE-Canon `/ne-analyze-transcripts` + Fieldwork-Debrief (4 Buckets)
**Use it when**: after a batch of ~5 interviews — to find what's actually there before you decide anything
**Reads**: all files in `customers/interviews/` · **Writes**: proposes updates to `strategy/` + `customers/debriefs.md`

**In Claude Code**: say *"analyze my interviews"* — Claude reads `customers/interviews/` directly.
**In ChatGPT/Claude.ai**: paste your interview notes/transcripts where marked. (Minimum 5.)

> This is the deeper, batch version of `/interview-debrief` (which handles one interview at a time).
> Run this when you've accumulated several and want the cross-interview picture.

---

You are a customer-discovery analyst. Read every interview in `customers/interviews/` (or
`[paste interviews here]`). Be rigorous and honest — your job is to find the truth, not to make
the founder feel good. **Preserve the customer's exact words; never paraphrase a quote. Count,
don't vibe** ("6 of 8 mentioned X unprompted" beats "several mentioned X").

Produce:

## 1. Themes (5-8)
For each: a name, how many interviews it appears in, 2-3 verbatim quotes, and the nuance.

## 2. Contradiction map
Where interviewees *disagree*. Do NOT resolve these — contradictions usually mark a boundary
between two different segments. Name both sides.

## 3. Surprises
Pain points, workarounds, or stakeholders you didn't expect. These are often the most valuable
findings.

## 4. Customer language glossary
The actual words/phrases they use for the problem. (You'll reuse these verbatim in your
positioning — see `prompts/deploy/pitch-coach.md`.)

## 5. Behavioral evidence (SAY vs. DO)
Separate what they *said* they want from what they actually *do* today. Flag every gap — stated
preference is weak; behavior is strong. Flag Mom Test violations (polite agreement with no real
pain behind it).

## 6. Evidence strength
A short table rating: sample size, depth, behavioral evidence, pain severity. Be blunt about
where it's thin.

## 7. The diagnosis — which bucket?
Sort the batch into one (or more) of the Fieldwork-Debrief buckets:
- **A — Interviews worked.** You learned something real. → Trust it; revise your problem statement.
- **B — Process problem.** Wrong people, leading questions, survivor bias, firehose conversations. → Fix the method, not the market.
- **C — Market signal.** Everyone agrees it's a problem but nobody fixes it; the "pain" is part of what they enjoy; willingness-to-pay exists but not for your solution type. → Often the most valuable finding. Consider pivot / narrow / reframe.
- **D — Need more data.** Can't tell yet. → Name the ONE question the next 5 interviews must answer.

## 8. Proposed strategy updates
Based on the above, propose specific edits (show before/after, write only on confirmation):
- `strategy/assumptions.md` — status/confidence changes + new assumptions surfaced
- `strategy/personas.md` — sharpen with real quotes
- `strategy/segments.md` / `beachhead.md` — does the evidence strengthen or weaken the pick?
- `customers/debriefs.md` — append the pattern summary

---

End with the single most important thing the founder should do next — one interview question to
chase, one assumption to test, or one decision to make.
