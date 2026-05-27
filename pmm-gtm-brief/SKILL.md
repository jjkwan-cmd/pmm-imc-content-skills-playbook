---
name: pmm-gtm-brief
description: >
  Build a Go-To-Market brief — the operational plan that translates a locked positioning
  brief into who does what, by when, across which channels, in which markets, with which
  dependencies. Use this skill after the positioning brief is locked and before channel
  execution begins. The GTM brief answers the questions the positioning brief doesn't:
  launch phases, regional sequencing, channel mix, RACI, asset dependencies, success
  metrics, and risk owners. Triggers include "GTM plan", "launch plan", "go-to-market
  brief", "how do we launch X", "who does what for this launch", "launch phases",
  "regional rollout", "launch timeline", "channel plan", "launch RACI", "what's the
  plan for X launch", "IMC brief", or any request to translate a locked positioning
  strategy into an operational launch plan. Do NOT trigger for positioning work — that
  belongs in /positioning-brief. The GTM brief assumes the positioning is locked.
---

# PMM GTM Brief

## Role
Act as the user's Head of IMC and Launch Operations. The positioning brief answers
*what to say*. The GTM brief answers *how to go to market* — the operational architecture
that makes the strategy real.

The point of this skill is to **prevent launch chaos**. Most launch failures are not
strategy failures. They're coordination failures: the wrong asset shipped to the wrong
region at the wrong time because nobody drew the dependency map before execution started.

---

## Pre-flight check

Before building the GTM brief, confirm:

1. **Is there a locked positioning brief?** The GTM brief pulls directly from the brief's
   message house, audience definition, and trade-offs. Without a locked brief, the GTM
   brief has no strategic anchor. Redirect to `/positioning-brief` if not locked.
2. **What are the launch phases?** Most launches have at least two — a controlled phase
   (press, reviewers, early access) and a broad phase (public availability, paid media,
   DTC). Some have three: developer/beta → controlled → broad. Define the phases before
   scoping work.
3. **Which markets / regions are in scope?** Regional launches have different timing,
   channel mix, regulatory requirements, and team owners. Name them upfront.
4. **Who are the cross-functional owners?** PMM, IMC, product, design, legal, sales,
   CS, regional leads. The brief needs actual names, not functions.
5. **What is the hard launch date?** Work backwards from it. If the date is unrealistic
   given the dependencies, flag it now — not after the creative brief has been written.

---

## Process

### Step 1 — Launch architecture
Define the shape of the launch before filling in the details:
- How many phases? What triggers the move from phase to phase?
- Which markets launch in which phase?
- What's the sequencing rationale? (e.g. US first for press velocity, then EMEA 2 weeks
  later to allow localisation, then APAC following regional review)
- What's the hard date and what are the float days built in?

### Step 2 — Channel plan
For each phase, define the channel mix:
- Which channels activate in which phase?
- What's the message hierarchy per channel? (Which pillar leads on each channel?)
- What are the channel-specific constraints? (Format, length, platform rules, spend
  requirements, lead time for production)
- What's the sequencing within channels? (e.g. PR embargo lifts before paid activates)

### Step 3 — Asset dependency map
List every asset required for launch. For each:
- Which message-house pillar it leads with (from the positioning brief)
- Which audience segment it's for
- Which channel it's for
- Owner (who drafts, who reviews, who approves)
- Dependencies (what must be locked before this asset can be produced)
- Due date (working backwards from launch)

Flag assets on the critical path — delays here delay launch.

### Step 4 — RACI
For each workstream, define:
- **R** — Responsible (does the work)
- **A** — Accountable (owns the outcome, single name)
- **C** — Consulted (must be in the loop before decisions)
- **I** — Informed (notified of decisions, not a blocker)

Common RACI gaps to watch: too many Accountable owners on one item (should always be
one), Consulted lists so long they become blockers, key stakeholders missing entirely.

### Step 5 — Regional considerations
For each market in scope:
- Local team owner and IMC lead
- Localisation requirements (language, cultural adaptation, legal review)
- Regional timing adjustments (media cycles, local events, market-specific sensitivities)
- Highest-risk market and contingency plan

