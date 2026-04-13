---
title: "Verification Methodology"
aliases:
  - How to Verify
  - Resolution Process
  - Evidence Verification
  - Rules of Engagement
  - Testing Protocol
  - Stress Test Methodology
tags:
  - structural/meta
  - framework/metabolic
role: methodology
confidence: high
last-verified: 2026-04-11
scope: meta
connections:
  - "[[Methodology]]"
  - "[[Foundation]]"
  - "[[The System]]"
---

This document governs how the Metabolic Foundations vault is tested, verified, and changed. It applies to stress testing, evaluating new evidence, adding topics, and any situation where the vault might need modification. It was distilled from the process of stress-testing five cases against the vault's architecture, where the most important finding was not about any specific case — it was about how to evaluate evidence against an integrated framework without degrading the integration.

---

## The Two Failure Modes

Every interaction with the vault's evidence base risks one of two opposite failures:

**Failure mode 1: Defending the framework unfairly.** The framework's built-in explanatory resources — the acute/chronic distinction and context-dependence — can absorb any counterexample if allowed to flex after the fact. This makes the framework unfalsifiable. The Three Rules below constrain when and how those resources can be invoked.

**Failure mode 2: Changing the framework based on shallow understanding.** The vault is an integration where mechanisms interlock and surface-level terms have deep implications. Apparent contradictions frequently dissolve when the vault is deeply understood rather than read at face value. The stress test revealed that this risk was more serious in practice — multiple proposed changes would have made the vault less accurate, not more, because they were based on misunderstanding what the vault was actually saying. The Default Position and Three Hypotheses below guard against this.

Both failures degrade the vault. The first makes it unfalsifiable. The second makes it less precise. This document guards against both.

---

## The Default Position: The Vault Is Correct Until Proven Otherwise

The vault was built through a rigorous three-phase verification process. It represents an integration — a connected system where mechanisms interlock and implications compound. Individual research papers do not have this integration. A paper measuring one variable in one context can appear to contradict the vault if you do not understand the vault's full picture.

The consistent finding during stress testing was: read the vault at surface level, find an apparent contradiction with external evidence, propose a change — and then discover on deeper investigation that the vault already handled the case through its existing logic, or that the apparent contradiction was a misunderstanding of what the vault was actually saying.

The cost of wrongly changing the vault is higher than the cost of wrongly leaving it unchanged. A wrong change degrades an integration that took rigorous work to build. A wrong non-change leaves a possible improvement unmade — but the vault can always be updated later when the evidence is clear. The asymmetry favors caution.

---

## The Three Hypotheses, In Order

When research appears to contradict the vault, check these three hypotheses in this sequence. Do not skip to hypothesis 3.

**Hypothesis 1: You are misunderstanding the vault.**

This is the most common case, and the most dangerous, because it feels like understanding. The vault is not a collection of independent claims. It is an integrated system where each claim exists within a web of connections, and the meaning of any single statement depends on the logic of the whole. Reading individual statements at face value — without tracing the reasoning chain that produced them and the implications that follow from them — produces a shallow reading that finds contradictions the vault does not actually contain.

The specific failure: reading words rather than understanding the system. Every term in the vault carries implications from its connections to every other term. When the vault says "metabolic rate," it does not mean raw energy throughput as an isolated variable. It means the rate that emerges from intact, efficient mitochondrial hardware — because T3 builds respiratory complexes, respiratory complexes determine oxidative capacity, and oxidative capacity manifests as metabolic rate. Rate and efficiency converge over time through structural integrity: poor efficiency degrades hardware, which reduces the rate the hardware can sustain; clean efficiency preserves hardware, which sustains rate. At long-term equilibrium in a freely-functioning organism, metabolic rate IS a readout of metabolic efficiency. A surface reading sees "higher rate = healthier" and finds a contradiction with caloric restriction. The deep reading sees that rate reflects hardware quality at equilibrium, and CR artificially separates them by externally constraining throughput — which is not a contradiction but a special case the architecture already accommodates.

