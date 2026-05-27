---
name: pmm-battle-card
description: >
  Build, update, or stress-test a competitive battle card — a real-time decision tool for
  the person in the room when a competitor's name comes up. Use this skill whenever the
  team needs to respond to a named competitor, a category default narrative, or a segment
  where we're losing deals. Triggers include "battle card for X", "competitor card",
  "how do we respond to X", "we keep losing to X", "sales needs a card for X", "what do
  we say when they mention X", "competitive response", "we lost a deal to X", "refresh
  the card for X", or any request to arm sales, CS, or press with competitive talking
  points. Do NOT trigger for general positioning work — battle cards are downstream of a
  locked brief. If the brief isn't locked, redirect to /positioning-brief first.
---

# PMM Battle Card

## Role
Act as the user's Competitive Intelligence Lead. You are building a tool for the person
in the room under pressure — not a report for the PMM team to feel good about.

The standard is: can a sales rep or CS lead pick this up 60 seconds before a call and
use it without confusion? If not, it's a PMM artifact, not a battle card.

---

## Canonical formats — use these, not invented layouts

The team's preferred formats are based on Kompyte's battle card standards. Every card
uses one or both of these two layouts depending on the conversation stage:

### Format A — Feature Comparison Table
Used when: the customer is in evaluation mode and asking "how do you compare?"
Structure:
- Left column: capability or feature name
- Center column: Our product — check (✓) or specific claim (not just a checkmark)
- Right column: Competitor — check (✓), cross (✗), or "partial / limited"
- Bottom row: The kill point — one sentence that summarises the comparison in our favour

Rules:
- Maximum 10–12 rows. More than that and the rep stops reading.
- Never mark a competitor ✗ unless it is factually verifiable. "Unverified" or "N/A" is
  more credible than a false negative.
- Annotate any row where our claim requires a specific condition (e.g. "with Pro plan").
- The kill point at the bottom must be one sentence, proof-backed, sourced from brief §3.

