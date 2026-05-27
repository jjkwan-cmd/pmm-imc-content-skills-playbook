---
name: pmm-aso-brief
description: >
  Build the App Store Optimization (ASO) brief — the PMM brief for App Store and
  Google Play listing copy, screenshots, preview video, and metadata. A distinct
  deliverable with distinct constraints from web copy. The App Store algorithm is
  not SEO. Character limits are hard stops. Screenshots are the primary conversion
  driver. Most PMM teams treat ASO as copy cleanup — it is a conversion channel.
  Triggers include "App Store copy", "ASO brief", "App Store listing", "Google Play
  listing", "app store optimization", "app store screenshots", "app preview video",
  "what's new copy", "app store metadata", or any request to write, brief, or
  optimize app store listing content.
---

# PMM ASO Brief

## Role
Act as the user's ASO Lead. App Store listings are high-traffic, low-attention
conversion moments. The customer is on their phone, scrolling, making a decision
in under 10 seconds. The PMM brief for ASO is different from every other brief
because the constraints are technical (hard character limits), the algorithm
is opaque (keyword density matters differently from SEO), and the primary
conversion driver is visual (screenshots, not copy).

---

## ASO vs. web copy — the key differences

| Dimension | Web copy | ASO copy |
|---|---|---|
| Primary conversion driver | Headline + hero copy | Screenshots + preview video |
| Character limits | Soft | Hard stops (title: 30, subtitle: 30, desc: 4000) |
| Algorithm | SEO / semantic | Keyword density + download velocity |
| Audience attention | Seconds to minutes | Under 10 seconds |
| Trust signals | Social proof, press logos | Ratings, reviews, editorial badge |
| Update cadence | Campaign-driven | Feature release + A/B test driven |

---

## App Store anatomy (iOS)

**Title** (30 chars): Product name + most important keyword. Not just the product name.
The keyword in the title carries the highest ASO weight of any field.
Example: "Plaud Note — AI Voice Recorder" not just "Plaud Note"

**Subtitle** (30 chars): Second-highest keyword weight. One clear value statement.
Example: "Transcribe, Summarize, Act"

**Description** (4000 chars): Only the first ~255 chars appear before "More" — these
are the only chars most users read. Front-load the value proposition. The rest of
the description is keyword-rich but still PMM-quality copy.

**What's New** (4000 chars, updates only): Not a changelog. A customer-facing value
statement about what improved. "Your meetings now work harder for you" — not
"Fixed bug where transcription would occasionally fail on recordings over 2 hours."

**Keywords field** (100 chars, iOS only, comma-separated, hidden): Words NOT already
in title/subtitle/description. Pure algorithm — customers never see this.

**Screenshots** (up to 10): The primary conversion driver. Each screenshot has a
device image + caption overlay. The caption is PMM copy, not a product description.
The first 3 screenshots appear in search results — these must convert without
the customer tapping into the full listing.

**Preview video** (15-30 seconds, auto-plays muted): First 3 seconds are critical.
Must work muted. Captions mandatory. Show the AI output — not the device.

---

## Google Play differences

- Title: 50 chars (more flexibility)
- Short description: 80 chars (visible before expand)
- Long description: 4000 chars
- No hidden keyword field — keywords must appear in copy
- Feature graphic: banner image in store listing
- Promotional text: 80 chars (can be updated without a new release)

---

## Process

### Step 1 — Keyword research
- Primary keyword: what does the target customer search? ("AI voice recorder",
  "meeting transcription", "voice memo AI")
- Secondary keywords: related intent terms
- Competitor keyword analysis: what keywords are Otter.ai, Fireflies, etc.
  ranking for in the App Store?
- Brand keywords: Plaud Note, Plaud NotePin, Plaud Intelligence
Map which keywords go in: title, subtitle, description, keyword field (iOS)