This pattern recurs across every term in the vault:
- "Estrogen is a metabolic amplifier" means it amplifies whatever trajectory is in motion, not that it is categorically harmful
- "The disease attractor is self-reinforcing" means the feedback loops deepen the state when engaged — but the loops require specific conditions (adequate temperature, metabolic flux, damage exceeding repair) to engage
- "Glucose is the preferred substrate" means glucose oxidation produces maximum CO2 in the context of the vault's metabolic fork — not that every non-glucose metabolic state is pathological

Before concluding the vault is wrong, trace the vault's full reasoning chain for the case in question. Follow the wikilinks. Read the System Connections tables. Ask: what does the vault's own logic PREDICT for this case, when I follow the chain all the way through? The answer often resolves the apparent contradiction without changing anything. If you cannot trace the chain, you do not understand the vault well enough to assess contradictions — and the responsible conclusion is to study the vault more deeply before proposing changes.

**Hypothesis 2: The research measures something different from what the vault is talking about.**

The vault's claims operate at the level of mitochondrial oxidative metabolism — CO2 production, lactate, mitochondrial membrane integrity, coupling efficiency, ATP-to-damage ratio. Much research measures proxy endpoints: blood lipids, HbA1c, body weight, serum hormone levels, inflammatory markers. A study showing improved blood markers does not confirm or deny a claim about mitochondrial function. A study measuring seizure frequency does not address CO2 production. The endpoint divergence documented throughout the vault (fish oil improving lipids while producing maximal mitochondrial oxidative stress) applies to new evidence exactly as it applies to the research the vault already evaluates.

Before concluding the vault is wrong, check whether the contradicting research actually measures the variables the vault's claims operate on. If it measures proxies, it cannot confirm or deny the vault's specific mechanisms — regardless of its outcome.

**Hypothesis 3: The vault is wrong.**

This is the least common case. It does occur — the M1/M2 macrophage metabolic labeling was a genuine factual error. But it is rare, and the bar for concluding it should be high:

- The evidence must be specific, replicated, and confirmed in humans (or the relevant organism)
- The evidence must directly measure the variables the vault's claims operate on, not proxies
- The contradiction must survive a deep reading of the vault's logic, not just a surface reading
- You must be able to state precisely what the vault says, precisely what the evidence shows, and precisely why the two cannot be reconciled

If all four conditions are met, the vault should be changed. If any one is not met, the evidence should be noted but the vault should not be changed until the remaining conditions are satisfied.

---

## The Bar for Changing the Vault

A vault change is warranted when:
- There is a **demonstrable factual error** (M1/M2 labeling) with clear, unambiguous evidence
- There is a **genuinely new finding** that connects existing vault topics in a way the vault doesn't currently model (iron→ERα degradation connecting the iron thesis to estrogen receptor biology) — this is ADDITIVE, not corrective
- There is a **specific, verified, replicated finding** that directly contradicts a vault claim at the mechanistic level the vault operates on, surviving deep reading of the vault's logic

A vault change is NOT warranted when:
- A surface-level reading suggests a contradiction that dissolves when the vault is deeply understood
- Research measures proxy endpoints that don't address the vault's specific mechanistic claims
- A proposed "refinement" would make the vault more complex without making it more precise
- The change would address a case the vault's existing architecture already handles through its stated principles

### What This Means in Practice

1. **Understand the vault deeply before evaluating challenges to it.** Not the words — the deep logic, the implications, the way mechanisms interlock across documents.
2. **Assume the vault is correct and look for why, before assuming it's wrong and looking for what to change.** Most apparent contradictions dissolve on deeper examination.
3. **When proposing a change, the burden of proof is on the change, not on the vault.** The change must be clearly, specifically, demonstrably better — verified through multiple angles, surviving deep analysis.
4. **A change that makes the vault more complex without making it more precise is not an improvement.** The vault's value is in its integration. Adding caveats, exceptions, and qualifications without increasing predictive power degrades that integration.
5. **"I don't understand this well enough to assess whether the vault needs to change" is a valid and responsible conclusion.** It is better than a confident-sounding proposal that makes the vault worse.

