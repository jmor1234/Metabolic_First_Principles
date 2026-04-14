# Ray Peat — Reading Protocol

**What this is:** The protocol for reading Peat's articles with agent-assisted real-time stress testing against the metabolic framework vault. Use this as the operational spec for each session.

---

## The Goal

Two outputs from each article, in priority order:

1. **Deepened understanding.** You internalize Peat's reasoning pattern — how he moves between topics, how he traces connections — so that over time you hold the integration in working memory, not as reference material.

2. **Per-article study notes.** A structured document capturing what matters: what he got right, what was corrected, what's new, what reasoning chains are most instructive. This becomes a parallel vault alongside the framework — the record of how the integration was built and refined.

**Secondary output:** Candidate vault refinements. Things worth considering for the main vault — flagged, not automatically added. The bar for changing the vault is high (see `metabolic_framework/Verification Methodology.md`). Most things you find will enrich your per-article notes without justifying a vault change.

---

## Session Setup

Start each session with this prompt (copy-paste):

```
I'm reading Ray Peat's article "[ARTICLE TITLE]" at [URL]. I want to work through it with you
as an agent holding the metabolic_framework vault's full context.

Before we start, please:

1. Read metabolic_framework/CLAUDE.md — the vault's navigation spec
2. Read metabolic_framework/Foundation.md and metabolic_framework/The System.md — the
   structural tier that defines the framework's core claims
3. Read metabolic_framework/Verification Methodology.md — the epistemic discipline
   (three hypotheses, default position, causal independence audit, the three rules
   governing when acute/chronic and context-dependence can be invoked)
4. Read the Ray Peat — Historical Assessment.md for the quantitative baseline
5. Skim project_history/peat_claims_verified/[relevant topic].md to see the
   original claim-by-claim verification for this article's main topic

Then read the article itself.

Working style for this session:

- Default position: the vault is correct until proven otherwise
- When Peat says X, trace what the vault's reasoning chain predicts for that claim
- If Peat and the vault agree, note it and move on
- If they disagree, apply the Three Hypotheses in order:
  (1) am I misunderstanding the vault? (2) does the research measure something
  different? (3) is the vault actually wrong?
- If you find something genuinely new — a connection the vault doesn't model, a
  mechanism it doesn't address — flag it as a candidate refinement but do NOT
  automatically update the vault. Candidate refinements get captured in the
  per-article notes and reviewed separately.
- Be honest. Don't defend the vault if the evidence doesn't support it. Don't
  defend Peat if his reasoning breaks down. Don't soften conclusions to be diplomatic.
- Push back on me when I'm wrong. I'm learning the integration — I will say things
  that don't fit the vault's logic. Catch it.

We'll work through the article section by section where the reasoning matters.
Not every paragraph needs deep engagement — only the ones where he's making a
substantive claim, drawing a connection, or proposing a mechanism.

Output: when we finish, create peat_articles_study/[article-slug].md using the
template at the end of Ray Peat — Reading Protocol.md.

Ready when you are.
```

---

## During the Session

**Read the article yourself first, without the agent.** Note:
- What he's arguing (the core thesis of the piece)
- Where the reasoning moved in a way that surprised you
- Claims that feel important or contentious
- Connections he draws that you hadn't seen before

**Then engage the agent with specific passages.** Not a blanket "what do you think?" Point to specific claims: "He says here that X causes Y through mechanism Z. What does the vault say? Does the evidence support Z specifically, or is it actually Z'?"

**Watch for these patterns:**

- **Right destination, wrong route.** Peat's most common error. Correct functional outcome, wrong molecular pathway. When the agent says "the direction is right but the mechanism is [X] not [Y]" — that's this pattern. Note the correction, note what it reveals about how modern tools changed the picture.

- **Conditionality collapse.** Peat tends to flatten dual-identity molecules (melatonin, lactate, estrogen) into single poles. Watch for blanket claims about what something "is" — they usually need acute/chronic, dose, or context qualification.

- **Parallel marker vs. causal agent.** The CO₂→ATP pattern. When he attributes causation to an observable correlate, check whether the actual mechanism is something less observable running alongside it.

- **Integration that holds.** Not every claim fails. Where he connects thyroid to PUFA to estrogen to liver in one chain and the vault's independent verification confirms it — that's where he was doing something nobody else was. Note these explicitly.

**When in doubt, apply Verification Methodology.** The vault has a formal epistemic discipline for exactly this situation. Use it.

---

## Per-Article Output Template

