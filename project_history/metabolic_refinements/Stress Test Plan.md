---
title: "Stress Test Plan"
tags:
  - stress-test
  - protocol
  - working-document
status: active
started: 2026-04-17
scope: methodology
---

# Stress Test Plan

## Purpose

This document defines **how** we stress-test the four priorities in [[Core Stress Test Priorities]]. It contains two parts:

1. **The Protocol** — the method applied to each priority. Reusable.
2. **The Plan** — the specific campaign for the four current priorities. Order, dependencies, stopping rules.

Design goal: honest and first-principles, not ritual. Simple enough to actually follow, rigorous enough to produce real verdicts.

This protocol is **probe-driven** (we proactively attack target claims) but its attack machinery is inherited from the vault's battle-tested [[metabolic_framework/Verification Methodology]], which is **evidence-driven** (responds to incoming evidence that appears to contradict the vault). Same tools, different orchestration. Where the Verification Methodology's tools apply, we use them rather than reinventing — those tools were forged by prior stress testing and have caught real errors (the CO₂ demotion came from the Causal Independence Audit).

---

## First Principles of Stress-Testing

A stress test is an honest attempt to *break* a claim, using evidence that already exists, such that the claim is either strengthened (survived real attack) or a specific weakness is identified.

### Two Failure Modes to Guard Against

Directly from the Verification Methodology's hard-won wisdom — both failures degrade the vault:

- **Failure Mode 1: Defending the framework unfairly.** The framework's built-in explanatory resources (acute/chronic distinction, context-dependence) can absorb any counterexample if allowed to flex post hoc. This makes the framework unfalsifiable. The Three Rules constrain when these can be invoked.
- **Failure Mode 2: Changing the framework based on shallow understanding.** The vault is an integration where surface terms have deep implications. Apparent contradictions frequently dissolve when the vault is deeply understood. Prior stress testing revealed this risk was *more* serious in practice — multiple proposed changes would have made the vault less accurate because they were based on misreading. The H1→H2→H3 sequence guards against this.

### The Three Ways a Stress Test Dies

- **Verification theater** — looking rigorous without actually attacking
- **Moving goalposts** — reframing the claim to protect it from evidence
- **Busy-work** — generating attacks that don't genuinely test

### The Measure of Success

Not "we did a thorough stress test." It is: **we learned something true we didn't know before** — either the claim is more trustworthy than we thought, or it has a specific weakness at a specific point.

---

## The Protocol

Three phases applied to each priority. Each phase has distinct operations. If a clear verdict emerges mid-protocol, document and exit — don't gold-plate.

### Phase 1 — Define the Target

**Purpose:** state precisely what is being tested, where it sits in the framework, and what would refute it.

1. **Restate the claim in its crispest form.** One or two sentences. If this requires hedging, name the hedges explicitly.

2. **Classify the claim's relationship to the Core Claims.** The vault pre-specifies five Core Claims (below). Anything affecting these is a **Core change**; everything else is **Peripheral**. State explicitly: is this claim one of the five, a sub-structure that supports one of them, or a peripheral instantiation?

   **Core Claims** (from [[metabolic_framework/Verification Methodology]]):
   1. Health is efficient oxidative metabolism of Krebs-cycle substrates to CO₂ (glucose preferred, ketones biochemically equivalent, raw fatty acid β-oxidation inferior); disease is its progressive failure
   2. The system can exhibit two self-reinforcing stable states when parameter conditions create a disease basin
   3. Positive feedback loops make each state self-maintaining
   4. Recovery requires addressing multiple loops simultaneously
   5. The system oscillates between attractors daily

   Mapping of current priorities:
   - **P3** (state-dependent damping as cross-system unifier): **not a Core Claim**. The framework itself names state-dependent damping as "one of several mechanisms generating bistability" alongside ultrasensitivity, mutual inhibition, saturation. P3 collapse = Refinement (bistability via subsystem mechanisms rather than cross-system unifier), not Fail. Core Claims 2-3 survive.
   - **P1** (convergence → causation): most directly implicates **Core Claim 1**. Most consequential priority for Core-scale findings.
   - **P2** (remaining self-reinforcement loops): **Peripheral** scope. Each loop correction is Refinement-scale (CO₂ precedent).
   - **P4** (bistability outside diabetes): qualifies **Core Claim 2's** generalization across disease categories.

3. **Unpack the prediction chain link by link.** Most claims decompose into premise → inference → conclusion chains. Mark each link as *textbook / well-supported / contested / inferred*. Target attack effort on contested and inferred links. Searching for evidence on textbook links wastes effort and misses the actual question.