---

## The Core Claims

These are the framework's core structural claims. They are pre-specified so that any testing has a clear definition of what constitutes a core change versus a peripheral modification.

1. **Health is efficient oxidative metabolism of Krebs-cycle substrates to CO2 — glucose preferred, ketone bodies biochemically equivalent at the Krebs cycle, raw fatty acid β-oxidation inferior; disease is its progressive failure.** The metabolic fork is the foundational definition.
2. **The system can exhibit two self-reinforcing stable states when parameter conditions create a disease basin.** The attractor structure — not a spectrum but two basins maintained by their own outputs, conditional on PUFA burden, iron load, chronic stress, and endotoxin exposure.
3. **Positive feedback loops make each state self-maintaining.** Bistability arises from interlocking reinforcement, not from a single cause.
4. **Recovery requires addressing multiple loops simultaneously.** Threshold dynamics — single interventions are insufficient because remaining loops compensate.
5. **The system oscillates between attractors daily.** The temporal architecture — the organism enters a partial conservation state nightly and must reverse it each morning.

A modification to any of these five constitutes a **core** change. Everything else — specific feedback loops, specific component roles, specific mechanism pathways, specific groupings — is **peripheral** and can be modified, added, or removed without the core falling.

---

## The Three Rules

These rules constrain when and how the framework's built-in explanatory resources can be invoked. They prevent Failure Mode 1 (defending the framework unfairly / unfalsifiability).

### Rule 1: The Acute/Chronic Distinction (Control Architecture)

The framework uses the acute/chronic distinction to resolve cases where the same metabolic signature (lactate elevation, glycolytic shift, conservation signaling) appears in both healthy and pathological contexts. This distinction is valid only under the following constraints.

The actual variable is not time. It is **control architecture** — whether the metabolic state is a controlled biological deployment or an uncontrolled drift into damage.

**Controlled Deployment** — ALL FOUR criteria must be met:

1. **Entered under programmatic biological control.** A defined trigger initiates the state through hormonal signaling, neural circuits, or gene expression programs.
2. **Has a built-in termination mechanism that is intact and will fire.** The biological program that enters the state includes the program that exits it, and that exit program is functional.
3. **Does not damage reversal systems beyond their repair/replacement capacity within the recovery window.** Transient damage is permitted if the system has intact capacity to repair or replace the damaged components within the recovery period, and the replacements are equal or better quality than what was damaged. (This accommodates hormesis — where controlled damage is the adaptation signal — while excluding chronic damage that degrades faster than repair.)
4. **The system returns to baseline or better** after the state resolves. Measurable: metabolic markers return to or exceed prior values.

**Uncontrolled Drift** — ANY of the following:

1. **Entered through accumulated damage or dysfunction** rather than programmatic biological control.
2. **No termination mechanism exists**, or the termination mechanism is itself impaired by the state.
3. **Damages reversal systems beyond their repair/replacement capacity.** The damage rate exceeds the repair rate, or replacements are equally or more vulnerable than what was lost.
4. **The system does not return to baseline.** Each cycle leaves a residual deficit that accumulates.

**Invocation Constraint:** This distinction can be invoked ONLY when the classification is based on the **entry mechanism and termination architecture** — observable biological features — NOT on whether the outcome was healthy or pathological. Classifying by outcome is circular and invalidates the resolution.

### Rule 2: Context-Dependence

The framework claims the same intervention can produce opposite effects depending on metabolic context. This is a legitimate property of bistable systems. It is also the most direct route to unfalsifiability. Context-dependence is a valid resolution ONLY when all three conditions are met simultaneously.

**The Three Required Conditions:**

1. **The context variable is specified in advance.** Before examining outcome data for the case, the framework states which measurable variable determines the effect direction.
2. **The context variable is independently measurable.** It can be assessed by a measurement that does not depend on the outcome being explained. Examples: ETCO2, RQ, blood lactate, mitochondrial membrane potential — measured before the intervention, not inferred from its results.
3. **The prediction is directional and falsifiable.** Given context measurement X above/below threshold Y, the framework predicts outcome Z. Outcome not-Z at that context value would constitute disconfirmation.

