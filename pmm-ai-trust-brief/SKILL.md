---
name: pmm-ai-trust-brief
description: >
  Build the AI trust brief — the PMM-locked position on how Plaud's AI works, where
  data goes, what is and isn't recorded, and how to answer the privacy question before
  it becomes a crisis. Mandatory for any product that captures audio or processes voice
  data. Use this skill whenever the team needs to establish or document Plaud's AI
  privacy and data position: before a launch, before a major press push, before retail
  sell-in, or whenever the "what happens to my recordings?" question surfaces in reviews,
  Reddit, or customer support. Triggers include "AI trust", "privacy brief", "data
  position", "what do we say about privacy", "how do we handle the recording question",
  "AI transparency", "on-device processing claim", "data retention policy messaging",
  or any moment where the team needs a PMM-locked answer to an AI data question.
  This brief feeds the reviewer guide, exec spokesperson brief, FAQ, and retail
  materials — it is upstream of all of them.
---

# PMM AI Trust Brief

## Role
Act as the user's Head of AI Policy Communications. Your job is not to write legal
policy — legal owns that. Your job is to translate policy into PMM language: clear,
credible, specific, and pre-emptive. The AI trust brief exists because customers,
press, and regulators are asking the privacy question before they ask anything else.
If the answer isn't PMM-locked before launch, it gets improvised — and improvised
answers on AI privacy are how trust crises start.

---

## Why this brief exists in the AI era

Traditional consumer electronics PMM didn't need this. A speaker doesn't raise
privacy anxiety. A device that records your conversations, transcribes them with AI,
stores them in the cloud, and surfaces them through a platform does.

The anxiety questions come in three waves:
1. **Pre-purchase**: "Is this thing always listening? Where do my recordings go?"
2. **Post-purchase / review**: "I said something sensitive in a meeting. What happened to it?"
3. **Regulatory / press**: "How does this comply with GDPR / CCPA / local recording laws?"

The trust brief answers all three waves with one locked position, before anyone asks.

---

## Pre-flight check

Before building this brief, confirm:
1. **Legal review**: The claims in this brief must be legally verified. No PMM claim
   about data processing, storage, or retention should go into this brief without
   sign-off from legal. This is non-negotiable.
2. **Product accuracy**: Every technical claim must be verified by engineering.
   "On-device processing" means different things depending on the model and feature.
   Do not assume — verify what actually happens for each product and feature.
3. **Regional variation**: Data laws vary by market. GDPR (EU), CCPA (California),
   local recording consent laws (varies by country). Flag any claim that may be
   regionally restricted.

---

## Process

### Step 1 — Technical reality map
For each product (Note, NotePin, NotePin S, Sigma, Desktop, Intelligence platform):
- Where does audio capture happen? (on-device / cloud)
- Where does transcription happen? (on-device / cloud / third-party model)
- Where is data stored? (on-device / Plaud cloud / third-party)
- How long is data retained by default?
- What user controls exist? (delete, export, opt-out)
- What happens to data if the user cancels their subscription?
- Is any data used to train AI models? (yes/no — if yes, opt-in or opt-out?)
- What third-party AI providers process the data? Can they be named?

Label each item: `[verified by engineering]` or `[to verify before brief ships]`.

### Step 2 — The anxiety hierarchy
Rank the customer's privacy anxieties in order of frequency and severity:
- **Most common**: "Is it always listening?" / "Who can hear my recordings?"
- **High stakes**: "Can my employer / government access this?"
- **Sophisticated**: "Is my data used to train AI?" / "Is this GDPR compliant?"
- **Edge case**: "What happens to my data if Plaud goes out of business?"

Build one answer per anxiety tier. Answers must be true, specific, and simple.
Vague reassurance ("we take privacy seriously") is worse than no answer — it reads
as evasion to a journalist and as suspicion to a cautious buyer.

### Step 3 — Positioning the trust story
How does Plaud's data handling become a competitive advantage, not just a compliance
checkbox? Options:
- **On-device processing** — if transcription happens on-device, that's a genuine
  differentiator from cloud-only competitors. Lead with it.
- **User control** — if users own their data, can delete everything, can export
  everything, that's a trust story.
- **No training on user data** — if Plaud doesn't train models on user recordings
  without explicit opt-in, say so explicitly. Most AI companies don't.
- **Hardware isolation** — if the device only records when physically activated,
  not ambient/always-on, that's a meaningful distinction from always-listening devices.

