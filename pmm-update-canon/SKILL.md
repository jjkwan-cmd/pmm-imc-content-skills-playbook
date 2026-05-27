---
name: pmm-update-canon
description: >
  Update product marketing canonical documentation — the message house, lexicon, proof
  bank, brand voice doc, competitor file, prompt library, and post-mortems — after a
  campaign, launch, repositioning, or any decision that changes what's true about how the
  brand goes to market. Use this skill at the end of a project, after a launch retro, when
  a positioning decision changes, when a claim gets killed, when a new proof point is
  validated, or when the team learns something the hard way that future work should
  inherit. Triggers include "update the messaging doc", "update the brand book", "post
  mortem", "lessons learned", "canon update", "update the lexicon", "add to the proof
  bank", "we learned X", "after this launch", "wrap up the campaign", "what should we
  remember from this", "update our docs", "log the learning", or any moment a project ends
  and there's institutional knowledge worth preserving so the next project starts smarter.
---

# PMM Update Canon

## Role
Act as the user's brand archivist. The point of this skill is to **make the team's
knowledge compound**. Without canon updates, every new project starts from zero and the
team's effective experience never grows beyond the tenure of its most senior member.

The output is a series of doc-by-doc changesets the user can paste into the actual canon
docs. Don't update prose loosely; produce diffs.

---

## Pre-flight check

Gather the inputs before drafting. Ask for what's missing:
1. **The locked brief** for the project that just shipped.
2. **The shipped assets** (or links to them).
3. **The performance readout** — what worked, what didn't, against the original KPIs.
4. **Customer / sales / support / CS feedback** captured during or after the launch.
5. **Anything the team killed mid-flight** and why (a claim, a campaign, a tactic).

Without these, the update will be vibes. Push back politely if the user wants to skip
the inputs.

---

## The seven canon docs

Update each, with diffs. Skip a doc only if there's genuinely nothing to add — but be
honest about that, since "nothing to add" usually means we didn't look hard enough.

### 1. The message house
- New pillars or supporting points to add?
- Pillars to retire or rephrase?
- Proof points to attach to existing pillars?
- A pillar that didn't survive contact with the market — recommend retiring or
  reformulating, with reasoning.

### 2. The lexicon
- New "words we use" earned during this project (with example).
- New "words we don't" — what failed in customer language? What did we ban for cause?
  Always cite the offending example so the next PMM knows *why*.
- New names or terms we introduced (and the rule for capitalization, hyphenation, plural).
- New banned claims, with the offending quote and the reason (legal, evidence,
  positioning, brand voice).

### 3. The proof bank
- New customer quotes, with attribution and consent status.
- New stats, with source and date.
- New case studies or social proof.
- Tag each by the pillar it supports.

### 4. The brand voice doc
- New voice rules learned the hard way (with the example that taught us).
- Tone deviations that worked (or didn't) in specific channels.
- Visual identity additions if relevant — typography, color, motion, layout rules.

### 5. The competitor file
- Moves observed during the project window.
- New claims they're making.
- Our response (if any), and lessons from how the response landed.

### 6. The prompt library
- If any /command needs an update based on what we learned, propose the diff.
- Especially: did /explore miss something we should add? Did /write produce off-brief work
  in a specific way we should prevent? Did /review fail to catch a category of error we
  should add to the eight-pass check?

### 7. The post-mortem
- What worked. (Be specific — generic praise teaches nothing.)
- What didn't. (Be specific — vague critique blames no one and changes nothing.)
- What we'd do differently. (One paragraph per change. Concrete enough to be a rule next
  time.)
- The single biggest lesson. (One sentence. The thing this project taught us that no other
  project has.)

---

## Output format

For each doc, produce a changeset block the user can paste:

```
=== UPDATE: Message House ===

ADD to Pillar 2 supporting points:
- "[new supporting point]" — proof: [quote/stat], evidence link: [...]

RETIRE: "[old supporting point]" — reason: [didn't survive customer testing /
no longer accurate / off-positioning post-relaunch]

EDIT: "[old phrasing]" → "[new phrasing]" — reason: [...]

=== UPDATE: Lexicon ===

ADD "Words we use":
- "[term]" — context: [...]

ADD "Words we don't":
- "[term]" — reason: [...]
  - Example of why: "[the offending shipped line]"

ADD "Banned claims":
- "[claim]" — reason: [...]

=== UPDATE: Proof Bank ===

ADD:
- Quote: "[customer quote]" — source: [...] — pillar: [...]
- Stat: [number + unit] — source: [...] — pillar: [...]

=== UPDATE: Brand Voice ===

ADD voice rule:
- [rule] — reason: [...]
  - Taught by: "[example asset]"

=== UPDATE: Competitor File ===

ADD entry, [Competitor], [date]:
- Move: ...
- Our response: ...
- Lesson: ...

=== UPDATE: Prompt Library ===

PROPOSED EDIT to /[command]:
- Current: "[old line]"
- New: "[new line]"
- Reason: [what we learned that this prevents]

=== POST-MORTEM ===

# [Project name] — Post-Mortem
Date: ...
Owner: ...

## What worked
- ...

## What didn't
- ...

## What we'd do differently
- ...

## The single biggest lesson
[One sentence.]
```

---

## Hard rules

- **Diffs, not prose.** The point of canon updates is paste-ability. Don't write
  paragraphs; write changesets.
- **Cite the example.** Every banned claim, every new voice rule, every retired pillar
  should reference the specific asset or quote that taught us. Without citation, the next
  PMM doesn't believe the rule.
- **No vague learnings.** "We need to be more disciplined about reviews" is not a learning.
  "Reviews missed three filler-word violations because reviewer didn't have the brand
  voice doc open — change /review pre-flight to require it" is a learning.
- **Every claim killed becomes a banned claim with reason.** This is the single most
  valuable canon entry — it stops the same bad claim from being re-proposed every quarter.

---

## Why this matters

The compounding part of PMM happens in the canon. The team's ten-thousandth shipped asset
should be better than the first not because the team is smarter, but because the team is
*better-informed*. Canon is the institutional memory that survives turnover, scaling,
agency changes, and re-orgs.

If the canon update produces nothing — no diffs, no lessons, no banned claims, no new
proof — that's a signal: either the project shipped on autopilot (in which case why did
we run it?) or the team didn't reflect honestly. Push back politely; ask one more time
what surprised them.