**Invalidation Criteria** — Context-dependence is NOT a valid resolution when:

- The context is identified only after seeing the result
- The context variable is defined by the outcome it is supposed to explain (circularity)
- No measurable threshold separates the contexts
- The "context" is a restatement of the outcome in mechanistic language ("estrogen is protective when cells are healthy" where "healthy" is not independently defined)

If the three conditions cannot be met, the resolution is invalid and the case stands as an unresolved challenge.

### Rule 3: Outcome Classification (Pass / Refinement / Fail)

Every evaluated case receives one of three verdicts. The decisive criterion: **does the resolution make the framework more or less falsifiable?**

**Pass** — The existing architecture handles the case with **no modifications**. The framework already contains the stated principles needed — it has simply not been explicitly applied to this domain.

**Refinement** — The architecture needs a modification that makes it **more precise and more predictive**. All of the following must be true:

- The modification **constrains** the framework's claims — narrows what it predicts, making it easier to falsify
- The modification **generates new testable predictions** that did not exist before
- The **core claims** survive intact
- Practical recommendations may be updated or made more specific, but not reversed

**Fail** — The architecture needs a modification that makes it **more vague or less predictive**. Any of the following indicate failure:

- The modification **widens** what the framework can explain — increases flexibility, makes it harder to falsify
- The modification does **not generate new testable predictions**
- A **core claim** must be abandoned or fundamentally weakened
- Practical recommendations must be **reversed**

**The Decisive Test:** After resolution, can the framework predict more specific things than before, or fewer? Refinements increase specificity. Failures decrease it.

---

## The Verification Sequence

For any case where the framework faces an apparent contradiction, a new claim to evaluate, or a mechanism to verify — follow these steps in this order. The order matters. Each step produces information that constrains the next.

### Step 1: Deeply Understand What the Vault Predicts

Before identifying a contradiction, trace the vault's full reasoning chain. Follow wikilinks. Read System Connections tables. Ask: what does the vault's own logic predict when I follow it all the way through? If you cannot trace it, you do not understand the vault well enough to assess whether a contradiction exists.

**Unpack the prediction chain link by link.** The vault's prediction is rarely a single claim — it is usually a chain of premises leading to a conclusion. For example, "ETCO2 reflects oxidative metabolism" decomposes into: T3 → mitochondrial activity → CO2 production → ETCO2 (in exhaled breath). Each link is a separate testable claim with its own evidentiary status. Write out the full chain. For each link, mark whether it is textbook, well-supported, contested, or inferred. Concentrate verification effort on contested and inferred links. Searching for evidence on textbook links wastes effort and misses the actual question.

**List adjacent measurements before searching.** The vault uses specific terms for measurements. The broader scientific literature may use related terms whose evidence is more direct or more abundant. Before searching, list ALL measurements that could test the vault's claim — not just the term the vault uses. For "CO2 production," that means listing V'CO2, indirect calorimetry, basal metabolic rate, RQ, resting energy expenditure — not just ETCO2. Each adjacent measurement is a search target. Anchoring on the vault's vocabulary instead of the underlying physiology produces searches that miss the strongest available evidence and surface only what the vault already cites.

### Step 2: Check the Framework's Own Metrics

What do the vault's diagnostic variables predict should happen in this case, and what do actual measurements show?

The vault's core measurement framework is:
- CO2 production: V'CO2 by indirect calorimetry (gold standard) or ETCO2 by capnography (accessible proxy that reflects production-ventilation balance, distinct from V'CO2)
- Blood lactate
- Respiratory quotient (RQ)
- Body temperature
- Resting pulse
- Mitochondrial function markers (Complex IV activity, cardiolipin composition, coupling efficiency)

For the case in question, determine: What does each metric predict? What do actual studies measure? Which metrics have NOT been measured? This step often reveals that the vault's own metrics support the vault's claims — or that the relevant metrics have never been measured, meaning the apparent contradiction cannot be confirmed.

