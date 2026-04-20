---
title: "Methodology"
aliases:
  - Evidence Standards
  - How to Read
  - How to Contribute
tags:
  - structural/meta
  - framework/metabolic
role: methodology
confidence: high
last-verified: 2026-04-10
scope: meta
connections:
  - "[[Foundation]]"
  - "[[The System]]"
  - "[[Practice]]"
---

> [!abstract] Essence
> This is one of two meta-layer documents that make the vault trustworthy rather than merely interesting: it governs how the knowledge was produced, what standards regulate it, how to navigate it, and how it grows (the companion [[Verification Methodology]] governs how the vault is tested, verified, and changed).
> Five evidence standards control what enters the vault: (1) evidence sourced, not remembered — every specific factual claim has a verifiable source (PubMed, DOI, institutional URL); training data and general knowledge do not count; (2) honest calibration over advocacy — forcing every finding into "confirmed" is as dishonest as dismissing every finding as "unproven," and the "Where the Evidence Is Complex" section in every doc flags genuine challenges; (3) mechanism over authority — evidence determines confidence, not source; (4) integration must be honest — overstating connections destroys the integration; (5) corrections are features, not failures — a vault that cannot be corrected is ideology, not knowledge.
> Two confidence scales operate at different levels: document-level (frontmatter `confidence` field: high / moderate / emerging / theoretical) applies to the doc as a whole, and claim-level (inline `[!warning]` callouts: textbook / strong / probable / plausible / speculative / contested) flags specific sub-claims — a document with "high" confidence may contain individual claims at "probable" or "speculative" because no biological topic is uniformly established at every level of detail.
> The mechanism-doc template is structurally identical across the vault (frontmatter → opening → How It Works → System Connections → Where the Evidence Is Complex → Research Context → Practical Implications), uses only four approved callouts (`[!abstract]`, `[!example]`, `[!warning]`, `[!tip]`), and the five-step expansion process (search existing references → verify against current research in real-time → write using the template → connect to the existing network → update structural docs if needed) is how new topics are added.
> The vault is evidence synthesis, not clinical guidance; it can be wrong, and the confidence calibration system exists because no synthesis of this scope is perfectly accurate — the integration (seeing how findings from endocrinology, hepatology, oncology, neurology, cell biology, and immunology describe the same underlying system) is the contribution, not the findings themselves, which belong to the researchers who produced them.

Every other document in this vault answers questions about biology. This document answers questions about the vault itself: how the knowledge was produced, what standards govern it, how to navigate it, how to evaluate its claims, and how it grows. It is one of two meta-layer documents — the one covering evidence standards, navigation, and the expansion process. Its companion [[Verification Methodology]] governs how the vault is tested, verified, and changed. Together they make the vault trustworthy rather than merely interesting.

---

## How This Vault Was Built

The knowledge in this vault was produced through a systematic verification project that tested metabolic claims against peer-reviewed research. Each mechanism was extracted from primary sources, then verified claim-by-claim against the best available evidence — not summarized, not paraphrased, but independently checked against published data.

The verification archive exists separately from this vault. It contains the raw claim extractions, the research landscape analysis for each topic, the individual claim assessments, and the corrections documented along the way. That archive is the audit trail.

This vault extracts the verified findings from that project and presents them as standalone knowledge, organized around the biology itself rather than around any single person's framework or claims. The structure follows the biology: how the system works, what its components are, how they connect, what to do about it. The provenance is documented here. The knowledge stands on its own.

The vault is not advocacy for a position. It is calibrated assessment. Some findings were confirmed strongly by modern research. Some were refined — the direction was right but the mechanism needed correction. Some were contradicted outright. All of these outcomes are documented honestly, because a vault that only confirms is not a verification — it is marketing.

---

## Evidence Standards

Five principles govern what enters this vault and how it is presented.

**1. Evidence sourced, not remembered.**

Every specific factual claim must have a verifiable source — a PubMed link, a DOI, an institutional URL. Training data and general knowledge are not evidence. When a claim matters, it must be traceable. The vault's credibility depends on the reader being able to verify any claim independently.