Create `peat_articles_study/[article-slug].md` (lowercase, hyphenated). Example: `peat_articles_study/mitochondria-and-mortality.md`.

```markdown
---
article: "[Full title]"
url: [raypeat.com URL]
tier: [1-4 from Reading Guide]
topic: [primary vault topic — thyroid, PUFA, estrogen, etc.]
vault-cross-reference: [vault document]
date-read: YYYY-MM-DD
---

# [Article Title]

## The Core Argument

[2-4 sentences: what is he arguing in this piece? The thesis, not the details.]

## The Reasoning Chain

[How does he get there? Trace the logical moves. What connects to what?
This is the MOST IMPORTANT section — it captures his integration skill.
Do not just list claims — show how he moves between them.]

## What's Confirmed

[Claims where the vault agrees. Include the strongest examples — not every
confirmed claim, just the ones that matter most or that vindicate something
contrarian.]

- **[Claim]** — [brief: why it's confirmed, what evidence]
- ...

## What's Corrected

[Claims where the direction is right but the mechanism needs updating —
the "right destination, wrong route" pattern.]

- **[Claim]** — Peat's mechanism: [X]. Actual mechanism: [Y]. Why it matters: [Z].
- ...

## What's Contradicted

[Claims where the evidence directly reverses Peat's position. Rare — most
articles will have zero or one.]

- **[Claim]** — Peat says: [X]. Evidence shows: [Y]. Source: [paper].
- ...

## What's New to Me

[Connections Peat makes that the vault doesn't explicitly model, or
reasoning chains you hadn't seen before. These are the most valuable for
internalization — they're where you're learning something you didn't
already hold.]

- ...

## Candidate Vault Refinements

[Things worth considering for the main vault. Flagged, not decided.
Bar for changes is high — see Verification Methodology. Most candidates
will not become vault changes; they'll just live here as the record.]

- **[Candidate]** — [what it is, why it might warrant a change, what
  evidence would be needed to justify it]
- ...

## The One Thing Worth Remembering

[If you forgot everything else about this article in 6 months, what's the
one reasoning chain or insight you want to preserve? Write it in a way
that makes sense cold.]

## Session Notes

[Brief notes on the session itself — questions the agent couldn't answer,
places where your own pushback produced an insight, anything worth
flagging for future sessions.]
```

---

## When to Consider a Vault Refinement

A candidate becomes a real proposed refinement only when:

1. You can state precisely what the vault currently says and what the new claim would be
2. You have verified evidence for the new claim that survives the Three Hypotheses check
3. The change would make the vault MORE specific, not more vague (per Rule 3 in Verification Methodology)
4. The core claims survive intact (the five numbered claims in Verification Methodology)

When those four conditions are met, flag it as a formal refinement proposal. Then evaluate it as its own stress test — don't just absorb it because it sounds right.

**Most "candidate refinements" will fail these checks.** That's fine. They still belong in the per-article notes as part of the record. The bar for the main vault is deliberately high.

---

## After Each Article

Two questions before closing the session:

1. **What did I learn about how Peat thinks that I didn't already know?** Not what he said — how he reasons. This is the skill you're trying to acquire.

2. **What should I read next, given what this article surfaced?** Sometimes the Reading Guide order will hold. Sometimes an article will point strongly toward another one (e.g., reading Mitochondria and Mortality may make reading Lactate vs. CO₂ the natural next step rather than When Energy Fails). Let the reading evolve.

---

## Operational Notes

- The `peat_articles_study/` directory should be created on the first article read. It parallels `project_history/peat_claims_verified/` but is organized by article, not by topic.
- Commit after each article. One article = one commit. Keeps history clean.
- Don't skip the "What's New to Me" section even when it feels redundant. This is where your integration is growing.
- The agent will sometimes tell you a claim you thought was novel is already in the vault. That's normal and good — it means the vault is dense. Note it and move on.
- If an article takes more than one session, that's fine. Close the session, resume with the same prompt on the next article-relevant document.

---

## Why This Protocol Works

The protocol's structure mirrors what produced the vault in the first place: extract Peat's reasoning honestly, verify each load-bearing claim against evidence, calibrate conclusions without bias, capture what survives and what doesn't. The difference is that you're now the one holding the context, with agents as the research and verification tool rather than agents holding the context while you manage them from outside.

The more articles you work through, the more the integration moves from the vault into your head. Eventually you won't need the protocol explicitly — the epistemic discipline will be intuition. That's the point.