### Step 3: State the Contradiction — If One Still Exists

Many apparent contradictions dissolve after Steps 1-2. If the contradiction survives deep understanding and metric checking, state it precisely: the exact vault claim, the exact evidence, and why they cannot be reconciled.

### Step 4: Identify What a Resolution Would Depend On

Before committing to any resolution, explicitly list: what specific evidence claims would need to be true for this resolution to hold? Write them down. Each is a load-bearing claim. If any one collapses, the resolution collapses.

**Causal independence audit — check whether the named causal variable can be an independent causal participant at all.** A second sub-practice learned from Sub-test 2.A, applied at Step 4 before Step 5 verifies specific evidence. When a feedback-loop resolution names a metabolite as a causal driver, check whether the metabolite could *in principle* be an independent causal participant — whether its causal role is not reducible to the role of a stoichiometrically co-produced partner acting through a different mechanism on the same target. This is the Pearl screening-off question (Pearl 2009 *Causality*) applied to biochemical networks, with the conservation-relations framework from Metabolic Control Analysis (Reder 1988; Heinrich & Schuster 1996; Palsson 2003 on the left null space of the stoichiometric matrix) as the formal machinery for identifying when two metabolites are stoichiometrically locked. The audit asks four sub-checks:

1. **Conservation check.** Is the metabolite in a conserved moiety pool or otherwise stoichiometrically locked to another variable under the physiological regime the loop is claimed to operate in? This is a diagnostic flag, not a verdict — proceed to the other checks.

2. **Mechanism specificity check.** Does the metabolite act on the loop's downstream target through a named molecular mechanism — a specific binding site, substrate role, or covalent modification — that its stoichiometric partner does not share? Or does the mechanism rely on a *non-specific* bulk effect (bulk pH, bulk osmolality, bulk thermal) the partner would also produce? Non-specific mechanism + partner with a specific mechanism = parallel marker.

3. **Realizable intervention check.** Is there a physiologically realizable intervention that dissociates the metabolite from its partner with differential downstream effects? Examples: carbonic anhydrase inhibition dissociates bicarbonate from ATP at soluble adenylyl cyclase; UCP activation dissociates CO₂ from ATP at the cellular level; non-linear amplification via the adenylate kinase equilibrium makes AMP quantitatively dissociable from ATP across physiological ranges.

4. **Quantitative dominance check.** At the concentrations, timescales, and tissue locations where the loop is claimed to operate, does the metabolite's effect magnitude exceed its stoichiometric partner's?

Classification: **independent driver** (specific mechanism or quantitative dominance), **parallel marker** (fails mechanism specificity when a partner has a specific mechanism), **gated driver** (parallel marker at baseline, independent driver when coupling breaks — e.g., proton gradient under UCP uncoupling), **co-driver** (mutually independent participants via distinct mechanisms — e.g., Ca²⁺ and IP3 in PLC oscillations), or **indeterminate**.

**Worked example — the original Loop 7 error.** The framework's original Loop 7 mechanism (extracellular CO₂ → carbonic acid → granule pH → mediator release) fails the mechanism specificity check: the claimed mechanism is bulk pH, and ATP has a specific mechanism at the same target (V-ATPase is ATP-specific at its catalytic site, actively maintains a ~1.9-unit pH gradient across the granule membrane, and the V₁-V₀ domain couples granule pH to exocytosis readiness). The audit correctly classifies original CO₂ as a parallel marker and refined ATP as an independent driver. This is the refinement Sub-test 2.A produced.