General biochemistry — the Krebs cycle, the Bohr effect, the electron transport chain — can be stated without citation. These are textbook knowledge taught in every biochemistry course. Specific findings — ferroptosis discovered 2012, ETCO2 lower in hypothyroidism, 670nm red light reducing blood glucose 27.7% — require sourced references. The line is: could a skeptical reader with PubMed access verify this claim? If the answer depends on a specific paper, cite the paper.

**2. Honest calibration over advocacy.**

The vault distinguishes what is established from what is probable from what is speculative. Forcing every finding into "confirmed" is as dishonest as dismissing every finding as "unproven." The "Where the Evidence Is Complex" section in every mechanism document exists specifically to flag genuine challenges, contradictions, and limitations.

If a finding is contradicted — acute lactate is neuroprotective, not excitotoxic — it is stated as contradicted. If a mechanism correction is needed — estrogen's glycolytic shift operates via PI3K/AKT signaling, not direct Complex IV blockade; progesterone depletion under stress is HPA axis suppression, not substrate competition — the correction is documented. These are features of honest science, not failures of it.

**3. Mechanism over authority.**

The vault cares about HOW things work, not WHO said they work. No argument from authority — not from researchers, institutions, or historical figures. A mechanism confirmed by a 2019 Nature paper and a mechanism proposed by an independent thinker carry the same weight IF they are verified against the same evidence standard. The evidence determines the confidence level, not the source.

**4. Integration must be honest.**

The vault's primary contribution is integration — seeing how mechanisms connect across disciplines that do not cite each other. But integration must connect things that genuinely connect, not force parallels. When the connection between two mechanisms is mechanistically confirmed (CO2 pH shifts → serotonin granule destabilization), it is stated as confirmed. When it is mechanistically plausible but untested as an integrated system (the full CO2→serotonin suppression chain operating in vivo), it is stated as untested. The integration is the contribution. Overstating the integration destroys it.

**5. Corrections are features, not failures.**

The vault improves by finding where it is wrong. When a mechanism correction is identified, the correction is documented and the understanding deepens. A vault that cannot be corrected is ideology, not knowledge. The `last-verified` date in every document's frontmatter exists specifically to signal when each document's evidence was last checked against current literature. If that date is old, the document is due for review.

---

## Confidence Calibration

Two scales operate at different levels.

**Document-level confidence** is recorded in the frontmatter `confidence` field. It applies to the document as a whole — the overall reliability of its core claims.

- **high** — Core mechanisms well-established. Corrections are refinements, not refutations. Multiple independent evidence lines converge. All current structural and mechanism documents carry this rating.
- **moderate** — Direction is supported but significant nuances, gaps, or unresolved contradictions exist.
- **emerging** — Mechanism is plausible and evidence is accumulating but not yet definitive.
- **theoretical** — Hypothesized from first principles but lacks direct evidence.

**Claim-level confidence** appears within mechanism documents, primarily in the "Where the Evidence Is Complex" sections. It uses `[!warning]` callouts to flag specific claims at each level:

- **Textbook** — Standard biochemistry. Taught in courses, not seriously contested. The Fenton reaction, the Bohr effect, the Randle cycle mechanism.
- **Strong** — Confirmed by multiple independent research groups with consistent results. Ferroptosis, lactylation, resmetirom mechanism, PUFA-cardiolipin remodeling.
- **Probable** — Mechanistically sound with supporting evidence, not yet definitive. The metabolism-serotonin axis (ATP/V-ATPase-mediated mediator sequestration) as an integrated system, MCAS as downstream metabolic output.
- **Plausible** — Logical from first principles, limited direct evidence. The carbamino aldehyde protection hypothesis.
- **Speculative** — Interesting hypothesis, insufficient data. CO2 methylation/epigenetics.
- **Contested** — Genuine scientific disagreement with evidence on both sides. Estrogen fracture reduction versus confirmed estrogen damage mechanisms.

The two scales interact naturally: a document with "high" confidence may contain individual claims at "probable" or "speculative." The document is reliable overall while specific sub-claims are flagged. This is normal. No biological topic is uniformly established at every level of detail.

---

## How to Read the Vault

The vault is organized in tiers. Read top-down for understanding, or enter at any point for targeted lookup.

**Tier 1: Foundation (start here)**

- [[Foundation]] — What health and disease are. The thesis. The evidence. The challenges.
- [[The System]] — How the system produces two stable states. The architecture.
- These two documents provide ~80% of the conceptual understanding. Always start here.

