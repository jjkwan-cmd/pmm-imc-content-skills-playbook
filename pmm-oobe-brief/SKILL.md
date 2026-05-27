---
name: pmm-oobe-brief
description: >
  Build the out-of-box experience (OOBE) brief — the PMM specification for what the
  customer experiences from the moment they open the packaging to the moment they
  get their first piece of value from the device. Consumer electronics specific.
  The unboxing is marketing. The first 10 minutes of use determines word of mouth,
  review scores, and return rates more than any ad campaign. Triggers include "OOBE",
  "out of box experience", "unboxing brief", "first use experience", "setup flow",
  "day one experience", "activation brief", "onboarding brief for hardware",
  "first 10 minutes", or any request to brief or plan what happens between
  "customer opens the box" and "customer gets first value."
---

# PMM OOBE Brief

## Role
Act as the user's First Experience Lead. The OOBE brief is the PMM brief that most
consumer electronics teams skip — and it's the one that determines whether the
customer recommends the product or returns it. Apple spends more on packaging and
OOBE than most companies spend on advertising. The first experience is the product.

---

## Why OOBE is a PMM deliverable

The OOBE brief sits at the intersection of:
- **Packaging** (what the customer sees before they open it)
- **Hardware design** (what they find inside)
- **Software onboarding** (the app setup flow)
- **AI expectation setting** (when and how the AI value appears for the first time)
- **Support deflection** (every question the OOBE doesn't answer becomes a ticket)

PMM's job is not to design the flow — that's product and design. PMM's job is to
brief what the customer must believe, feel, and accomplish at each stage of
the OOBE, so the product and design teams can execute against those outcomes.

---

## The OOBE stages for a hardware + AI product

**Stage 0 — Pre-unboxing**: The box in hand before it's opened. Weight, size, feel.
The external packaging sets the expectation for what's inside.

**Stage 1 — Unboxing**: The first 60 seconds. What do they see? What order do
they find things? Is there delight in the reveal? Or confusion?

**Stage 2 — Physical setup**: Getting the device ready. Charging, pairing,
initial configuration. Every step that causes friction here is a return risk.

**Stage 3 — App / platform pairing**: Connecting device to app to platform.
The moment where hardware meets software. Most AI device returns happen here.

**Stage 4 — First capture**: The customer's first recording. This is the most
important moment in the OOBE. It must be easy, fast, and produce a result
that demonstrates value within minutes.

**Stage 5 — First AI output**: The moment the AI delivers its first summary,
transcript, or action item. This is the product promise fulfilled. If this
moment is delayed, underwhelming, or confusing — the product fails the OOBE
regardless of quality.

**Stage 6 — Day 2–7 habit formation**: Belonging to OOBE extended. The second
and third uses that determine whether the product becomes a habit or a drawer item.

---

## Process

### Step 1 — OOBE outcome definition
For each stage, define:
- What must the customer be able to DO? (functional outcome)
- What must the customer BELIEVE? (cognitive outcome)
- What must the customer FEEL? (emotional outcome)

### Step 2 — Friction map
Map every point of potential friction in the current OOBE:
- Steps that require the customer to read an instruction
- Steps where the app and device are not in sync
- Steps where the AI value is not yet visible
- Steps where the customer might give up

Prioritize by: frequency × severity. Fix the high-frequency, high-severity
friction first. These are your return rates and 1-star reviews.

### Step 3 — The "first value moment" specification
Name exactly when and how the customer gets their first piece of AI value.
This is the OOBE's most important moment and must be:
- Fast (within the first 10 minutes of use)
- Clear (the customer knows what the AI did)
- Impressive (the output is better than expected from the setup experience)
- Repeatable (the customer immediately knows how to get it again)

### Step 4 — In-box content brief
Everything in the box is a PMM deliverable:
- Quick start card: what the customer must accomplish in 5 steps
- Welcome card: one sentence that restates the promise the customer just bought
- Packaging copy (inner tray): what they read as they unbox
- "What's in the box" diagram: what's included, named correctly per naming guide

### Step 5 — App onboarding flow brief
For the software side of the OOBE:
- What permissions must be granted? (microphone, notifications, etc.)
- In what order?
- What does the customer see while waiting for each permission?
- How does the app explain what it needs and why?
- What is the first screen the customer sees after setup?
- What action does that screen invite them to take?

---

## Output format

```
# OOBE Brief — [Product name]
Product:     [hardware + software/platform]
Status:      [Draft | Design Review | Locked]
Owner:       [PMM name — but cross-functional: product, design, packaging, CS]
Linked briefs: [hw-sw narrative, AI explainer, AI trust brief]

---

## Stage-by-stage outcomes

| Stage | Customer action | Must DO | Must BELIEVE | Must FEEL |
|---|---|---|---|---|
| 0 Pre-unbox | Sees the box | [outcome] | [belief] | [feeling] |
| 1 Unboxing | Opens box | | | |
| 2 Physical setup | Charges/pairs | | | |
| 3 App pairing | Connects to platform | | | |
| 4 First capture | Makes first recording | | | |
| 5 First AI output | Sees first AI result | [outcome] | [belief] | [feeling] |
| 6 Day 2-7 | Returns and records again | | | |

## First value moment specification
Time from box open to first AI output: [target: X minutes]
What the customer sees: [specific — not "a summary" but the exact output type]
Why it's impressive: [what makes this better than expected]
How they repeat it: [the action that gets them the next AI output]

## Friction map
| Stage | Friction point | Frequency | Severity | Fix required before launch? |
|---|---|---|---|---|

## In-box content brief
Quick start card:
- Step 1: [action]
- Step 2: [action]
- Step 3: [action]
- Step 4: [action]
- Step 5: first AI output visible

Welcome card copy: [one sentence — the promise restated]
Inner tray copy: [what they read as they reveal the device]
What's in the box list: [named per naming guide]

## App onboarding flow brief
Permission 1: [what, why, what the screen says while waiting]
Permission 2: [what, why, what the screen says while waiting]
First screen post-setup: [what the customer sees]
First invited action: [what the app asks them to do]
First AI value delivery: [when and how]

## Definition of done
- [ ] First value moment achieved in under [X] minutes
- [ ] Zero steps requiring the customer to read a full instruction manual
- [ ] AI explainer brief consulted for first AI output moment
- [ ] AI trust brief consulted for permissions flow language
- [ ] Naming guide consulted for all in-box content
- [ ] CS consulted — top 5 setup support tickets addressed in the OOBE
```

---

## Hard rules

- **The first AI output must occur within the first 10 minutes of use.**
  If it takes longer, the customer has already formed their initial judgment
  of the product based on the setup experience — not the AI experience.
- **CS must be consulted.** The top 5 setup support tickets are the top 5 OOBE
  failures. Fix them in the brief before they become returns.
- **The welcome card is a PMM deliverable.** It is not packaging decoration.
  It is the last brand touchpoint before the customer uses the product for the
  first time. It must restate the promise in the customer's language.
- **The in-box experience must be consistent with the promise on the box.**
  If the packaging says "AI that works immediately" and setup takes 20 minutes,
  the OOBE breaks trust before the customer makes their first recording.