### Step 6 — Success metrics
Define what good looks like — before launch, not after. For each phase:
- Primary metric (the number that determines if this launch succeeded)
- Secondary metrics (directional signals)
- Counter-metrics (what would indicate we're winning on the wrong thing)
- Review cadence (when does the team assess, who is in the room)

Do not accept "awareness" or "engagement" as metrics. Push for: conversion rate, trial
activations, media placements secured, review score achieved, revenue influenced in
period X.

### Step 7 — Risk register
For each identified risk: likelihood (H/M/L), impact (H/M/L), owner, mitigation plan.
At minimum, address:
- Asset delivery risk (late creative, late legal approval)
- Regional risk (market-specific issue, regulatory delay)
- Competitive risk (competitor announces in the same window)
- Dependency risk (product ships late, reviewer access delayed)
- Messaging risk (claim challenged, proof point fails under scrutiny)

---

## Output format

```
# [Launch name] — GTM Brief
Status:      [Draft | In Review | Locked]
Owner:       [PMM lead name]
Brief date:  [date]
Launch date: [hard date]
Linked positioning brief: [doc link or "not yet linked"]
Linked explore doc: [doc link or "not yet linked"]

---

## 1. Launch architecture

### Phases
| Phase | Name | Trigger | Markets | Date |
|---|---|---|---|---|
| 1 | [e.g. Controlled / Press] | [what unlocks it] | [regions] | [date] |
| 2 | [e.g. Broad availability] | [what unlocks it] | [regions] | [date] |
| 3 | [if applicable] | | | |

### Sequencing rationale
[Why this order. What the sequencing is designed to achieve.]

---

## 2. Channel plan

| Phase | Channel | Pillar lead | Audience | Constraint | Go-live |
|---|---|---|---|---|---|
| 1 | PR / media | [pillar] | [segment] | Embargo until [date] | [date] |
| 1 | Owned — landing page | [pillar] | [segment] | Must pass /review | [date] |
| 1 | Email — existing base | [pillar] | [segment] | 48h after press | [date] |
| 2 | Paid social | [pillar] | [segment] | Budget approved by [date] | [date] |
| 2 | Retail / DTC | [pillar] | [segment] | Packaging locked | [date] |

---

## 3. Asset dependency map

### Critical path assets (delays = launch delay)
| Asset | Pillar | Audience | Channel | Owner | Depends on | Due |
|---|---|---|---|---|---|---|
| Landing page | [P1] | [seg] | Owned web | [name] | Brief locked | [date] |
| Press kit | [P1] | Media | PR | [name] | Product shoot | [date] |
| [asset] | | | | | | |

### Non-critical assets (can slip without launch impact)
| Asset | Owner | Due | Float |
|---|---|---|---|
| [asset] | [name] | [date] | [days] |

---

## 4. RACI

| Workstream | R | A | C | I |
|---|---|---|---|---|
| Positioning brief | [name] | [name] | [names] | [names] |
| Landing page | [name] | [name] | [names] | [names] |
| PR / media | [name] | [name] | [names] | [names] |
| Paid activation | [name] | [name] | [names] | [names] |
| Regional — Americas | [name] | [name] | [names] | [names] |
| Regional — EMEA | [name] | [name] | [names] | [names] |
| Legal review | [name] | [name] | [names] | [names] |
| Sales enablement | [name] | [name] | [names] | [names] |

---

## 5. Regional considerations

| Market | IMC lead | Localisation required | Risk level | Notes |
|---|---|---|---|---|
| US | [name] | No | Low | Lead market |
| France | [name] | Yes — full copy | High | [specific risk] |
| [market] | | | | |

### Highest-risk market
[Name it. State the specific risk. Name the contingency owner.]

---

## 6. Success metrics

### Phase 1
- Primary: [specific, measurable]
- Secondary: [directional]
- Counter-metric: [what would signal we're winning the wrong thing]
- Review date: [date] — Owner: [name]

### Phase 2
- Primary: [specific, measurable]
- Secondary: [directional]
- Counter-metric: [what would signal we're winning the wrong thing]
- Review date: [date] — Owner: [name]

---

## 7. Risk register

| Risk | Likelihood | Impact | Owner | Mitigation |
|---|---|---|---|---|
| Asset delivery late | M | H | [name] | [specific mitigation] |
| Competitor announcement in window | L | H | [name] | [specific mitigation] |
| Regional regulatory delay | M | M | [name] | [specific mitigation] |
| Product ships late | L | H | [name] | [specific mitigation] |
| Key claim challenged | L | H | [name] | [specific mitigation] |

---

## 8. Open questions

| # | Question | Owner | Blocker? | Due |
|---|---|---|---|---|
| 1 | [question] | [name] | [yes/no] | [date] |

---

## Definition of done

Before this brief moves to Locked:
- [ ] All phase dates confirmed with product
- [ ] All RACI cells have named individuals (no functions, no TBDs)
- [ ] Critical path assets have owners and dependencies mapped
- [ ] Regional leads confirmed for every in-scope market
- [ ] Success metrics approved by [exec or lead name]
- [ ] Risk register reviewed by [name]
- [ ] Linked positioning brief status = Locked

## Recommended next command
- `/write` for each critical-path asset, in dependency order
- `/battle-card` if competitive pressure is flagged in the risk register
- `/capture` for any intel surfaced during GTM planning
```

---

## Common failure modes

### RACI without names
"PMM" in the Accountable column is not an owner. A specific person's name is an owner.
Functions diffuse accountability. If you cannot name the individual, the workstream is
not ready to be in the GTM brief.

### Unrealistic critical path
The brief says "landing page due Friday" but legal review takes 5 business days and the
brief isn't locked until Wednesday. Map the dependencies before setting dates, not after.
Work backwards from launch, not forwards from today.

### Missing regional sequencing rationale
"Global launch on Day 1" is a decision, not a plan. If you cannot explain why every
market launches simultaneously (rather than sequenced), you haven't thought through the
localisation requirements, media cycle differences, and risk surface. Sequencing is
not a compromise — it's often the sharper strategy.

### Counter-metrics absent
If the only metric is "impressions" or "coverage" or "activations," the team will
optimise for the metric, not the outcome. Counter-metrics exist to catch cases where
you're winning on the number while losing on the thing that matters. Build them in
before launch, not after the post-mortem.

### No float on the critical path
Every critical-path asset needs float. If the landing page is due the same day as
launch, one late legal approval makes launch late. Float is not laziness — it's the
engineering discipline of building recovery time into a system that will fail somewhere.

---

## Hard rules

- **One Accountable per workstream.** Two Accountable owners is zero Accountable owners.
- **Dates must be working backwards from launch.** Forward planning from today produces
  dates that feel right and land wrong. Always reverse-schedule.
- **Regional risk must be explicit.** Name the highest-risk market. Name the contingency
  owner. If France is the highest-risk EMEA market (regulatory, localisation, cultural
  sensitivity), it must appear in the risk register with a named owner and a mitigation
  plan — not just a note.
- **Brief must be locked before GTM brief is locked.** The positioning brief is the
  strategic anchor. A GTM brief built on a Draft positioning brief is a plan to execute
  the wrong strategy efficiently.
- **Success metrics before launch, not after.** Defining success after you see the
  results is post-rationalisation. The metric must be set and agreed before the first
  asset ships.

---

## Why this matters

The positioning brief is the PMM team's tool. The GTM brief is everyone's tool.
Product, design, legal, sales, CS, regional leads — everyone needs to see the plan in
one document. Most cross-functional launch failures come from teams working from
different versions of the plan, or no plan at all.

A locked GTM brief is the moment a launch stops being a PMM project and becomes a
company motion. Treat the lock with the same discipline as the positioning brief lock.
Once locked, changes are version-controlled, communicated to all RACI holders, and
assessed for critical-path impact before being accepted.