### Step 2 — Title and subtitle
With 30 chars each, every character is a decision:
- Title must contain: brand name + primary keyword
- Subtitle must contain: secondary keyword + value statement
- Test for: keyword density, character count, readability, brand consistency

### Step 3 — First 255 chars of description
This is the copy most users read. It must:
- State the primary value proposition
- Name the most important feature
- Create enough curiosity to tap "More"
- Contain secondary keywords naturally

### Step 4 — Screenshot brief
Screenshots are a creative brief within the ASO brief. For each of the 10 slots:
- Device image: what screen/state of the app to show
- Caption copy: the PMM claim this screenshot proves (max ~60 chars visible)
- Caption position: above or below the device
- Which 3 are "search visible" (appear without tapping into listing)?

The first 3 screenshots must convert a customer who has never heard of Plaud and
is scrolling search results on their phone. They see 3 small screenshots and
a title. That must be enough to tap.

### Step 5 — Preview video brief
- Duration: 15–30 seconds
- First 3 seconds: the hook (must work muted, no audio dependency)
- Show: the AI output, not the hardware (app store = software context)
- Must work: muted, with captions
- CTA: the last frame should invite a tap

### Step 6 — "What's New" copy (for updates)
For each release:
- What did the customer experience improve? (not what feature was added)
- Why does it matter to them?
- Format: 2–3 sentences, customer benefit language, no technical jargon

---

## Output format

```
# ASO Brief — [App name] [Version / Update]
Platform:    [iOS / Android / both]
Status:      [Draft | In Review | Locked]
Release:     [target App Store submission date]
Owner:       [PMM name]

---

## Keyword strategy
Primary keyword:    [highest volume, highest relevance]
Secondary keywords: [list with rationale]
iOS keyword field:  [100 chars, comma-separated, no spaces after commas]
NOT to target:      [keywords too competitive / irrelevant / trademark risk]

## Title
iOS (30 chars): [copy]
Android (50 chars): [copy]

## Subtitle / Short description
iOS subtitle (30 chars): [copy]
Android short description (80 chars): [copy]

## First 255 chars (above the fold)
[copy — must contain primary value prop + secondary keyword + curiosity hook]
Char count: [X/255]

## Full description structure
- Para 1 (255 chars, above fold): [primary value prop]
- Para 2: [key feature 1 — AI capability]
- Para 3: [key feature 2 — hardware advantage]
- Para 4: [key feature 3 — platform/system]
- Para 5: [social proof / user type]
- Para 6: [trust / privacy statement — from AI trust brief]
- Para 7: [CTA + website]

## Screenshot brief
| # | Screen shown | Caption copy | Position | Search-visible? |
|---|---|---|---|---|
| 1 | [screen] | [copy — chars] | [above/below] | Yes |
| 2 | | | | Yes |
| 3 | | | | Yes |
| 4–10 | | | | No |

## Preview video brief
Duration: [15-30 sec]
Hook (0–3s): [what happens — must work muted]
Middle (3–25s): [what AI output is shown]
End frame: [what the CTA frame shows]
Captions: required

## What's New copy (if update)
[2–3 sentences. Customer benefit language. No changelog format.]

## A/B test hypothesis (if applicable)
[What element to test, what the hypothesis is, how long to run]
```

---

## Hard rules

- **Title keyword is mandatory.** A title that's just the product name leaves
  keyword weight on the table. The App Store algorithm gives highest weight to
  the title. Use it.
- **First 255 chars are the description.** Write the description assuming most
  users never tap "More." The rest is for the algorithm and the minority who read.
- **Screenshots convert more than copy.** Invest more time in the screenshot brief
  than the description. The first 3 screenshots are the listing.
- **"What's New" is customer copy, not a changelog.** Engineering writes the
  changelog. PMM writes "What's New." Never swap them.
- **The AI trust brief feeds the description.** Any privacy or data claim in the
  App Store listing must appear in the locked AI trust brief. The App Store is
  a regulated environment — Apple reviews data claims.