**Worked counterexample — soluble adenylyl cyclase.** CO₂/bicarbonate is stoichiometrically co-produced with ATP at OXPHOS, but in the soluble adenylyl cyclase (sAC) pathway (Acin-Perez et al. 2009 *Cell Metabolism*; Valsecchi et al. 2014 *BBA* PMC4257896; Kleinboelting et al. 2014 *PNAS* crystal structures) bicarbonate binds sAC directly at a specific allosteric site (Arg176 with salt bridge disruption and active-site closure), and ATP functions as substrate not allosteric activator. Bicarbonate therefore passes the mechanism specificity check and is classified as an independent driver despite stoichiometric coupling to ATP. The case establishes that **stoichiometric coupling alone does not disqualify a metabolite** from independent causal status — the audit must always check mechanism specificity before declaring parallel-marker status. (The sAC pathway is currently framed in the literature as feedforward metabolic matching rather than closed positive feedback, and is not currently a formalized loop in the vault. But it illustrates that "stoichiometrically coupled → parallel marker" is an over-generalization the audit must avoid.)

**Not a novel principle.** This sub-practice is a biochemical application of existing tools (Pearl's do-calculus and screening-off test; MCA conservation relations and flux/concentration control coefficients — Kacser & Burns 1973; Heinrich & Rapoport 1974; Reder 1988; Heinrich & Schuster 1996; Palsson 2003). Where the vault's feedback-loop analysis becomes quantitative (loop gain, formal bistability), MCA's control coefficients are the appropriate formal machinery to reach for. Individual sub-tests citing this audit should cite back to the existing work, not to this document as if it originated the concept.

### Step 5: Verify Each Dependency Against Primary Sources

For every load-bearing claim, search for the actual evidence:

- **Has this finding been replicated?** A single study is a hypothesis. Replication is evidence.
- **Has it been confirmed in humans?** Animal and in vitro findings frequently fail to translate.
- **What are the caveats?** Dose, duration, population, comparison group, endpoint measured.
- **What was NOT measured?** The most important information is often what the study didn't assess.

Apply the same rigor to evidence that SUPPORTS the resolution as to evidence that CHALLENGES it. Evidence that conveniently confirms what you want to conclude is exactly the evidence that needs the hardest pull.

**Distinguish citation accuracy from claim accuracy.** A vault citation can be inaccurate while the underlying claim is supported by other evidence the vault did not cite. These are different problems with different fixes. When you find that the vault's cited paper does not support what the vault says it does, do not immediately collapse this into "the vault is wrong." First check whether OTHER evidence supports the broader claim. The vault may be making a true claim with a weak or misread citation — in which case the fix is to update the citation, not retract the claim. Check citation accuracy and claim accuracy as separate questions, in that order. The citation problem is local. The claim problem, if there is one, is structural.

**Citation deployment audit — go beyond topical relevance.** A stronger sub-practice learned from Sub-test 2.A: check the *deployment context* of each load-bearing citation, not just its topical relevance. A paper can be correctly cited at the title/abstract level but mis-deployed if the vault's specific claim differs from the paper's specific scenario. Ask four questions for every load-bearing citation:

1. **Species match.** Does the paper test the organism the vault's claim operates on? (Canine airway models can look like human respiratory findings at the title level.)
2. **Scenario match.** Does the paper test the physiological scenario the vault is claiming? (An in vitro study of *stimulated* exocytosis with thrombin or ionophore is not a test of *spontaneous release at rest* under physiological pH variation, even if both involve "pH-dependent release.")
3. **Endpoint match.** Does the paper measure what the vault's claim operates on? (Bronchial hyperreactivity to exogenous histamine is not the same as endogenous systemic histamine release. ETCO₂ is not the same as V'CO₂. Serum markers are not the same as tissue-level measurements.)
4. **Proposed-mechanism match.** Does the paper's authors attribute the finding to the same mechanism the vault invokes? (Airway drying / osmolality is not the same as systemic CO₂/pH chemistry, even if both follow hyperventilation.)

If any of these differ, the citation may still be useful but needs explicit recontextualization in the vault — not uncritical reuse as support for a claim the paper doesn't actually test. Sub-test 2.A identified two vault citations (Pollard 1977 and Freed 2001) as topically relevant but deployment-mismatched on scenario, endpoint, species, and proposed mechanism respectively. This pattern is likely not isolated; budget for citation-deployment audits on every load-bearing claim during stress testing, not just the ones that happen to surface contradictions through other routes.