**Tier 2: Mechanisms (the detailed biology)**

Nine documents covering the components of the system, grouped by biological reality:

1. [[The Master Throttle]] — Thyroid (T3)
2. [[The Preferred Substrate]] — Glucose / Randle cycle
3. [[The Metabolic Fork]] — CO₂ + Lactate
4. [[Membrane Damage and Defense]] — PUFA + Iron + Vitamin E
5. [[The Hormonal Axis]] — Estrogen + Progesterone
6. [[Conservation Signaling]] — Serotonin + Histamine
7. [[The Gut-Liver Axis]] — Endotoxin + Liver
8. [[The Cellular Readout]] — Calcium
9. [[The Temporal Dimension]] — Circadian

Read in order for the logical flow: throttle → substrate → fork → damage → regulation → signaling → gateway → readout → time. Or read any single document for targeted understanding — each is self-contained with wikilinks to context.

**Tier 3: Application**

- [[Practice]] — What to do. Interventions, monitoring, sequence.

**Tier 4: Meta**

- [[Methodology]] — How the vault works: evidence standards, confidence calibration, document template, expansion process.
- [[Verification Methodology]] — How the vault is tested and changed: default position, three hypotheses, bar for changes, verification sequence, research standards, three rules for evaluating contradictions.

> [!tip] Following wikilinks
> Mechanism docs reference each other extensively. Follow wikilinks to the canonical treatment of any mechanism mentioned in passing — don't re-read what a wikilink can navigate to. Grouped mechanism docs have aliases for their component topics: [[PUFA]], [[Iron]], [[Vitamin E]], [[Ferroptosis]] all resolve to [[Membrane Damage and Defense]]. [[Serotonin]] and [[Histamine]] resolve to [[Conservation Signaling]]. Use the natural topic name — the aliases handle routing.

---

## The Document Template

Every mechanism document follows the same structure. This template governs both existing documents and future additions.

**Frontmatter:**

```yaml
---
title: "[Document Title]"
aliases:
  - [Component names for wikilink resolution]
tags:
  - mechanism/[name]
  - framework/metabolic
role: mechanism
confidence: [high/moderate/emerging/theoretical]
last-verified: [YYYY-MM-DD]
scope: mechanistic
connections:
  - "[[Foundation]]"
  - "[[The System]]"
  - [other mechanism docs this document connects to]
---
```

**Body sections, in order:**

1. **Opening** (no heading) — What this mechanism is and its role in the system. Two to three paragraphs. Links to [[Foundation]] and [[The System]].
2. **## How It Works** — The verified biology, organized by mechanism. Subsections for merged docs. Inline citations for specific findings. This is the bulk of the document.
3. **## System Connections** — Table or structured list of connections to other mechanism docs. What the connection is and which direction it operates.
4. **## Where the Evidence Is Complex** — Honest calibration. What is textbook versus probable versus speculative. Key corrections. Uses `[!warning]` callouts.
5. **## Research Context** — Funding structures, chemical conflation, design distortions, why the fragmented picture persists for this specific topic.
6. **## Practical Implications** — Brief (3-5 bullet points), linking to [[Practice]].

**Callout types (only these four):**

- `[!abstract]` — Section summaries, key takeaways
- `[!example]` — Concrete evidence with citation
- `[!warning]` — Honest calibration: challenges, limitations, uncertainty
- `[!tip]` — Practical implications, navigation

**Tag taxonomy:**

- `structural/entry`, `structural/system`, `structural/practice`, `structural/meta` — Tier 1, 3, and 4 documents
- `mechanism/[name]` — Mechanism documents
- `framework/metabolic` — All files in the vault

---

## How to Expand the Vault

The vault currently covers nine mechanism groupings. It can grow. The process:

**Step 1: Search existing references.** Before writing a new mechanism document, search the existing vault for how the topic is already mentioned. Check System Connections tables. The new topic likely already appears in passing throughout the vault — those references tell you which existing documents need wikilinks to the new one and which mechanisms are already partially documented.

**Step 2: Verify against current research.** Every factual claim about the research landscape must be verified from real-time sources, not training data. Fetch the actual papers. Read the actual findings. Note the actual funding sources. This is the most time-intensive step and the one that produces the most value.