4. **List adjacent measurements before searching.** The vault uses specific vocabulary; the broader literature may use related terms whose evidence is more direct. Anchor on the underlying physiology, not the vault's vocabulary. (Example: for "CO₂ production," list V'CO₂, indirect calorimetry, BMR, RQ, resting energy expenditure — not just ETCO₂.)

5. **State falsifiers explicitly.** What observations would be inconsistent with the claim? If nothing could falsify it, reformulate before proceeding. An unfalsifiable claim is not testable.

### Phase 2 — Attack

**Purpose:** honestly attempt to break the claim, using the vault's own Verification Sequence as attack machinery, with H1→H2→H3 discipline to prevent both failure modes.

#### Apply the Verification Sequence (six steps, from the Verification Methodology)

**Step 1 — Deeply understand what the vault predicts.** Trace the reasoning chain through wikilinks. Read System Connections tables. Before attacking, verify you can state what the vault's own logic predicts when followed all the way through. If you cannot trace it, you do not understand the vault well enough to assess contradictions.

**Step 2 — Check the framework's own metrics.** V'CO₂, ETCO₂, RQ, blood lactate, body temperature, resting pulse, mitochondrial function markers (Complex IV activity, cardiolipin composition, coupling efficiency). What does each predict for this case? What has actually been measured?

**Step 3 — State the contradiction (if one survives Steps 1-2).** Many apparent contradictions dissolve. If one survives, state it precisely: exact vault claim, exact evidence, why they cannot be reconciled.

**Step 4 — Identify what a resolution would depend on.** Write down each load-bearing sub-claim. If any collapses, the resolution collapses.