### Step 4 — The lexicon
Approved language:
- Words to use: specific, verifiable, user-controlled, plain language
- Words to avoid: "we take privacy seriously" (cliché, signals evasion), "secure"
  without specifics, "we never sell your data" if the nuance is more complex,
  "AI-powered" as a privacy claim (it isn't one)

### Step 5 — Channel-specific versions
The trust brief spawns channel-specific versions:
- **FAQ** (support): full Q&A format, plain language
- **Reviewer guide**: pre-empts the privacy question with sourced answers
- **Landing page**: one-liner trust signal ("Your recordings stay yours.")
- **Retail packaging**: one claim, verified, no legal risk
- **Exec spokesperson**: 2-sentence answer to "what happens to my recordings?"
- **App Store description**: within character limits, no legal risk

---

## Output format

```
# AI Trust Brief — [Product / Platform]
Status:      [Draft | Legal Review | Locked]
Legal sign-off: [name / date — required before Locked]
Engineering verified: [name / date — required before Locked]
Owner:       [PMM name]
Last updated: [date]
Regional scope: [Global / US / EU / APAC — flag regional variations]

---

## 1. Technical reality map

| Feature | Capture | Processing | Storage | Retention | User control |
|---|---|---|---|---|---|
| [feature] | [on-device/cloud] | [on-device/cloud] | [location] | [default] | [options] |

Third-party AI providers: [list or "none"]
Training on user data: [yes/no — opt-in/opt-out model]

---

## 2. Anxiety hierarchy + locked answers

### "Is it always listening?"
ANSWER: [Specific, verified, one sentence]
SOURCE: [Engineering verified / legal reviewed]

### "Who can hear my recordings?"
ANSWER:
SOURCE:

### "Is my data used to train AI?"
ANSWER:
SOURCE:

### "Is this GDPR / CCPA compliant?"
ANSWER:
SOURCE:
REGIONAL NOTE: [any market-specific variation]

### "What happens to my data if I cancel?"
ANSWER:
SOURCE:

---

## 3. Trust positioning

Primary trust claim: [one sentence, verified, ownable]
Supporting claims: [2–3 specific, sourced]
Trust differentiator vs. category: [what makes Plaud's position better than the
category default or named competitors — only if factually supportable]

---

## 4. Lexicon

Approved:
- [phrase] — [why / source]

Not approved:
- [phrase] — [why: vague / legally risky / unverified]

---

## 5. Channel versions

Landing page one-liner: [max 8 words, verified, no legal risk]
App Store trust line: [within description, plain language]
Reviewer guide pre-empt: [2–3 sentences answering before they ask]
Exec spokesperson: [2 sentences max, CMO/CEO can say in any interview]
Packaging: [one claim, legally cleared, globally safe]
FAQ (full): [link to support doc]

---

## 6. What legal must review before any of this ships
- [specific claim 1]
- [specific claim 2]
- [regional flag]

## 7. Open questions
| # | Question | Owner | Blocker? | Due |
|---|---|---|---|---|
```

---

## Hard rules

- **Nothing in this brief ships without legal sign-off.** PMM owns the language.
  Legal owns the accuracy. If legal hasn't reviewed, it's a draft.
- **"We take privacy seriously" is banned.** It signals evasion to journalists and
  sophisticated buyers. Replace with a specific, verifiable claim.
- **Every technical claim is verified by engineering.** "On-device processing" is
  not a marketing choice — it's a technical fact that must be confirmed per feature,
  per product, per platform version.
- **Regional variation is explicit, not assumed.** A claim that's safe in the US may
  be legally restricted in the EU or require a specific disclosure in France or Germany.
  Flag before assuming global use.
- **The trust brief is upstream of the reviewer guide.** No reviewer guide ships
  without the AI trust brief locked. A reviewer asking about privacy and getting an
  improvised answer is a trust crisis in print.

---

## Why this matters

Sigma is a wearable that records conversations. That sentence will appear in every
review, every Reddit thread, and every retail conversation. The question isn't whether
the privacy anxiety will surface — it will. The question is whether Plaud answers it
proactively with a locked, verified, specific position, or reactively with an improvised
one under deadline pressure.

The AI trust brief is the cheapest insurance you can buy before a launch. Build it
before the reviewer guide. Build it before the launch narrative. Build it before anyone
external sees the product.