### Step 6: Construct and Stress-Test the Resolution

Only after Steps 1-5 are complete, construct the resolution. Then immediately stress-test it:

- **What is the weakest link?** What would happen if that dependency broke?
- **Am I being more generous to this resolution than I would be to someone else's?**
- **Does it make the framework more precise or more flexible?** Classify per Rule 3.
- **What new predictions does it generate?** If none, it may be accommodation disguised as refinement.

---

## Research Standards

Research papers are written as isolated pieces — single variables, single disciplines, specific timescales, specific endpoints, specific funding. Biology is interconnected. The gap between what a paper measures and what it claims to show can be as important as the finding itself.

### What Must Be Evaluated for Every Study

1. **Who funded it.** Industry-funded studies have structural incentives that shape which questions get asked and which conclusions survive peer review. This does not make them wrong. It determines what they can and cannot see.
2. **What comparison was made.** A study comparing two options within a paradigm the framework's question operates outside of cannot answer the framework's question regardless of quality.
3. **What timescale was covered.** Acute findings can contradict chronic findings for the same molecule.
4. **What endpoint was measured — and what was not.** Does the study measure the mechanistic variable the framework cares about, or a proxy that may diverge from it? This is the most consequential evaluation.
5. **What the study claims versus what it shows.** Report the data and the interpretation separately when they diverge.
6. **Disciplinary fragmentation.** The biology relevant to any case spans multiple specialties that do not cite each other. Research must be gathered across all relevant disciplines.

### The Integration Principle

Individual studies are data points. Evaluation requires integrating findings across disciplines — the same principle that produced the vault. When a study reports an outcome, the relevant questions include: what happened to the mechanistic variables the framework's predictions operate on? If a study does not measure these variables, it cannot confirm or disconfirm the framework's specific predictions, regardless of its outcome.

---

## Who Does the Research

The person holding the full framework context does the research directly, following the verification sequence. This was learned through direct experience: delegating research to agents without framework context required multiple correction passes to reach what one careful context-aware pass would have produced.

### Why Delegation Fails for Evaluation

1. **The agents' synthesis becomes an intermediary you have to un-accept.** A coherent narrative built without context FEELS like verified evidence. It's interpretation without the context needed to interpret correctly.
2. **Without framework context, agents can't evaluate which findings are load-bearing.** An unreplicated finding and a replicated finding look the same in a report. Only someone holding the context can see which one the resolution depends on.
3. **Agents measure what studies measured, not what the framework needs measured.** Only someone who knows the framework's metrics can evaluate whether a study's endpoints are relevant.

### When Delegation Is Still Useful

Sub-agents add value for **narrow, specific searches** where framework context is not needed:
- "Find the most recent meta-analysis on X" — retrieval, not evaluation
- "What is the IC50 of compound Y for target Z?" — factual lookup
- "Has study X been replicated?" — specific verification

The synthesis stays with the person holding the context.

---

## Applying This Beyond Stress Testing

This methodology applies whenever the vault encounters new evidence, a new mechanism, a new claim, or an apparent contradiction:

- **New research contradicts a vault claim:** Start with Hypothesis 1 (am I misunderstanding the vault?), not with proposing a change.
- **A new topic is being added:** Verify the evidence base (Step 5) before constructing the mechanism document. Check what the vault already says about adjacent topics (Step 1). Understand how existing mechanisms interlock before adding new ones.
- **A practical recommendation is questioned:** Check whether the recommendation follows from the architecture (Steps 1-2) and whether the questioning evidence measures the variables the vault's claims operate on.
- **Expanding the framework into new domains:** Identify what a resolution would depend on (Step 4) before committing to a direction. Trace the vault's existing logic into the new domain to see if the architecture already predicts what you're seeing.

The methodology protects against both failures: the framework becoming an ideology that absorbs all evidence without changing (prevented by the verification sequence and honest calibration), and the framework being degraded by well-intentioned changes based on shallow understanding (prevented by the default position and three-hypothesis sequence).
