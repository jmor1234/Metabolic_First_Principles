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

Start each session with this prompt (copy-paste). The prompt loads all vault
context first; send the article separately after the agent confirms it's ready.

```
I'm starting a Ray Peat article reading session. I'll send you the article
(URL or text) after you've loaded the vault context. I want to work through
it with you as an agent holding the metabolic_framework vault's full context,
applying the bidirectional stress testing protocol.

Before I send the article, please load:

1. CLAUDE.md (project root) — workspace overview
2. Ray Peat — Reading Protocol.md — the operational spec for this session
   (read it fully; it defines the working style and the per-article output
   template you'll produce at the end)
3. Ray Peat — Historical Assessment.md — the quantitative baseline for what
   Peat got right and wrong
4. metabolic_framework/CLAUDE.md — the vault's navigation spec
5. metabolic_framework/Foundation.md and metabolic_framework/The System.md —
   the structural tier defining the framework's core claims
6. metabolic_framework/Verification Methodology.md — the epistemic discipline
   (three hypotheses, default position, causal independence audit, the three
   rules, citation deployment audit)

Once you've loaded these, confirm you're ready and briefly state:
- Your understanding of the bidirectional stress testing protocol
- That you'll treat both Peat and the vault as simultaneously under test,
  with primary literature (via WebSearch/WebFetch) as the arbiter for
  load-bearing claims
- That you'll catch me when I'm wrong

Then I'll send the article. When the article arrives:
- Identify the primary vault topic (thyroid, PUFA, estrogen, etc.) and
  skim project_history/peat_claims_verified/[that topic].md for the
  original claim-by-claim verification context
- Read the article itself
- Let me know you're ready to work through it

Working style for this session — BIDIRECTIONAL STRESS TESTING:

Both Peat AND the vault are under test. Neither gets the benefit of the doubt.
The arbiter is primary literature, verified in real time when a claim is
load-bearing.

- When Peat and the vault agree on something substantive, stress-test the
  agreement against primary literature via WebSearch/WebFetch. Convergence on
  a wrong answer is still wrong.
- When Peat and the vault disagree, apply the Three Hypotheses in order:
  (1) am I misunderstanding the vault? (2) does the research measure something
  different? (3) is one of them actually wrong?
- The vault has a default-correct presumption because it's been verified — but
  that presumption is rebuttable by primary literature, as demonstrated by the
  CO₂→ATP refinement this session produced.
- When Peat makes a claim the vault doesn't address, don't just note it — test
  it directly against current primary literature. Real-time WebSearch for the
  specific mechanism. Fetch the actual papers. Peat may be surfacing something
  the verification process missed, or making a claim modern evidence now
  contradicts.
- When the vault makes a claim that goes beyond Peat, same discipline — verify
  it against primary sources. The vault's corrections are themselves claims
  subject to verification.
- If real-time literature verification produces a refinement candidate for
  either the vault or the per-article notes, flag it clearly. Do NOT
  automatically update the vault. Candidate refinements get captured in the
  per-article notes and reviewed separately against the bar in Verification
  Methodology.
- Be honest. Don't defend the vault if the evidence doesn't support it. Don't
  defend Peat if his reasoning breaks down. Don't soften conclusions to be
  diplomatic. Convergent wrongness is still wrong.
- Push back on me when I'm wrong. I'm learning the integration — I will say
  things that don't fit the vault's logic or the evidence. Catch it.

Real-time verification tools:
- WebSearch for finding primary literature on specific claims
- WebFetch for reading actual papers (prefer PMC full text over abstracts)
- When a claim is load-bearing (a core mechanism, a causal chain, a specific
  quantitative prediction), verify it directly rather than relying on the
  vault's citations alone. The CO₂ stress test in this repo is the template.

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

**Watch for these patterns (in Peat):**

- **Right destination, wrong route.** Peat's most common error. Correct functional outcome, wrong molecular pathway. When the agent says "the direction is right but the mechanism is [X] not [Y]" — that's this pattern. Note the correction, note what it reveals about how modern tools changed the picture.

- **Conditionality collapse.** Peat tends to flatten dual-identity molecules (melatonin, lactate, estrogen) into single poles. Watch for blanket claims about what something "is" — they usually need acute/chronic, dose, or context qualification.

- **Parallel marker vs. causal agent.** The CO₂→ATP pattern. When he attributes causation to an observable correlate, check whether the actual mechanism is something less observable running alongside it.

- **Integration that holds.** Not every claim fails. Where he connects thyroid to PUFA to estrogen to liver in one chain and the vault's independent verification confirms it — that's where he was doing something nobody else was. Note these explicitly.

**Watch for these patterns (in the vault):**

- **Overcorrection.** The vault may have swung too far in correcting Peat. The CO₂ stress test found this — "parallel marker" was slightly too strong because CO₂ has genuine independent mechanisms at other targets. When the vault's correction feels absolute, check whether the actual literature supports that level of certainty.

- **Citation deployment errors.** The vault cites papers for specific claims. The paper may be topically relevant but not actually test the scenario the vault is claiming. Verification Methodology's "citation deployment audit" catches this. Apply it when a vault claim feels surprisingly confident.

- **Gaps in coverage.** Peat may raise a connection or mechanism the vault doesn't address at all. That's not necessarily a failure of the vault — it's a candidate for expansion. Flag it, test it against primary literature, then evaluate whether it belongs in the vault.

- **Stale corrections.** The vault's last-verified date matters. A correction from 2024 may have been superseded by 2025-2026 evidence. When a correction is load-bearing, check whether more recent literature affects it.

**When in doubt, apply Verification Methodology.** The vault has a formal epistemic discipline for exactly this situation. Use it bidirectionally — it applies to testing Peat's claims AND testing the vault's corrections.

---

## Bidirectional Stress Testing — How It Actually Works

The core move is refusing to treat any source as authoritative on its own terms. Peat, the vault, and the verification documents are all TESTIMONY about what primary literature shows. The literature itself is the arbiter.

**For any load-bearing claim in the article, the test has four positions:**

1. **Peat says X. Vault agrees with X.** Still stress-test via real-time primary literature when X is load-bearing. Convergence doesn't prove correctness. This is how the CO₂ refinement surfaced — both Peat and the vault's non-loop framing were partly right, but primary literature revealed a more precise picture neither had fully captured.

2. **Peat says X. Vault says Y (correction).** Stress-test BOTH via primary literature. Don't default to the vault; verify the correction is itself supported. The vault has been verified, but verification was done at a point in time — new evidence or missed evidence can update it.

3. **Peat says X. Vault doesn't address X.** Stress-test X directly. If it holds, it's a candidate for vault expansion. If it doesn't, it's a Peat error the verification may have missed.

4. **Vault says Y. Peat doesn't address Y.** The vault's corrections sometimes go beyond Peat — citing mechanisms he never discussed. Verify these too. The vault is not automatically right about things Peat didn't say.

**The tooling loop for real-time verification:**

1. Identify the load-bearing claim precisely. Not "estrogen is bad" — "estrogen shifts cells toward glycolysis via PI3K/AKT at physiological concentrations."
2. WebSearch for primary literature on the specific claim. Prefer recent (2020+) reviews and primary research over older citations.
3. WebFetch the actual papers. Prefer PMC full text over abstracts. Read what the paper actually tested, measured, and concluded.
4. Apply the citation deployment audit (Verification Methodology Step 5): species match, scenario match, endpoint match, proposed-mechanism match.
5. Form a verdict based on what the literature actually shows — not what the vault says or what Peat says. Either may turn out right, wrong, or partially right.

**Budget:** Not every claim warrants real-time verification. Textbook claims (Krebs cycle, Bohr effect) don't. Claims where Peat and the vault agree and the agreement matches well-established biology don't. The trigger for verification is: **load-bearing + non-obvious + not already stress-tested** in prior project work.

**Output:** Every real-time verification produces a note in the per-article document specifying what was verified, what the literature showed, and what the verdict is. This builds the evidence trail that either strengthens the existing vault, surfaces candidate refinements, or flags things worth deeper investigation later.

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

## Real-Time Verification Log

[Every claim that triggered real-time primary literature verification during
the session. One entry per verified claim. This is the evidence trail.]

### [Claim 1, stated precisely]
- **Peat's position:** [what he says]
- **Vault's position:** [what the vault says, or "not addressed"]
- **Literature searched:** [search terms, papers fetched]
- **What the evidence shows:** [synthesis of what the primary literature actually demonstrates]
- **Verdict:** [confirmed / corrected / contradicted / ambiguous — applies to Peat AND vault separately]
- **Implications:** [does this change anything? vault refinement candidate? Peat error the vault already caught? new finding?]

### [Claim 2, stated precisely]
...

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