**Step 3: Write using the template.** Follow the document template above. Open with the mechanism's role in the system. Organize "How It Works" by mechanism, not by historical claims. Include honest calibration. Source everything specific.

**Step 4: Connect to the existing network.** Update the new document's System Connections table. Update existing documents' System Connections tables to reference the new topic. Add wikilinks where the new topic is mentioned in other documents. Update [[The System]] component table if the new topic represents a genuinely new system component.

**Step 5: Update structural docs if needed.** If the new topic reveals a new feedback loop, update [[The System]]. If it has practical implications beyond what [[Practice]] covers, update [[Practice]]. If it changes the overall thesis, update [[Foundation]] — though this should be rare for a well-established framework.

> [!abstract] Potential future topics
> Cholesterol as substrate and signaling molecule. Dopamine and prolactin as metabolic regulators. NAD+ metabolism and sirtuins. Altitude and metabolic optimization. Water, cellular swelling, and the structured state. Pregnenolone and DHEA as neurosteroids. The microbiome beyond endotoxin. Connective tissue and extracellular matrix.

---

## Scope and Limitations

**This vault is evidence synthesis, not clinical guidance.** It integrates peer-reviewed findings into a coherent metabolic framework. It does not diagnose conditions, prescribe treatments, or replace clinical judgment. Individual medical decisions require clinical context — the patient's history, current medications, comorbidities, and practitioner assessment — that no document can provide.

**The vault can be wrong.** The confidence calibration system exists because no synthesis of this scope is perfectly accurate. Some claims rated "probable" will turn out to be wrong. Some corrections documented today will themselves be corrected by future research. The vault improves through correction, not through defense of its current state. If you find an error, the response is to update the document, not to explain why the document was right all along.

**Integration is the contribution, not the findings.** The individual findings in this vault are published in peer-reviewed journals. Most are not controversial within their home disciplines. What the vault adds is integration — seeing how findings from endocrinology, hepatology, oncology, neurology, cell biology, and immunology describe the same underlying system. The integration is the intellectual work. The evidence belongs to the researchers who produced it.

---

## On the Essence Callouts

Every canonical doc in this vault (structural, mechanism, application, and meta tiers) opens with an `[!abstract] Essence` callout — a 4-5 sentence prose distillation that includes what the component IS, its core mechanism, load-bearing refinements (mechanism corrections, acute/chronic distinctions, tissue-specific qualifiers), and its architectural connection. The essence exists to give agents and humans a low-cost path to framework-level orientation without reading the whole body. Reading just the essence callouts across the vault (~3,500 tokens total) gives the full framework skeleton.

**Subordination clause.** The essence is derived from the canonical doc body. If the essence and body conflict, **the body is authoritative**. Re-verify the essence when the body changes substantively.

**Shared `last-verified`.** The essence does not carry its own verification date — it shares the doc's `last-verified` frontmatter field. If the doc is re-verified, the essence is re-verified with it. A separate date would double the maintenance burden without reducing drift risk.

**Writing rules.** Prose form, not bullets — bullets fragment interconnection back into a list and destroy the integration the essence is meant to preserve. 5-sentence hard cap, because any longer drifts back into exposition. Write the essence last, after the body is stable; writing it first produces aspirational summaries that the body fails to deliver.

**Relationship to `Essence.md`.** The per-doc essences do not duplicate the framework-level [[Essence]] document. `Essence.md` distills the vault's 13 first principles across six layers (what life is, what health and disease ARE, how the system behaves architecturally, temporal dynamics, scope, interpretive discipline). Per-doc essences distill one component's mechanism. They answer different questions and should complement, not mirror.

**Audit.** Periodically (quarterly, or before major releases), an agent should read each essence, then read its doc body, and flag any mismatch. The audit cost is small (~3,500 tokens per pass) and prevents the drift problem that asymmetric maintenance would otherwise produce.

**Why this exists.** The vault's primary cost for agents and humans seeking framework-level understanding is reading time. The CLAUDE.md navigation guide does most of the orientation work, but opener quality across the docs was historically inconsistent — some crystallized the essence immediately, most delayed it behind exposition. The `[!abstract] Essence` callout enforces consistency: same location, same length, same content requirements, across every canonical doc. Framework-level orientation costs ~2% of the vault's token weight instead of 100%.
