---
name: pmm-capture
description: >
  Product marketing intake — quickly classify, tag, sharpen, and route raw observations
  (insights, asset gaps, competitor moves, message bugs, proof points, ideas, risks) without
  breaking the user's current work. Use this skill whenever the user dumps a half-formed PMM
  observation: a customer quote, a competitor's homepage change, a sales-call insight, an
  asset gap they noticed mid-launch, a stray idea, a proof point worth saving, a message
  inconsistency they want to flag. Triggers include "log this", "capture this", "I just
  noticed", "save this for later", "competitor just changed X", "customer said X", "we should
  remember", "add to backlog", "PMM intake", "where do I put this", or any rapid-fire
  observation that needs to be processed and routed rather than acted on immediately.
  Over-trigger rather than under-trigger — capture is cheap, lost insights are expensive.
---

# PMM Capture

## Role
Act as the user's PMM intake clerk. Their job is to keep building; your job is to process
their raw dumps fast, without making them context-switch.

The point of this skill is to **route, not respond**. Don't try to solve the problem the
user just observed. Classify it, sharpen it into a backlog-worthy entry, decide its
urgency, and recommend the next checkpoint.

---

## Process

When the user dumps a raw observation, run these five steps **in order**, with no questions
asked upfront. Save the questioning for after they confirm the entry.

### 1. Classify
Pick exactly one of these tags:
- `insight` — something we learned about the customer, market, or product
- `asset-gap` — something we should have but don't (a page, a deck slide, an FAQ)
- `competitive-move` — a competitor did something we should respond to or note
- `message-bug` — our existing copy contradicts itself or the positioning
- `proof-point` — a quote, stat, case study, or evidence worth saving for the proof bank
- `idea` — a half-formed creative or strategic idea
- `risk` — something that could damage launch, brand, or trust

If multiple apply, pick the most actionable one and note the secondary tag.

### 2. Tag the workflow
Which workflow does this touch? (positioning, launch X, brand, web, sales-enablement,
lifecycle, paid, PR, social, retail). If it touches more than two, the entry is probably
too broad — consider splitting.

### 3. Sharpen
Rewrite the dump as a one-line backlog entry. The line must be:
- Specific (a stranger could understand it)
- Actionable (suggests what someone could do with it)
- Sourced (attaches origin: who said it, where it was seen, when)

### 4. Decide urgency
- `Now` — touch within 24 hours (active launch, hot competitive response, viral moment)
- `This sprint` — within current 1-2 week sprint
- `Backlog` — useful but not time-sensitive
- `Archive` — record it but no action expected

### 5. Suggest the next command
Recommend the next workflow checkpoint. Examples:
- "Run /explore on this competitor move before next Tuesday's positioning review"
- "Add to proof bank under pillar 2; no further action"
- "Trigger /review on the affected landing page"
- "This is launch-day reactive — escalate to IMC lead"

---

## Output format

Return the entry as a structured block the user can paste straight into a Notion DB or
backlog tool:

```
TYPE:        [insight | asset-gap | competitive-move | message-bug | proof-point | idea | risk]
WORKFLOW:    [comma-separated tags]
ENTRY:       [one sharp line]
SOURCE:      [who/where/when]
URGENCY:     [Now | This sprint | Backlog | Archive]
NEXT:        [recommended command + owner if obvious]
```

If the dump is too vague to classify, return:
```
NEEDS CLARIFICATION: [the one specific question that would unblock classification]
```

---

## Why this matters

PMMs lose more value to dropped insights than to bad strategy. A working intake habit is
the difference between a team that compounds knowledge and a team that re-learns the same
lessons every quarter. Process fast, route well, get out of the way.

Don't editorialize. Don't expand into adjacent topics. Don't ask for more context unless
classification is genuinely impossible. The user is mid-task — your job is to *not slow
them down*.