**Causal Independence Audit** (applied at Step 4, where a claim invokes a metabolite's causal role). Four sub-checks from Pearl's do-calculus + MCA conservation relations:
- **Conservation check.** Is the metabolite stoichiometrically locked to another variable under the physiological regime?
- **Mechanism specificity check.** Does it act on the downstream target through a specific named molecular mechanism the stoichiometric partner does not share? Or is the mechanism a non-specific bulk effect the partner would also produce?
- **Realizable intervention check.** Is there a physiologically achievable intervention that dissociates the metabolite from its partner with differential downstream effects?
- **Quantitative dominance check.** At the concentrations/timescales/tissue locations where the loop is claimed to operate, does the metabolite's effect magnitude exceed its partner's?

Classification: **independent driver** / **parallel marker** / **gated driver** / **co-driver** / **indeterminate**. (The CO₂ demotion came from this audit applied to Loop 7.)

**Step 5 — Verify each dependency against primary sources.** For every load-bearing citation:

- **Separate citation accuracy from claim accuracy.** A vault citation can be wrong while the underlying claim is supported by other evidence the vault didn't cite. Check these as separate questions in order.
- **Citation Deployment Audit** — go beyond topical relevance:
  - **Species match** (organism the vault's claim operates on?)
  - **Scenario match** (physiological scenario the vault is claiming?)
  - **Endpoint match** (measures what the vault's claim operates on?)
  - **Proposed-mechanism match** (authors attribute it to the same mechanism the vault invokes?)

Apply the same rigor to supporting evidence as to refuting evidence. Evidence that conveniently confirms what you want to conclude is exactly what needs the hardest pull.

**Step 6 — Construct and stress-test the resolution.** Only after Steps 1-5. Then:
- What is the weakest link?
- Am I being more generous to this resolution than I would be to someone else's?
- Does it make the framework more precise or more flexible? (Decisive test, see Phase 3)
- What new predictions does it generate? If none, it may be accommodation disguised as refinement.

#### H1 → H2 → H3 Escalation Discipline

Before concluding the vault is wrong, explicitly check in order. Do not skip steps.

- **H1: Am I misunderstanding the vault?** The most common case, and the most dangerous because it feels like understanding. The vault is not a collection of independent claims — it's an integrated system where meaning depends on connections. Reading individual statements at face value produces contradictions the vault doesn't actually contain. Trace the reasoning chain through wikilinks. Ask: does the vault's own logic handle this case through its stated principles? Most apparent contradictions dissolve here.

- **H2: Does the evidence measure the variables the vault's claims operate on?** The vault operates at the level of mitochondrial oxidative metabolism. Much research measures proxy endpoints (blood lipids, HbA1c, body weight, serum hormones, inflammatory markers). Evidence measuring proxies cannot confirm or deny vault claims at the mechanistic level, regardless of outcome.

- **H3: The vault is wrong.** Only after H1 and H2 are ruled out. Bar: specific, replicated, confirmed in relevant organism, directly measures the variables the vault's claims operate on, survives deep reading, precisely stateable (exactly what the vault says, exactly what the evidence shows, exactly why they cannot be reconciled).

#### Additional Attacks

Run alongside or after the Verification Sequence:

- **Steel-man critique.** Write the strongest version of the counter-argument an informed skeptic would make. Don't weaken it. Name specifically: "A theoretical biologist / biochemist / systems modeler would attack this by saying X." Grapple with X.
- **Alternative explanations.** Is there a different account fitting the evidence at least as well as the vault's claim? If yes: what observation would distinguish them? If nothing distinguishes, the vault's claim is underdetermined — a specific kind of weakness.

#### Rule Compliance Check (applicable when a resolution invokes acute/chronic or context-dependence)

If a stress-test resolution rescues a claim by invoking these, verify the invocation is legitimate:

- **Rule 1 (acute/chronic).** Classification must be based on entry mechanism and termination architecture (biological features observable independently of outcome), NOT on whether the outcome was healthy or pathological. Classifying by outcome is circular and invalidates the resolution.
- **Rule 2 (context-dependence).** All three conditions must hold: context variable specified in advance, independently measurable (not defined by the outcome), prediction directional and falsifiable.

If the rescue violates these, the resolution is invalid and the challenge stands.

### Phase 3 — Adjudicate

**Purpose:** produce an honest verdict using the vault's own classification system.

1. **Verdict: Pass / Refinement / Fail.**
   - **Pass** — existing architecture handles the case with no modifications. The framework already contained the stated principles needed.
   - **Refinement** — architecture modified to be *more precise and more predictive*: narrows what it claims, generates new testable predictions, core survives intact, practical recommendations may be updated but not reversed.
   - **Fail** — architecture modified to be *more vague or less predictive*: widens what it can explain, generates no new predictions, or abandons/weakens a core claim, or practical recommendations must be reversed.

2. **Apply the Decisive Test.** After resolution, does the framework predict *more* specific things than before, or *fewer*? Refinements increase specificity. Fails decrease it. If a proposed change makes the vault more complex without making it more precise, it is not an improvement.

3. **Classify scope: Core or Peripheral.** Modifications affecting Core Claims 1-5 are **Core**. Everything else is **Peripheral**. Core changes face the highest bar.

4. **Apply the change bar** (from the Verification Methodology). For findings that might trigger vault modification, all four must hold:
   - Verified evidence (replicated, confirmed in relevant organism)
   - Directly measures the variables the vault's claims operate on (not proxies)
   - Survives deep reading of the vault's logic
   - Precisely stateable: what the vault says, what the evidence shows, why they cannot be reconciled

5. **Confidence change.** Directional and specific. "Confidence increased because X." Not "confidence remains high."

6. **Document the finding.** Structured record in the stress_test/ per-priority file (template below). Update tracking table in [[Core Stress Test Priorities]]. Findings clearing the change bar produce proposed refinements. Findings that don't clear it are preserved with their evaluation — the reasoning stays on record.

---

## Documentation Standard

Each priority produces one file in `stress_test/`:

```
stress_test/
  P3 — State-Dependent Damping.md
  P1 — Convergence to Causation.md
  P2 — Self-Reinforcement Loops.md
  P4 — Bistability Outside Diabetes.md
```

Template for each file:

```markdown
---
priority: P3
claim: [one-line]
scope: [core | peripheral]
status: in-progress | complete
verdict: [pass | refinement | fail]
confidence-change: [specific]
started: YYYY-MM-DD
completed: YYYY-MM-DD
---

# P[N] — [Claim name]

## Phase 1 — Define the Target
### 1.1 Restatement
### 1.2 Core Claim relationship
### 1.3 Prediction chain (textbook vs contested vs inferred)
### 1.4 Adjacent measurements
### 1.5 Falsifiers

## Phase 2 — Attack
### 2.1 Verification Sequence
- Step 1: Vault's prediction (traced)
- Step 2: Framework's own metrics
- Step 3: Contradiction statement (if surviving)
- Step 4: Resolution dependencies + Causal Independence Audit (where applicable)
- Step 5: Dependency verification + Citation Deployment Audit
- Step 6: Resolution stress-test
### 2.2 H1 → H2 → H3 check (only if moving toward "vault is wrong")
### 2.3 Steel-man critique
### 2.4 Alternative explanations
### 2.5 Rule compliance (if applicable)

## Phase 3 — Adjudicate
### 3.1 Verdict (Pass / Refinement / Fail)
### 3.2 Decisive test (more or fewer specific predictions?)
### 3.3 Scope (Core / Peripheral)
### 3.4 Change bar assessment
### 3.5 Confidence change
### 3.6 Proposed refinement (if any)
```

The summary goes back to the tracking table in [[Core Stress Test Priorities]].

---

## The Plan

### Attack order

1. **P3 — state-dependent damping.** First. Most empirically inferred; highest probability of producing a definitive finding either way. Outcome informs how we read P2 (loops closing via ATP-dependent mechanisms) and P4 (cross-system damping signature). Also validates the Causal Independence Audit's application to cross-system claims before we extend it to individual loops.
2. **P1 — convergence to causation.** Second. Most consequential for Core Claims (most directly implicates Core Claim 1). Somewhat independent of P3 structurally — could be run earlier if consequence-ordering is preferred over information-ordering, but P3 first gives us maximum information gain for the effort.
3. **P2 — self-reinforcement loops.** Third. Each loop runs through the Causal Independence Audit (the same test that caught CO₂). Can be batched once the per-loop pattern is clear. Peripheral-scope findings mostly; cumulative weight matters more than any single loop.
4. **P4 — bistability outside diabetes.** Fourth. Qualifies rather than collapses Core Claim 2's generalization. Benefits from P3 settled (if cross-system damping is the unifier, other diseases should show the same signature, not just clinical hysteresis).

### Dependencies

- **P3 → P2.** State-dependent damping status affects how we read loop claims, because several loops close through ATP-dependent mechanisms. Do P3 first.
- **P3 → P4.** If P3 holds, bistability outside diabetes should be evaluated partly via the cross-system damping signature, not just clinical hysteresis.
- **P1 is mostly independent.** Can be run anytime. Placed after P3 for information-ordering reasons.

### P3 substructure

P3 is decomposed into four sub-questions for efficient attack:

- **3a.** Does each named damping system (HPT, HPA, GSH/SOD/GPx, PGC-1α biogenesis, PINK1/Parkin autophagy, SPM immune resolution, hepatic regeneration, lactate oxidation) genuinely have ATP as rate-limiting under disease-state conditions?
- **3b.** Do they actually fail together on correlated timescales?
- **3c.** Is there a direct cross-system measurement, or only pattern-inference from individual systems?
- **3d.** Is ATP actually the primary shared currency, or do alternative currencies (NADPH for GSH, NAD+/NADH for sirtuins, cofactor supply, membrane potential) operate independently in ways that decouple the systems? **3d is itself a Causal Independence Audit applied to ATP as unifier.**

Phase 2 attacks will be applied to each sub-question where relevant.

### Stopping rules

- **Per priority:** stop when Phase 3 produces a verdict with specific reason. If evidence exists, use it. If it doesn't, honestly mark "gap requiring empirical research we cannot perform" and document the gap. Don't keep attacking a claim with a clear verdict.
- **Per attack:** if an attack finds a clear weakness, note it and continue to the remaining attacks (we still want the full picture). If an attack finds strong confirmation that makes subsequent attacks obviously redundant, note that and move on.
- **Overall:** the stress test is done when all four priorities have verdicts. Proposed vault modifications clearing the change bar are logged. Unresolved gaps are documented as "known gaps in the foundation."

### Efficiency principles

- **Use the vault first.** Its own articulation of its claims + its own strongest cited evidence = starting point. H1 first, not last.
- **Reason from first principles before searching.** If the logic audit alone produces a verdict, we don't need external evidence-gathering. If it doesn't, we do.
- **Search when it matters.** External literature when (a) vault's evidence needs independent verification, (b) stress-test requires evidence vault doesn't cite, (c) checking for updates since `last-verified`.
- **Batch evidence-gathering where claims overlap.** Example: literature on state-dependent damping across systems may surface evidence for specific P2 loop claims too.
- **Don't generate attacks artificially.** If an attack axis doesn't yield meaningful content for a given claim, say so and move on rather than manufacturing weak content for completeness.
- **Use the vault's tools rather than reinventing.** Causal Independence Audit, Citation Deployment Audit, H1-H2-H3 sequence, Pass/Refinement/Fail classification — these exist, they work, they've caught real errors. Use them.

---

## Expected Scope

Rough estimate per priority:

- **P3:** most effort. Four sub-questions; each deserves attention; 3c and 3d are the critical ones (direct cross-system measurement + alternative currency audit). Longest single stress test.
- **P1:** medium. Focused on one logical step (convergence → causation) with associated evidence. Expect the H1 check to do a lot of work here — the vault's "five structural factors" + resmetirom may handle more of the case than the surface makes obvious.
- **P2:** medium-to-fast per loop, but many loops. Can be efficient once the Causal Independence Audit pattern is applied cleanly.
- **P4:** fast-to-medium. Targeted literature search for hysteresis and critical-slowing evidence in specific non-diabetic disease categories.

---

## Workflow Summary

For each priority:

1. Create `stress_test/P[N] — [name].md` from template
2. Phase 1: define the target, classify against Core Claims, unpack prediction chain, state falsifiers
3. Phase 2: run the Verification Sequence (6 steps), apply H1→H2→H3 before concluding "vault is wrong," add steel-man + alternatives, check Rule compliance if applicable, **apply Methodology Guardrails below**
4. Phase 3: adjudicate (Pass/Refinement/Fail, decisive test, scope, change bar, confidence, documentation)
5. Update tracking table in [[Core Stress Test Priorities]]
6. If findings clear the change bar: prepare proposed refinement for the relevant vault document
7. Move to next priority

---

## Methodology Guardrails (Lessons from Active Stress Tests)

These are specific failure modes identified during actual stress tests and the disciplines that prevent them. **Apply these in Phase 2 of every stress test going forward.**

### Guardrail 1 — Causal Chain Tracing Discipline

**Failure mode to prevent: Parallel-Intervention Misattribution.**

Treating "intervention A and intervention B both help disease X" as evidence that "A and B operate at equivalent causal levels, therefore the mechanism A and mechanism B target are parallel candidate primary causes."

This is a **logic error**, not a minor sloppiness. An upstream intervention and a downstream intervention on the *same* causal cascade can both produce clinical benefit — they reduce damage at different points in the same chain. Equivalent effect sizes do NOT imply equivalent causal priority.

Example of the error:
```
Observed:  Intervention A (metabolic) helps disease X.
           Intervention B (anti-inflammatory) helps disease X.
Faulty:    A and B are parallel primary causes of disease X.
           Metabolism and inflammation are equivalent convergence points.
Correct:   A and B might be on the SAME causal chain — A upstream, B downstream.
           Both help; this says nothing about their relative causal priority.
```

Analogy: spraying water on a fire and fixing the leaking gas line both reduce damage. Both work. Neither being a successful intervention tells you which is the upstream cause.

**The discipline: Trace causal chains BACKWARD before treating parallel-trial evidence as refutation of upstream causation claims.**

Procedure for each intervention cited as evidence:

1. **Identify the immediate target.** What molecular/cellular node does the intervention block, activate, or remove?
2. **Trace upstream.** What causes the state the intervention is targeting? What activates this pathway? What damage signal triggers it?
3. **Ask: is the proposed upstream cause in the chain?** If yes, the intervention targets a downstream node of a cascade whose upstream is the proposed cause.
4. **Classify the evidence:**

| Intervention targets | Outcome | What this evidence tells you |
|---|---|---|
| Proposed upstream directly | Works | **Supports** upstream causation |
| Proposed upstream directly | Fails | **Weak evidence against** (check intervention specificity — see Guardrail 2) |
| Downstream of proposed upstream | Works | **Consistent with** upstream causation (does NOT refute; downstream therapy is valid) |
| Truly parallel pathway (not in same chain) | Works | **Supports parallel** upstream causation as alternative |
| Proposed upstream directly | Insufficient | Check for multi-input threshold (bistable regime requirement) |

**Worked example (P1 stress test, 2026-04-17 — the mistake that motivated this guardrail):**

CANTOS trial: canakinumab reduces IL-1β → reduces cardiovascular events + lung cancer. Initially cited as refutation of "metabolism is dominant convergence point across chronic disease." **This was wrong.**

Causal chain trace (what I should have done in Phase 2):
- Canakinumab target: **IL-1β**
- IL-1β source: **NLRP3 inflammasome activation**
- NLRP3 triggers: **mROS, mtDNA release into cytoplasm, oxidized cardiolipin, AGEs from hyperglycemia, oxidized LDL, cholesterol crystals, ceramides, Ca²⁺ dysregulation**
- Every major NLRP3 trigger: **downstream of metabolic/mitochondrial dysfunction**

CANTOS patients had prior MI with elevated hsCRP. They were inflamed because they had atherosclerosis, which involves dyslipidemia, insulin resistance, vascular mitochondrial dysfunction — upstream metabolic failures. Canakinumab blocks a downstream step in a cascade whose upstream is metabolic.

Correct interpretation: CANTOS success is **consistent with metabolism as upstream convergence point**, not refutation of it. The trial shows downstream intervention on a metabolic cascade can produce clinical benefit — valuable for therapy, irrelevant as evidence for "metabolism isn't the upstream cause."

Same analysis correctly applied to:
- **Senolytics:** senescence is largely triggered by metabolic/oxidative/replicative stress (ATP-dependent DNA repair failure, mROS, metabolic cofactor depletion) → senolytic efficacy is downstream intervention
- **GrimAge mortality prediction:** incorporates inflammation, cardiovascular, and metabolic surrogates → integrative measure, not competing unifier
- **Hallmarks of aging "networked peers" framing:** describes network topology, not causal direction; when causal chains are traced, most hallmarks have metabolism upstream

### Guardrail 2 — Intervention Specificity Caveat

**Failure mode: Treating any failure of a metabolic intervention as refutation of metabolism-as-upstream.**

A specific metabolic intervention may fail not because metabolism isn't upstream, but because the intervention addresses a different metabolic node than the one actually disrupted in the specific disease.

**The discipline: When a metabolic intervention fails, check whether it addressed the specific metabolic mechanism disrupted in the disease, OR a different metabolic mechanism.**

Worked example (P1 stress test):

CoQ10 failed in Huntington's disease (CARE-HD, 2CARE stopped for futility). Initially cited as evidence that metabolic intervention doesn't work in HD.

- CoQ10's metabolic target: **ubiquinone pool** (Complex II → III electron transfer)
- HD's mitochondrial dysfunction mechanism: **mHTT disrupts TIM23 mitochondrial protein import complex**
- TIM23 disruption: cannot be addressed by CoQ10 supplementation

CoQ10 failed in HD because it targeted the wrong metabolic node, not because metabolism isn't upstream in HD. The vault's original Convergence Point Reading refinement correctly identified mHTT → TIM23 → OXPHOS as the pathogenic cascade. CoQ10-HD is evidence about intervention specificity, not about metabolic primacy.

### Guardrail 3 — Mechanistic Specificity vs Unfalsifiability

**Failure mode: Treating legitimate mechanistic causal tracing as unfalsifiable "everything is metabolism" hand-waving.**

There is a genuine unfalsifiability risk for the vault's claim: "all non-metabolic interventions that work are actually working via metabolism downstream." This becomes unfalsifiable if every non-metabolic success is vaguely reinterpreted as "somehow metabolic."

But there is ALSO a false-positive risk: treating any "metabolism upstream" interpretation as the unfalsifiability move, when the interpretation is actually grounded in specific traceable mechanisms.

**The discipline:**

"Metabolism is upstream" is **unfalsifiable** if:
- The claim is stated without mechanistic specificity
- The upstream pathway isn't named
- "Metabolism" is used as a catch-all for any cellular dysfunction

"Metabolism is upstream" is **legitimate mechanistic causation** if:
- Specific pathway is named (e.g., mROS → NLRP3 → IL-1β)
- Each step in the chain is independently evidence-supported
- Predictions follow from the specific chain that could distinguish it from alternative causal topologies

Test: "Can I describe the specific molecular pathway from the proposed upstream cause to the downstream intervention target? If yes, it's mechanistic tracing. If I'm hand-waving because every cellular function needs ATP, it's unfalsifiability risk."

### Guardrail 4 — Topology vs Causation

**Failure mode: Treating network-topology frameworks as causal-direction claims.**

The hallmarks-of-aging framework describes multiple hallmarks as "interdependent." This is a statement about network topology — the nodes are connected. It does NOT specify which direction causation runs between nodes.

**The discipline:**

When evaluating framework language like "interdependent," "networked," "interconnected," "integrated" — ask:

- Is this a claim about mutual influence (both directions)?
- Is this a claim about causal direction (specific upstream-downstream relations)?
- Or is this a non-specific topological description that's agnostic on causation?

For any node in a network, the question "is this node upstream or downstream of node X?" requires specific causal evidence, not just a description that they're connected.

Worked example: "Mitochondrial dysfunction and chronic inflammation are interdependent hallmarks of aging" is topologically accurate but **does not specify** whether mitochondrial dysfunction causes chronic inflammation, chronic inflammation causes mitochondrial dysfunction, or both directions operate. Causal analysis is needed for directional claims.

### Guardrail 5 — Overcorrection Pass After Verdict Flip

**Failure mode: Swinging too far in the opposite direction when correcting a wrong verdict.**

When a stress-test verdict is flipped (e.g., from Refinement to Pass after applying Guardrail 1), the natural tendency is to swing to the opposite pole. A wrong "too harsh" verdict gets replaced with an equally wrong "too generous" verdict. Both are wrong — they just differ in which direction.

**Specific risk after applying Guardrail 1 (Causal Chain Tracing):** Once you realize that downstream intervention success doesn't refute upstream causation, the temptation is to reinterpret every non-framework-aligned piece of evidence as "downstream of the framework's upstream variable." This creates new unfalsifiability risk — the framework gets over-rescued.

**The discipline: After a verdict flip, do an explicit pass looking for overcorrection.**

Checklist:
1. Am I now treating evidence that genuinely refutes the framework as "downstream of the framework's variable" through hand-waving?
2. Are there disease categories / contexts / mechanisms I'm now brushing aside that actually do refute the claim?
3. Is there a middle position I collapsed through too cleanly?
4. Am I applying Guardrails 3 and 4 symmetrically to BOTH directions of the claim, or only to defend the framework?

**Worked example (P1 stress test, 2026-04-17 — second correction):**

First correction applied Guardrail 1 correctly — CANTOS and senolytics are downstream interventions. But the first-corrected verdict ("Pass, metabolism as dominant convergence point") overshot. Triangulation caught:

- NLRP3 has non-metabolic triggers (bacterial toxins, crystal arthropathies, asbestos) that I glossed over by claiming "all NLRP3 triggers are metabolic"
- Senescence has non-metabolic primary modes (oncogene-induced, developmental, telomere-mechanical)
- Proteostasis has ATP-independent components (small heat shock proteins)
- Autoimmune, monogenic structural, primary mental illness have primary non-metabolic lesions
- Several "metabolism upstream" chains were directionally ambiguous or topological rather than causal

Second correction: "Pass with SCOPED observations" — metabolism as dominant convergence point holds for aging-associated/acquired chronic disease, not universally. Specific disease categories require explicit scope exclusion.

### Guardrail 6 — Apply Causal Independence Audit to Umbrella Terms

**Failure mode: Treating the vault's upstream variable as a single unified thing when it's actually an umbrella covering heterogeneous signals.**

When the vault claims "X is the upstream cause" where X is a broad term (metabolism, inflammation, stress, immune dysfunction), apply the same Causal Independence Audit that would be applied to a specific metabolite. Decompose X into its constituent signals and ask: are they a single variable, or heterogeneous signals that happen to co-occur?

**The discipline:** Before accepting "metabolism is the shared upstream variable" (or any similar umbrella claim), ask:
1. Is "metabolism" a single variable, or does it cover multiple distinct signals (ATP, NADPH, NAD+, Δψ_m, mROS, mtDNA, lipid species, AGEs, etc.)?
2. Do all these signals track together under the conditions the framework operates on, or do they dissociate?
3. Is the framework's upstream claim actually "metabolism as single variable" or is it "several different signals that happen to be categorizable as metabolic"?

**Worked example (P1 stress test, 2026-04-17 — second correction):**

In P3, I correctly decomposed "ATP" into multiple coupled currencies (ATP, NADPH, NAD+, Δψ_m) via Causal Independence Audit. In P1's first correction, I did NOT run the analogous audit on "metabolism." When I traced CANTOS back to NLRP3 triggers (mROS, mtDNA, oxidized cardiolipin, AGEs, oxLDL, cholesterol crystals), I categorized them all as "metabolic failure signals" without asking whether they're a single upstream variable or heterogeneous signals.

The triangulation Agent 3 caught this asymmetry: "The NLRP3 triggers are at least as heterogeneous as the four currencies P3 separated. Calling them all 'metabolic' is the same umbrella move that P3 corrected against for 'ATP.'"

**Corrected discipline:** When applying Guardrail 1 (Causal Chain Tracing), check whether each step in the chain is a well-defined molecular mechanism or an umbrella term that itself needs decomposition. If umbrella: apply Guardrail 6 before accepting the chain as valid.

### Guardrail 7 — Soft-Language Hedge Audit

**Failure mode: Using soft hedging language to create an impression different from what the evidence actually shows.**

Words like "modulate," "support," "may be," "can contribute," "is associated with" — these hide what the hard language would reveal. In the P1 scope-out that was caught in 2026-04-17: I used "metabolism can modulate when autoimmunity becomes clinical" when the evidence actually showed metabolism is the clinical trigger converting latent susceptibility into disease. "Modulate" was soft language hiding "trigger."

The hedging can happen in both directions:
- **Soft-downward** (what P1 scope-out did): "metabolism merely modulates" → hides that metabolism is actually central
- **Soft-upward**: "X may be primarily metabolic" → hides that evidence is actually weak

**The discipline:** For every claim involving softening language, ask: "What would the hard version of this claim say? Is the hard version supported by evidence? If yes, use the hard version. If no, acknowledge explicitly that evidence is weaker than the claim."

Words that trigger the audit:
- "modulate," "support," "affect," "influence" — can hide either "cause" or "mere correlation"
- "may be," "could be," "might" — can hide either "is" or "is not known to be"
- "associated with," "linked to" — hides causal direction
- "complex," "bidirectional," "networked" — can hide "we don't know the direction"
- "plays a role," "is involved in" — hides the strength of the involvement

**Worked example (P1 scope-out correction, 2026-04-17):**
- Original: "Metabolism can modulate WHEN susceptibility becomes clinical (via β-cell stress, gut endotoxin, thyroid effects on thymus)"
- Hard version: "Metabolism is the clinical trigger that converts latent genetic susceptibility into clinical autoimmune disease. HLA/TCR susceptibility alone is not sufficient — most carriers never develop clinical disease. Metabolic triggers (gut barrier failure, β-cell ER stress, thymic involution) are what activate the susceptibility."
- The hard version is supported. The softened version created a false impression of peripheral metabolic role.

### Guardrail 8 — Source Reading Discipline

**Failure mode: Taking research papers at face value without interrogating what was actually measured, in whom, under what incentives, and what mechanism claims are data-backed vs. speculative.**

Academic papers are not neutral evidence. They embed:
- Authorial framework (what the researcher was prepared to see)
- Funding incentives (what pharma wanted to justify; what agency grants funded)
- Publication bias (positive results publish; null results disappear)
- Clinical trial surrogate endpoints (biomarkers measured instead of disease states)
- Discussion-section mechanism speculation presented as if data-backed
- Technical terms used loosely or as metaphors instead of in their precise dynamical/biochemical sense

**The discipline (applied to every load-bearing source):**

1. **Evidence vs. narrative.** What was actually measured (results section, tables, figures)? Not what the abstract claims. Not what the discussion speculates.

2. **Population and scope.** In whom? At what disease stage? Over what time? Longitudinal or cross-sectional? Human or model organism? A narrow population can't support broad claims.

3. **Surrogate vs. real endpoint.** Did they measure a biomarker (HbA1c, LDL, ejection fraction) or the actual vault variable (mitochondrial function, V'CO2, oxidative phosphorylation capacity)? Biomarker change ≠ disease state change.

4. **What wasn't measured.** Absence of measurement ≠ absence of effect in either direction. If the paper didn't measure mitochondrial function, it cannot support or refute claims about it.

5. **Mechanism claims vs. mechanism data.** Discussion sections speculate about mechanism; results sections show what was measured. A paper can show A→B correlation while the authors speculate about mechanism Y without having measured Y at all.

6. **Funding and authorial framework.** Who funded it? What framework does the author work in? Pharma-funded trials optimize for the drug's story; researchers see what their framework prepares them to see.

7. **Technical term vs. metaphor.** "Hysteresis," "threshold," "tipping point," "bistability" appear in clinical literature sometimes as precise dynamical terms and sometimes as loose metaphors. Check which one the paper means. The vault's claims operate at the precise technical level.

8. **Absence of evidence vs. evidence of absence.** If a bistability signature isn't in the literature for disease X, this could mean: (a) nobody measured it (sampling bias, not measurement result), (b) it was measured and not found, (c) it was measured and found but framed differently. Collapsing (a) to either presence or absence is a reasoning error.

**Application in Phase 2:** For every source cited to support or refute a claim, produce a one-sentence mini-audit:
- What was actually measured
- Population and time frame
- Surrogate or vault variable
- Mechanism data or mechanism speculation
- Funding/framework flags
- Technical-sense vs. metaphorical-sense of key terms

This is the Citation Deployment Audit applied to *every* source, not just load-bearing ones. And it's a separate discipline from the reasoning errors — reasoning guardrails (G1-G7) are about how we reason; G8 is about how we read.

### How to Apply These Guardrails

In Phase 2, after running the Verification Sequence but before adjudicating in Phase 3:

1. **Source reading first** (Guardrail 8) — for every source cited, produce the mini-audit. If sources fail the discipline, the downstream reasoning is compromised.
2. List every intervention/evidence cited that supports any causal claim (in either direction)
3. For each, run the Causal Chain Tracing procedure (Guardrail 1)
4. For any metabolic intervention failure, apply the Intervention Specificity Caveat (Guardrail 2)
5. Before claiming something is upstream or downstream, verify mechanistic specificity (Guardrail 3)
6. For any framework-language claims ("interdependent," "networked"), distinguish topology from causation (Guardrail 4)
7. Decompose umbrella terms into their constituent signals; verify each signal is actually a single variable (Guardrail 6)
8. For any softening language ("modulate," "support," "may be"), run the Hard-Version Test (Guardrail 7)

After Phase 2 produces a verdict, BEFORE Phase 3 adjudicates:

9. If the verdict is different from the vault's (i.e., refinement or fail), do an overcorrection pass (Guardrail 5) — check for unfalsifiable rescue moves you might be making to defend your own corrected verdict

**Evidence that survives these guardrails is stronger than effect-size comparison. Evidence that fails them needs to be recharacterized before adjudication. The guardrails apply symmetrically to protect both the vault from unfair critique AND the analysis from motivated overcorrection.**
