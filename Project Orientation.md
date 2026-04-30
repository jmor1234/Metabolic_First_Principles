# Project Orientation

> What this project actually is, how it got here, and the discipline for reading what it produced. Written for a fresh agent so the conceptual + historical + methodological picture comes from one file rather than nine.

This file does not replace `CLAUDE.md` (navigation), `essence/Essence.md` (the 13 first principles), `metabolic_framework/Foundation.md` (the thesis), or `metabolic_framework/The System.md` (the architecture). It situates them — so when you read them you know what you are reading, why it exists, and what discipline it must be read with.

---

## 1. The Question

Not "how do I treat condition X." Not "what supplement should I take." The question that started this work was more fundamental:

**What IS health, at the deepest resolution biology currently allows? And what IS disease — not which diseases exist, but disease itself, as a biological phenomenon?**

Every other artifact in this workspace exists because that question was taken seriously and pursued for as far as the evidence reached.

---

## 2. The Answer That Survived

**Health IS efficient oxidative metabolism of Krebs-cycle substrates — primarily glucose, with ketone bodies as a biochemically equivalent alternative — to CO₂ and abundant ATP. Disease IS its progressive failure.**

This is not "metabolism is one factor among many in health." Metabolism **IS** health at the cellular level. The reasoning:

- Every cellular function requires ATP. A human produces and consumes ~40 kg of ATP daily — approaching their own body weight. ATP production is not a side process. It IS the central activity of being alive.
- Every disease, at some level, involves the failure of a cellular function. Therefore every disease involves, at some level, a failure of energy production.
- What we call "disease" is what cellular energy failure looks like from different angles, in different tissues, at different stages of progression.

This is identification of the common denominator, not reductionism. Genetics, immunity, hormones, and psychological stress are real — but they operate **through** metabolic capacity. The metabolic level is where they converge.

