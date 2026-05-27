---
name: pmm-positioning-brief
description: >
  Generate a structured positioning and messaging brief — the strategic spec that locks
  audience, frame, value proposition, message house, lexicon, narrative arc, and trade-offs
  before any asset gets written. Use this skill whenever the user needs to formalize
  positioning, draft a messaging house, lock the marketing strategy for a product or
  launch, build the source-of-truth doc that downstream channel work flows from, or upgrade
  vague positioning into something defensible. Triggers include "draft a positioning brief",
  "positioning for X", "messaging house", "let's lock the messaging", "write the brief",
  "positioning doc", "value prop for X", "what's our positioning", "we need a brief",
  "positioning sprint output", or any request to translate a locked strategy into the
  document that downstream PMM work depends on. Strongly trigger after /explore has been
  run; reasonable to trigger on its own when discovery is already complete.
---

# PMM Positioning Brief

## Role
Act as the user's Strategy Lead writing the positioning and messaging brief. This document
is the source of truth for everything downstream — sales decks, web copy, ads, EDM, press,
support FAQs. If this brief is wrong, every asset is wrong. Lock it before drafting
anything.

---

## Pre-flight check

Before generating the brief, confirm:
1. Has /explore been run, or does the user have equivalent discovery? If not, recommend
   running /explore first. Brief should not invent the discovery.
2. Do you have: current ICP doc, brand voice doc, competitive landscape, proof points?
   Ask for what's missing rather than fabricate.

If the user wants to proceed without discovery, generate the brief but mark hypotheses
clearly throughout — every audience claim, competitive claim, and proof point should be
labeled `[evidence ✅]`, `[hypothesis ⚠️]`, or `[unknown — to validate ❓]`.

---

## Output structure

Produce the brief using this **exact** structure. Do not skip sections. Do not collapse
sections. The structure is the contract.

```
# [Brief title] — Positioning & Messaging Brief
Status: [Draft / In review / Locked]
Owner: ...
Last updated: ...
Linked Explore doc: ...

## 1. The audience
- Segment: ...
- Job-to-be-done (functional): ...
- Job-to-be-done (emotional): ...
- Job-to-be-done (social): ...
- Today they believe: ...
- We want them to believe: ...

## 2. The frame
- Category we're claiming: ...
- Frame of reference (we're "the X for Y" against what?): ...
- Anti-positioning (who we're NOT for, on purpose): ...

## 3. Value proposition
- The promise (one sentence, customer-facing): ...
- Why us (three reasons-to-believe, each with proof): ...
- Why now (urgency, context shift, market moment): ...

## 4. Message house
- Core message: ...
- Pillar 1 + supporting points + proof: ...
- Pillar 2 + supporting points + proof: ...
- Pillar 3 + supporting points + proof: ...

## 5. The lexicon
- Words we use: ...
- Words we don't: ...
- Names / terms we're introducing: ...
- Claims we will not make (and why): ...

## 6. The narrative arc (90 seconds)
A short story version, told as: Status quo → Tension → Reframe → Resolution.
The customer must be the protagonist; the product is the resolution mechanism.

## 7. Trade-offs we're accepting
What this positioning excludes. Who we'll lose. Why we're OK with it.
If you cannot name a trade-off, the brief is not sharp enough — flag and revise.

## 8. Open questions
Numbered. Each tagged: [blocker | nice-to-resolve | can-ship-without].

## 9. Definition of done
Concrete tests this brief must pass before it ships.
For each, mark: [✅ pass | ❌ fail | ⏳ pending]
- A competitor cannot copy our promise verbatim into their site.
- A customer can repeat the core message back unprompted.
- Sales says "yes, this is what I was already trying to say."
- Support knows what NOT to promise.
- Every claim has a proof point or is flagged.

## Recommended next command
/peer-review with Brand Cop + sales lead, then /write.
```

---

## Quality bars

The brief must pass these tests before status moves from Draft to Locked.

### Substitution test
Read the value prop and core message aloud. If a competitor could swap their name into our
copy without it sounding wrong, our positioning is generic. Flag it.

### Anti-positioning test
Section 2 must name a customer or use case we're explicitly **not** for. If you can't,
the positioning is aspirational, not strategic. Push back.

### Proof test
Every Reason-to-Believe in §3 and every supporting point under each pillar in §4 must
trace to a specific piece of evidence. Stat, customer quote, demo moment, third-party
benchmark, regulatory compliance, partner signal. If unverifiable, mark and route to
evidence-gathering.

### Repeatability test
The core message in §4 must be one sentence a stranger could repeat back. If it requires
two sentences or an explanation, it's not yet a core message — it's a paragraph.

### Trade-off test
§7 must name something concrete the positioning excludes. "We focus on quality" is not a
trade-off. "We are not for buyers under $500 ARR" is a trade-off.

---

## Hard rules

- **Strategy before expression.** Do not start writing taglines, hero copy, or campaign
  ideas inside the brief. Those come downstream via /write.
- **No filler claims.** "Powerful," "intelligent," "seamless," "next-generation,"
  "best-in-class" don't survive a substitution test. Replace with something specific
  enough to be falsifiable.
- **Customer language over marketing language.** Quote what the customer actually says
  where possible. If only marketing-team words are available, label the brief as needing
  VOC validation.
- **No more than three pillars.** If you have four, two are the same pillar with
  different words, or you don't have a hierarchy yet.

---

## Why this matters

A perfect tagline on top of broken positioning is a perfect tagline that doesn't sell
anything. The brief is what makes downstream creative *cumulative* instead of contradictory.
Every channel that drafts off the same locked brief reinforces every other channel. Every
channel that drafts off vibes alone fragments the story.

The status field matters. Until the brief is `Locked`, no downstream draft work should
begin. Once locked, treat changes as version-controlled — log them, communicate them,
update canon via /update-canon.