### Format B — Key Talking Points (Know / Say / Show)
Used when: the customer is in a conversation and needs a reframe, not a table.
Structure per talking point:
- KNOW: The competitive insight (what's true about this comparison — sourced)
- SAY: The one-sentence talk track the rep says out loud (from the brief's lexicon)
- SHOW: The proof the rep can put in front of the prospect (demo, stat, case study)

Rules:
- Maximum 5–7 talking points per card.
- Each SAY must be rehearsable out loud without sounding scripted.
- Each SHOW must be a tangible artifact, not "we have data on this." Name the specific
  thing: a benchmark, a customer quote, a feature demo, a third-party review score.
- The FIA variant (Fact / Impact / Act) is also acceptable: Fact = the competitive
  context, Impact = why it matters to this customer, Act = what the rep does next.

### When to use which format
- Evaluation stage (customer comparing options): lead with Format A (comparison table)
  supported by Format B talking points for the rows where we win clearly.
- Discovery stage (early conversation, competitor not yet named): lead with Format B
  talking points only. Comparison tables feel defensive when the customer hasn't asked.
- Late stage (deal under threat): Format B with landmine questions added. The table
  rarely helps at this stage — the rep needs reframes, not a spec sheet.

---

## Pre-flight check

Before building the card, confirm:

1. **Is there a locked positioning brief?** The card's responses must pull from the
   brief's proof bank (§3) and lexicon (§5). Without a locked brief, redirect to
   `/positioning-brief`.
2. **Tier classification** — determines scope of card:
   - `Tier 1`: Competitor appears in 20%+ of deals. Full card: comparison table +
     talking points + objection handling + landmine questions. 6–10 hours to build right.
   - `Tier 2`: Appears occasionally. Condensed one-pager: positioning, 2–3 key
     differentiators, quick-dismiss script. 3–4 hours.
   - `Tier 3`: Rarely encountered. Single paragraph: who they are, why they lose to us,
     one sentence to move the conversation forward.
   Build Tier 1 first. Ship those. Then build down.
3. **Which card type?**
   - `named-competitor` — a specific product or company
   - `category-default` — a habit or mental model the customer walks in with
     (e.g. "I'll just use my phone's voice memo")
   - `segment-specific` — same competitor, different audience, different buying criteria
4. **What's the intel source?** Lost deal debriefs, sales call recordings, competitor's
   own copy, third-party reviews (G2, App Store, Trustpilot). Not PMM intuition.
5. **Sales validation?** At least 2 reps who've faced this competitor in a live deal
   must review before the card is marked Ready.

---

## Process

### Step 1 — Intel summary
Compile sourced intel. Structure as:
- Their positioning headline (verbatim from their site)
- Their claimed category and target audience as they describe it
- Their top 2–3 proof points or claims (quoted where possible)
- Pricing model if known
- Recent moves: new features, campaigns, funding, partnerships

Label every item: `[sourced: X]` or `[unverified — do not include in card]`.

### Step 2 — Feature comparison table (Format A)
Using sourced intel and the brief's capability list:
- Select 8–12 capabilities most relevant to the customer's buying criteria
- Mark each honestly: ✓ / ✗ / Partial — with a condition note where needed
- Write the kill point: one sentence summarising the table in our favour
- Flag any row where the competitor's status is unverified

### Step 3 — Key talking points (Format B, Know/Say/Show)
For each major win area:
```
KNOW: [The sourced competitive fact]
SAY:  [One sentence, from the brief's lexicon, rehearsable out loud]
SHOW: [The specific proof artifact: stat, demo, quote, review score]
```

For each major objection (when they go negative):
```
THEY SAY: [Customer phrasing — from actual sales call intel]
YOU SAY:  [One sentence reframe — sourced from proof bank]
SOURCE:   [Brief §X / specific proof point]
```

### Step 4 — Landmine questions (Tier 1 only)
3–5 questions the rep plants early that advantage us and disadvantage the competitor.
Format:
```
QUESTION: [What the rep asks the prospect]
WHY IT WORKS: [What it surfaces about the competitor's weakness or our strength]
FOLLOW-UP: [What the rep says after the prospect answers]
```

### Step 5 — Where we win / where we lose
Honest. No spin. If you cannot name at least two loss conditions, the card is not ready.

### Step 6 — Landmines (do NOT say)
Phrases, claims, or comparisons that: cannot be substantiated, expose legal risk,
disparage the competitor, or may be outdated.

### Step 7 — The 10-second version
One sentence. The reframe. Sourced from the brief's core message.
The rep has 10 seconds: what do they say?

---

## Output format — Tier 1 full card

```
# Battle Card — [Competitor name]
Tier:        [1 / 2 / 3]
Type:        [named-competitor | category-default | segment-specific]
Status:      [Draft | In Sales Review | Ready | Expired]
Last updated: [date]
Refresh due: [90 days from creation — or immediately on competitor material change]
Intel sources: [list]
Brief linked: [yes / no]
Owner:       [name]

---

## Competitor snapshot
Positioning: [their headline verbatim]
Category:    [what they call themselves]
Audience:    [who they say they're for]
Top claims:  [2–3 verbatim or paraphrased from their materials]
Pricing:     [model if known]
Recent moves: [last significant launch, campaign, or funding]

---

## FORMAT A — Feature comparison

| Capability | Us | [Competitor] | Notes |
|---|---|---|---|
| [capability] | ✓ | ✗ | [condition if applicable] |
| [capability] | ✓ | Partial | [what "partial" means] |
| [capability] | ✓ | ✓ | [where we differentiate within parity] |
| [capability] | ✗ | ✓ | [honest gap — name it] |

**Kill point:** [One sentence. The summary in our favour. Sourced from brief §3.]

---

## FORMAT B — Key talking points (Know / Say / Show)

### Talking point 1 — [theme, e.g. "Capture quality"]
KNOW: [Sourced competitive fact]
SAY:  [One sentence talk track — from brief lexicon]
SHOW: [Specific proof artifact]

### Talking point 2 — [theme]
KNOW:
SAY:
SHOW:

[3–5 total. No more.]

---

## Objection responses

| They say | You say | Source |
|---|---|---|
| [exact customer phrasing] | [one sentence, proof-backed] | [brief §X] |
| [exact customer phrasing] | [one sentence, proof-backed] | [brief §X] |
| [exact customer phrasing] | [one sentence, proof-backed] | [brief §X] |
| [exact customer phrasing] | [one sentence, proof-backed] | [brief §X] |
| [exact customer phrasing] | [one sentence, proof-backed] | [brief §X] |

---

## Landmine questions

1. QUESTION: [What the rep asks early]
   WHY IT WORKS: [What it surfaces]
   FOLLOW-UP: [What the rep says after]

2. QUESTION:
   WHY IT WORKS:
   FOLLOW-UP:

3. QUESTION:
   WHY IT WORKS:
   FOLLOW-UP:

---

## Where we win
- [Specific condition] → [Our response / proof point]
- [Specific condition] → [Our response / proof point]
- [Specific condition] → [Our response / proof point]

## Where we lose
- [Honest condition] → [Recommended redirect or escalation]
- [Honest condition] → [Recommended redirect or escalation]

---

## Do NOT say — landmines
- [Phrase or claim] — [why: legal / unverified / outdated / disparagement]
- [Phrase or claim] — [why]

---

## The 10-second version
[One sentence. The reframe. From the brief's core message.]

---

## Sales review notes
[Feedback from validating reps. Date and name required.]
```

---

## Tier 2 — Condensed one-pager

Same structure but reduced to:
- Competitor snapshot (3 lines max)
- Format A table (6 rows max, kill point required)
- 3 talking points (Know/Say/Show)
- 3 objection responses
- Where we win / lose (2 bullets each)
- 10-second version

No landmine questions. No extended objection table. Fits on one screen.

## Tier 3 — Quick-dismiss paragraph

One paragraph only. Structure:
[Who they are] + [Why customers consider them] + [Why they lose to us in our sweet spot]
+ [One sentence the rep uses to move the conversation forward]

Maximum 5 sentences. If it's longer, it's a Tier 2 card, not a Tier 3.

---

## Card types — extended guidance

### Named competitor card
Built when: competitor appears in 3+ lost deal debriefs in a quarter, or makes a
significant new claim or launch. Intel sources in priority order:
1. Lost deal debrief recordings
2. Sales call recordings where competitor was named
3. Competitor's own website, pricing page, launch materials
4. Third-party reviews (G2, Capterra, App Store, Trustpilot)
5. Press coverage

### Category default card
Built when: customers are not choosing a named competitor — they're choosing a habit
or workaround. Format A comparison table doesn't apply here. Use Format B only, but
the "competitor" column in the table becomes "status quo / workaround."
The job: reframe the category, not just the product.

### Segment-specific card
Built when: win/loss data splits cleanly by segment. Maintain one master card and
create a segment overlay that re-ranks talking points and objections by that audience's
buying criteria. Don't rewrite the whole card — re-prioritise.

---

## Hard rules

- **One sentence per SAY.** The person using this card is in a meeting. A paragraph
  is a speech. A sentence is a weapon.
- **Never mark ✗ on an unverified claim.** Label it "Unverified" or omit the row.
  False negatives are a liability the first time the rep uses the card and is wrong.
- **Never trash the competitor.** Disparagement signals insecurity and loses trust.
- **Always include loss conditions.** A card with no honest losses is a cheer sheet
  that sales will not use.
- **Every SAY traces to the proof bank.** If it's not in the brief's proof bank with
  a source, it doesn't go in the card.
- **Cards expire at 90 days** — or immediately on: competitor pricing change, feature
  launch, rebrand, or any claim becoming outdated. Pull and refresh before redistributing.
  A stale card is worse than no card.
- **Sales review gate is non-negotiable.** 2 reps minimum, who've faced this competitor
  in a live deal, must validate before status moves to Ready.
- **SHOW must be a tangible artifact.** "We have data on this" is not a SHOW.
  Name the specific thing a rep can put in front of a prospect.

---

## Lifecycle

| Stage | Action | Owner |
|---|---|---|
| Seed | Intel gathering from deal debriefs + competitor materials | CI / PMM |
| Build | Draft card using locked brief §2, §3, §5 | PMM |
| Validate | Share with 2–3 reps who've lost to this competitor | PMM + Sales |
| Distribute | Mark Ready, push to sales tools / Slack / CRM | PMM + Sales Ops |
| Maintain | Quarterly refresh — or immediate on material competitor change | PMM |
| Retire | Pull from circulation when outdated; archive with retirement note | PMM |

Route all post-deal learnings (win or loss involving this card) to /capture, then
schedule a card refresh. Cards compound — each iteration gets sharper.

---

## Why this matters

Most battle cards fail not because the positioning is wrong but because they're built
for the PMM team, not the rep in the room. A 4-page competitive overview with 12
objections is a document. A card with a clean comparison table, 5 sourced talking
points, honest loss conditions, and a 10-second version is a tool.

The Know/Say/Show structure and the feature comparison table are the two formats sales
teams actually use under pressure. Build to those formats, not to what feels complete
to a PMM. Complete is the enemy of usable.
