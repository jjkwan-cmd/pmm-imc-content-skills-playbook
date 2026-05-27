# PMM IMC Content Skills Playbook

A library of Claude skills for Plaud's PMM team — built to make AI-assisted work more structured, consistent, and repeatable across the full content lifecycle.

---

## Why this exists

Most of us jump straight into briefing or execution. We give AI some context, hope the output lands close enough, and adjust from there. That works for small tasks. For anything bigger — a product launch, a repositioning, a new narrative — it creates problems downstream.

When the upstream thinking is thin, everyone who depends on it (IMC, regional, design, DTC) has to fill in the gaps themselves. The result is inconsistent messaging, briefs that go back and forth, and content that doesn't hang together.

The skills in this playbook are built around a different idea: **brief is the cheapest asset in the whole pipeline.** Invest more time upstream, and everything downstream gets easier and more consistent.

One more thing worth saying upfront: **upstream thinking can't be outsourced to AI.** AI can help you go deeper, but the direction you give it is bounded by what you already know. The sharper your instincts and knowledge, the sharper the output. These skills give AI better instructions — they don't replace the judgment behind them.

---

## The workflow

Four phases. Not every project needs all four — use your judgment based on project size and how much is already locked.

```
EXPLORE → BRIEF → EXECUTE → CANON
```

### 1. Explore
Before any brief or copy, answer the core questions:
- Which segment are we serving? What do they believe today?
- What is the dominant narrative in this category?
- What do we want them to believe after?
- What is our competitive frame? Who are we really up against?
- What evidence do we have? What gaps exist?

Don't think about taglines, campaign concepts, or deliverables yet. Get the foundation right first.

**Skills:** `pmm-explore`, `pmm-capture`, `pmm-learning-opportunity`

### 2. Brief
Turn the exploration into a structured positioning brief. Lock the narrative, audience, message house, lexicon, and trade-offs before any execution begins.

A brief that's been properly built from the upstream is something the whole team — writers, designers, regional, DTC — can execute from without going back to you constantly.

**Skills:** `pmm-positioning-brief`, `pmm-gtm-brief`, `pmm-aso-brief`, `pmm-oobe-brief`, `pmm-demo-brief`, `pmm-ai-trust-brief`, `pmm-battle-card`, `pmm-hw-sw-narrative`

### 3. Execute
With a solid brief in hand, produce the downstream assets. The brief does the heavy lifting here — execution becomes faster and more consistent.

**Skills:** `pmm-write`, `pmm-ai-explainer`, `pmm-versus-page`, `imc-launch-video`, `plaud-copywriting-audit`

### 4. Canon
Before shipping, stress-test assets against the brief. Does the copy hold up to the narrative? Are the claims defensible? Is the lexicon consistent?

Think of this as governance — you are the source of the narrative, and this is where you protect it.

**Skills:** `pmm-review`, `pmm-peer-review`, `pmm-update-canon`

---

## Skills index

| Skill | Phase | What it does |
|-------|-------|-------------|
| `pmm-explore` | Explore | Asks structured questions to surface what you don't know before you brief |
| `pmm-capture` | Explore | Logs raw observations, insights, competitor moves, and ideas quickly |
| `pmm-learning-opportunity` | Explore | Breaks down concepts and frameworks AI surfaces that are worth understanding |
| `pmm-positioning-brief` | Brief | Full positioning framework: audience, value props, JTBD, message house, lexicon, narrative |
| `pmm-gtm-brief` | Brief | Go-to-market brief for a product or feature launch |
| `pmm-aso-brief` | Brief | App Store Optimization brief |
| `pmm-oobe-brief` | Brief | Out-of-box experience brief — maps the consumer journey from unboxing |
| `pmm-demo-brief` | Brief | Demo narrative and structure brief |
| `pmm-ai-trust-brief` | Brief | Brief for building AI credibility and trust messaging |
| `pmm-battle-card` | Brief | Competitive battle card — how we win against a specific narrative or competitor |
| `pmm-hw-sw-narrative` | Brief | Hardware and software narrative framework — how to tell the integrated product story |
| `pmm-write` | Execute | Drafts copy from a brief |
| `pmm-ai-explainer` | Execute | Explains complex AI features in plain, compelling language |
| `pmm-versus-page` | Execute | Comparison page — us vs. competitor or us vs. us (e.g. Sigma vs. Note Pro) |
| `imc-launch-video` | Execute | Launch video narrative and script brief |
| `plaud-copywriting-audit` | Execute | Audits copy for brand voice, accuracy, and consistency (includes Plaud-specific references) |
| `pmm-review` | Canon | Reviews an asset against its brief |
| `pmm-peer-review` | Canon | Structured peer review of a brief or asset |
| `pmm-update-canon` | Canon | Updates the message house, lexicon, and proof bank after a launch or positioning decision |

---

## How to use these skills in Claude Code

Run any skill with a slash command from your Claude Code session:

```
/pmm-explore
/pmm-gtm-brief
/plaud-copywriting-audit
```

Provide context before running — the more background you give (product, audience, business goal, what you already know), the better the output. These skills follow a fixed logic, so you always know what Claude is doing and why.

**In VS Code**, you can run multiple skill sessions in parallel terminals and compare outputs side by side — useful for exploring competing narratives or hypotheses at the same time.

---

## When to use the full workflow vs. a single skill

You don't need to run every step for every project.

| Project type | Approach |
|-------------|----------|
| New product launch or positioning | Run the full workflow: Explore → Brief → Execute → Canon |
| Feature update with locked messaging | Start at Execute; run audit before shipping |
| Copy check or refresh | Jump straight to `plaud-copywriting-audit` |
| Quick content piece with clear brief | `pmm-write` → `pmm-review` |
| Competitive question or new category | `pmm-explore` + `pmm-battle-card` |

---

## What makes upstream thinking good

A few things worth having an answer to before you write any brief:

1. **Who exactly are we talking to?** Not just "3H professionals" — what's the sharper cut within that group? What's their appetite for AI? What do they believe today?
2. **What is the dominant narrative in this category?** What story are customers already telling themselves?
3. **What do we want them to believe after?** Is it about capability, status, workflow transformation, something else?
4. **What is our competitive frame?** Who are the real alternatives — and how do we win that comparison?
5. **What evidence do we have?** 70% proof is enough to move forward. Waiting for 100% means nothing ships.

If you can answer these before opening a brief template, the brief writes itself.

---

*Maintained by the PMM team. Add new skills as the team's workflow evolves.*
