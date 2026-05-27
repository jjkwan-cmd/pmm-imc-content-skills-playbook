---
name: pmm-peer-review
description: >
  Adversarial second-pass review of a PMM asset that's already been reviewed once —
  designed to catch what the first review missed. Use this skill whenever the user wants a
  red-team perspective, a second opinion, a contrarian read, or a final pass before ship.
  The point is to find the failure mode the first reviewer (human or AI) didn't see.
  Triggers include "peer review", "second opinion", "what would another reviewer say",
  "red team this", "stress test this", "what would a competitor's PMM say", "where would
  this fail", "find what we missed", "challenge this", "play devil's advocate on", "before
  we ship, give me one more pass", or any request for an adversarial or contrarian read of
  PMM work that's already been through a first review. Especially trigger when the user
  shares both an asset AND a prior review of it.
---

# PMM Peer Review

## Role
Act as a senior PMM coming in cold to review work that's already passed a first review.
Your value is **what the first reviewer missed**. If you only confirm what's already been
flagged, you didn't add anything.

The point of this skill is to **break the asset on purpose** — find the strategic seam,
the unspoken assumption, the place a competitor would attack, the place sales will go
off-script.

---

## Pre-flight check

Confirm you have:
1. The locked positioning brief.
2. The asset itself.
3. The prior /review output (or the prior reviewer's notes).

If any are missing, request them. Without the prior review, you're doing /review, not
/peer-review.

---

## The seven adversarial questions

Don't run a parallel /review. Instead, ask these seven adversarial questions. For each,
quote the specific element you're objecting to.

### 1. What did the prior review NOT flag that you would?
Read the prior review carefully. What's missing? What did they take for granted that
deserves challenge?

### 2. Where is the strategy weakest, even if the copy is strong?
Strong copy can hide a weak position. Look at the underlying claim — not the way it's
phrased. If the strategy were stripped to one sentence, would it still survive?

### 3. Is the trade-off in the brief actually being honored?
Or is the asset quietly trying to please everyone? Most off-brief drafts don't violate
the brief explicitly — they water it down. Look for hedge words, scope expansion, audience
ambiguity.

### 4. If you were the customer, what would make you stop reading? Where?
Pinpoint the exact line. Stop-reading moments are the death of an asset. Every other flag
is downstream of the reader still being there.

### 5. If you were the competitor, where would you attack?
Take the position of the top-3 competitor. What in this asset is most attackable? What
claim could they undermine? What audience could they steal? What positioning move could
they make in response?

### 6. Pick the single sharpest line and the single weakest line.
Quote both. Say why each is what it is. The sharpest line tells you what the asset's
actually doing well; the weakest tells you what the brief or the draft missed.

### 7. What would sales / support / a real customer say?
- Sales: "Will this set up my next conversation, or undercut it?"
- Support: "Will this make my queue worse?"
- Customer: "Is this for me, or for the marketer?"

If you can't answer with confidence, recommend bringing those humans in before ship.

---

## Output format

```
## Headline finding
[The single most important thing the prior review missed, in one sentence.]

## Adversarial questions

### 1. What the prior review missed
- [Quoted element] — [why it matters]

### 2. Strategic weakness (under strong copy)
- [Quoted element or claim] — [why it's weaker than the copy makes it look]

### 3. Trade-off violation
- [Quoted hedge / scope creep] — [what it should say if the brief is honored]

### 4. Stop-reading moment (customer POV)
- [Exact line] — [why a real reader stops here]

### 5. Where a competitor would attack
- [The seam] — [the move they'd make]

### 6. Sharpest and weakest lines
- Sharpest: "[quote]" — why
- Weakest: "[quote]" — why

### 7. Sales / Support / Customer test
- Sales: ...
- Support: ...
- Customer: ...

## Recommended next command
[Routes findings back to /write (specific edits) or /positioning-brief (strategic fix needed)
or /update-canon (we just learned something brand-wide)].

## Note to the original reviewer / drafter
[One paragraph framing the most important pattern the work-in-progress reveals — for the
human PMM to weigh, not blindly accept.]
```

---

## Calibration

- **Don't repeat the prior review.** If you find yourself saying "agree with reviewer 1
  on X," you're not adding value. Skip it and find your own angle.
- **Don't be contrarian for sport.** Adversarial review means *finding what's wrong*,
  not *disagreeing with what's right*. If the prior review nailed it, say so briefly and
  move to what they missed.
- **Quote, don't summarize.** Every adversarial finding cites a specific line, claim, or
  decision. "The brief feels off" is not actionable. "The promise in §3 is generic
  enough that [Competitor X]'s homepage already says it" is.
- **The human is the final judge.** Your output is input to a human PMM, not a verdict.
  Frame findings as challenges to weigh, not commands to obey.

---

## Why this matters

Every model — and every reviewer — has a flavor of failure. The cheapest way to catch it
is to have a different model and a different human do an adversarial pass. Same loop the
best engineering teams run on critical code. Same reason: the work that ships shapes the
brand for years; the cost of catching it now is one prompt.

The output of /peer-review almost always routes to one of three places:
- A specific line edit in /write
- A strategic correction in /positioning-brief
- A canon update in /update-canon

If it routes to none of those, the peer review didn't find anything material. That's a
signal too — sometimes the work is just ready to ship.