The framework applies in two modes — primary driver (metabolic syndrome, T2D, NASH, CVD, most cancers, increasingly functional psychiatric illness) and central pathway (autoimmune, Huntington's, hemoglobinopathies, channelopathies, where non-metabolic initiating lesions still route their pathogenic cascade through metabolism). Only a narrow third category is genuinely peripheral (cystic fibrosis, Marfan, clearly syndromic genetic neurodevelopmental conditions). **Non-metabolic initiating lesion does not mean non-metabolic disease.**

---

## 3. How We Got Here — Three Epistemic Stances

The project moved through three vaults, each holding a different stance toward the same underlying biology. Understanding the trajectory matters because it explains why the current vault is what it is.

### Stance 1 — Verification (`project_history/peat_claims_verified/`)

The investigation needed a starting point. Ray Peat's body of work was chosen not because he was right but because his was the most coherent first-principles integration of metabolic biochemistry available — broad enough to test against, freely available in primary form, and operating at the deepest mechanistic level (mitochondrial respiration, not symptoms).

A three-phase methodology was applied to 16 topics, 118+ specific claims:

1. **Extract Peat's actual position** from raypeat.com — reasoning chains, not summaries.
2. **Map the research landscape** — funding, comparison choices, timescales, endpoints, disciplinary fragmentation — from real-time research, not training data.
3. **Verify against peer-reviewed evidence** with full context, using a calibrated scale (confirmed / confirmed with nuance / partially supported / overstated / speculative / not supported).

**Outcome:** ~79% of specific claims survived directionally, ~4% contradicted outright, the rest refined. The biggest discovery was not about any single mechanism — it was that **the evidence for an integrated metabolic picture already existed in the peer-reviewed literature**, scattered across endocrinology, hepatology, oncology, neurology, immunology, and cell biology. No discipline had assembled it. The integration itself was the contribution that no specialist had made.

### Stance 2 — Extraction (the original `metabolic_foundations/`, now subsumed)

A problem became visible: the verified knowledge was trapped inside the verification scaffold. To know what was true about estrogen, a reader had to read "Peat said X → research says Y → assessment Z." The intent was never a monument to one person's framework. It was to find what is most fundamentally true.

So the verified findings were extracted as standalone biology — organized around the system itself, not around any person's claims. 14 documents in four tiers (Structural / Mechanisms / Application / Meta). Zero references to Peat. The scaffold removed; the knowledge preserved.

### Stance 3 — Stress Test (`project_history/metabolic_refinements/`)

The extracted vault was then probed adversarially. Layer by layer, the load-bearing claims were challenged with the goal of finding where they were wrong. This produced six refinement documents and one deep structural insight (state-dependent damping — see §5).

**The verification methodology had codified an asymmetry**: the cost of wrongly changing an integration that took rigorous work to build is higher than the cost of wrongly leaving it unchanged. So refinements did not silently overwrite the original — they sat beside it as a separate epistemic layer.

### The Current State — One Unified Vault (`metabolic_framework/`)

All stress test refinements are now incorporated into a single live vault. The three precursor vaults remain in `project_history/` as the audit trail. The current best understanding of the biology is in `metabolic_framework/`. The first-principles distillation is `essence/Essence.md`. The honest accounting of Peat is `Ray Peat — Historical Assessment.md`.

---

## 4. The Structural Dependency That Holds Everything

This is the layer below the architecture — the reason every feature of the framework follows *necessarily* rather than as an independent design choice.

**Principle 1.** Life is continuous energy throughput maintaining order against entropy. A living organism is an ordered system; order requires continuous energy input.

**Principle 2.** ATP is the universal currency. The metabolic fork at pyruvate (oxidation → CO₂ + ~36 ATP **vs.** reduction → lactate + 2 ATP) defines health vs. disease at the cellular level. An 18-fold asymmetry between a cell that runs its full machinery and a cell that must triage.

**The circular dependency that follows:** the machinery that produces energy is itself maintained by energy. Energy production creates the conditions for its own continuation or degradation.

**This circularity is why self-reinforcement is structural to life rather than coincidental.** Every architectural feature below — active outputs, conditional bistability, state-dependent damping, multi-loop recovery, dual lock-in, daily oscillation — is a consequence of this single fact, not an independent assumption.

---

## 5. The Architecture That Follows

### Active outputs, not passive byproducts

The two endpoints of the metabolic fork actively shape their own continuation:
- **CO₂ + co-produced ATP** sustain more oxidation (Bohr effect delivers O₂ to active tissues; ATP powers V-ATPase to keep inflammatory mediators sequestered; carbamino bonds protect proteins).
- **Lactate** deepens metabolic failure (histone lactylation reprograms gene expression toward glycolysis; HIF-1α stabilization shifts immunity toward tolerogenic M2; lactylation drives fibrosis).

Output shapes continuation. Health maintains health. Disease produces more disease.

### Conditional bistability

When parameter conditions (PUFA burden, iron load, chronic stress, endotoxin exposure) place the organism in the bistable region, both attractors exist and each is self-reinforcing. An organism with low damage burden and robust damping may be **monostable** — the healthy state is the only attractor. This conditionality is the stress-test refinement of Peat's unconditional bistability claim. Confirmed at four independent levels: structural (10+ positive circuits in 3 canonical motifs), mathematical (Topp 2000 saddle-node bifurcation), cellular (Mulukutla 2014 hysteresis at the glycolysis/OXPHOS switch), whole-organism (bariatric remission hysteresis + Tabak 2009 critical slowing down).

### State-dependent damping — the deepest insight

This is the structural mechanism the stress test surfaced and Peat never articulated. Every negative feedback mechanism in the body — HPT, HPA, antioxidant defenses (GSH, SOD, GPx), mitochondrial biogenesis (PGC-1α), autophagy (PINK1/Parkin), immune resolution (resolvins), hepatic regeneration, lactate clearance — depends on **mitochondrial respiratory capacity** for the machinery that performs it (enzyme synthesis, folding, trafficking, cofactor regeneration).

Not ATP alone. The coupled currencies vary across systems — ATP, NADPH (PPP-produced, ATP-independent), Δψ_m, NAD+ (tissue-specific, not reliably human-translatable per Chubanava 2025). All share the OXPHOS origin. When mitochondrial function falls, they fall together, and the damping machinery degrades across systems that are otherwise independent.

**The consequence:** positive feedback loops do not defeat negative feedback through brute force. They operate **by weakening it**. The nonlinear gain that produces bistable transitions comes from the opposition collapsing, not the drive strengthening. This is multiplicative, not additive — and it unifies feedback failure across systems that look unrelated at the surface.

### Multi-loop recovery

The interlocking loops compensate for single interventions. Crossing the threshold back requires breaking enough loops simultaneously that the remaining loops cannot compensate. Single-intervention plateau-then-regression is the predictable signature of partial loop interruption in a multi-loop system.

### Dual lock-in

Two layers operate:
- **Dynamical** — state maintained by feedback self-reinforcement; reversible when upstream metabolic capacity is restored.
- **Structural** — physically irreversible (post-infarction cardiomyocyte loss, adult nephron loss, crosslinked fibrotic ECM, thermodynamically stable amyloid/tau/α-synuclein aggregates). Produced by prolonged metabolic failure but persisting independent of current metabolic state once formed.

Metabolic restoration slows further damage; it does not reverse damage already done. **This is why early intervention has disproportionate leverage** — not just because fewer feedback loops have engaged, but because structural ceilings on reversibility have not yet been crossed.

### Daily oscillation as temporal expression

Every 24 hours the organism enters a partial conservation program (melatonin → cortisol rise → FFA mobilization → T3 suppression) and must reverse it each morning through two independent pathways: blue light → SCN → melatonin suppression, and red/NIR light → cytochrome c oxidase → ATP. Health is the capacity to enter the dip shallowly and exit it completely each morning. Long-term trajectory is determined by the daily balance of time spent in each attractor — not by which state the organism is "in."

---

## 6. The Peat Pattern, Honestly Named

The verification produced one consistent finding across nearly every topic: **right destination, wrong route.**

| Level | Accuracy |
|---|---|
| Thesis (what health and disease ARE) | ~95% |
| Architecture (how the system works) | ~85% |
| Mechanisms (~80% direction, ~50–60% specific pathway) | The gap IS the pattern |
| Practical recommendations | ~80–85% |

Peat saw the system correctly at the level he could see it. The molecular tools that would have refined his mechanism attributions — Seahorse, cryo-EM, iPSC-derived models, mass spec proteomics, the ferroptosis field, the lactylation discovery — largely arrived after his framework was established. He was reasoning backward from correct system-level observations to mechanisms, and naturally picking the most parsimonious explanation available. The more direct explanation was consistently wrong, but the strategy that produced the pattern (working backward from correct observations) is what *validated itself*: if the destinations are reliably right, the observer is seeing something real.

### The single biggest error: CO₂ as a causal driver

Peat treated CO₂ as the active agent in feedback loops (sustaining oxidation, sequestering mediators, supporting thyroid). The stress test's causal-independence audit (Pearl screening-off + MCA conservation relations) found that **ATP, not CO₂, is the causal agent at every loop target**. CO₂ is stoichiometrically co-produced with ATP at OXPHOS but has no specific molecular mechanism at any loop target — only non-specific bulk pH effects. ATP has specific mechanisms everywhere (V-ATPase catalytic site, tight junction maintenance, smooth muscle contraction). CO₂'s non-loop roles (Bohr effect, carbamino bonds, calcium/pH buffering) are real and preserved.

**This error is not independent.** It inherits directly from Peat's coacervate ontology of mitochondria. In a coacervate framework, mitochondria are phase-separated structures whose stability depends on interfacial chemistry — the natural regulatory agent is a small, diffusible molecule that alters interfacial forces, exactly what CO₂ is. Replace the coacervate ontology with the endosymbiont/membrane-bound-organelle picture (which requires ATP-dependent transport for organelle maintenance), and ATP becomes the natural regulatory agent. **The CO₂→ATP correction is a consequence of correcting his ontology, not an independent molecular error.**

### The physical-chemistry preference pattern

Beneath the individual errors is a single methodological preference. When biology offered two candidate explanations — one grounded in general physical principles (phase dynamics, interfacial forces, bulk water structure) and one grounded in specific molecular machinery (specific pumps, specific organelles with specific genomes) — Peat consistently chose the physical-chemistry version. The fingerprint of his error pattern: when his specified mechanism conflicts with well-established molecular biology, the conflict is almost always diagnostic of this preference overriding the evidence. The system-level observation is usually still correct; the mechanism he cites is usually wrong.

### How to read Peat now

- **System-level observations** — usually right. Trust as a first pass.
- **Mechanism attributions where molecular biology wasn't yet characterized** — right direction, wrong route. Hold cautiously.
- **Mechanism attributions where molecular biology was well-established but conflicted with his framework** — systematically wrong. Be actively skeptical.
- **When he says "CO₂ does X"** — read it as "ATP does X, and CO₂ is the parallel marker you can monitor."
- **When he dismisses something categorically** — add conditionality (acute vs. chronic, regime-dependent).

---

## 7. The Reading Discipline

This is non-negotiable for any agent doing work that touches the framework.

### Read it as an integration, not a database

The vault is a connected system. The meaning of any single statement depends on its connections to other documents through the wikilink network. Surface terms have deep implications: "metabolic rate" is not raw throughput but the rate that emerges from intact hardware; "estrogen amplifies disease" means it amplifies whatever trajectory is in motion, not that it is categorically harmful; "the disease attractor is self-reinforcing" requires specific parameter conditions to engage.

**Reading individual statements at face value, without tracing the connections, produces shallow conclusions and false contradictions the vault does not actually contain.** Before evaluating evidence, proposing changes, or answering complex questions: trace the reasoning chain. If you cannot trace it, you do not yet understand the vault well enough to draw conclusions.

### The asymmetry principle

The cost of wrongly changing an integration that took rigorous work to build is higher than the cost of wrongly leaving it unchanged. The framework is designed to be corrected, but **the bar for correction is high**. Default position: the vault is correct until proven otherwise with verified evidence that survives a deep reading of its logic. The discipline for doing this rigorously is `metabolic_framework/Verification Methodology.md`.

### Three interpretive disciplines that prevent false contradictions

1. **Mechanistic specificity is required** — every claim of "operating through metabolic capacity" must be traceable as a specific pathway at each step. Where no trace exists, the framework does not claim convergence through metabolism.
2. **Acute and chronic states can have opposite effects at the same mechanism** — acute lactate is neuroprotective fuel; chronic lactate is an epigenetic disease driver. Intermittent PTH builds bone; chronic PTH destroys it. Confusing the two manufactures contradictions.
3. **Context-dependence is a property of a bistable system** — the same intervention interacts with whichever attractor the organism currently occupies. Aspirin protects younger populations and increases cancer mortality in healthy elderly (ASPREE). This is not noise — it is a predictable consequence of attractor dynamics.

---

## 8. Where Things Live Now

### The live knowledge

- **`metabolic_framework/`** — the unified vault. 14 documents, four tiers (Structural / Mechanisms / Application / Meta). All stress test refinements incorporated. Start with `metabolic_framework/CLAUDE.md` for navigation.
- **`essence/Essence.md`** — the 13 first principles distilled across 6 layers (what life is → what health and disease ARE → architecture → temporal dynamics → scope → interpretive discipline). Read in ~10 minutes; gives the principles skeleton.

### The audit trail (archived, not modified)

- **`project_history/peat_claims_verified/`** — the original verification (16 topics, 118+ claims, calibrated assessment scale).
- **`project_history/metabolic_refinements/`** — the stress test layer (six refinement documents, audit trail, methodology).
- **`project_history/metabolic_foundations_snapshot/`** — the pre-stress-test snapshot.
- **`project_history/Overview.md`** + **`project_history/The Integrated Framework.md`** — the journey synthesis as it stood mid-project.

### The honest accounting

- **`Ray Peat — Historical Assessment.md`** — first-principles assessment of Peat's accuracy, error patterns (physical-chemistry preference), and the three-tier reading rule.

---

## 9. How to Continue

A reader with the time for full depth reads, in order:

1. This file.
2. `essence/Essence.md` — the 13 principles. ~2,500 tokens.
3. `metabolic_framework/Foundation.md` — the thesis with evidence. The bulk of conceptual understanding.
4. `metabolic_framework/The System.md` — the architecture (attractors, loops, state-dependent damping, predictions, temporal oscillation).
5. `Ray Peat — Historical Assessment.md` — the honest accounting of where the starting point holds and where it doesn't.

A reader doing work that touches the vault adds:

6. `metabolic_framework/Verification Methodology.md` — default position, three hypotheses, bar for change, six-step verification sequence.
7. `metabolic_framework/Methodology.md` — evidence standards, confidence calibration, document template, expansion process.

A reader looking up a specific mechanism uses the canonical-location table in `metabolic_framework/CLAUDE.md` instead of reading mechanism documents end-to-end.

---

## 10. What This Project Is, in One Sentence

**An attempt to answer "what IS health" at the deepest resolution biology currently allows, built by taking the most coherent first-principles starting point available, verifying it claim-by-claim against peer-reviewed evidence, extracting what survived as standalone biology organized around the system itself, then adversarially probing the result — and producing, in the process, an integrated map (one circular dependency at the foundation, one attractor architecture, one deepest mechanism — state-dependent damping — that no single discipline had named) that exists nowhere else because no specialty assembled the evidence that was already there.**

The integration is the contribution. The evidence belongs to the researchers who produced it. Every correction made the framework stronger. The bar for further correction is high — but the framework is designed to be corrected, not defended.
