---
title: "Core Stress Test Priorities"
tags:
  - stress-test
  - verification
  - working-document
status: active
started: 2026-04-17
scope: foundational
---

# Core Stress Test Priorities

## Purpose

Before investing deeply in learning the vault, verify that its load-bearing non-textbook claims hold up under rigorous first-principles examination. The cost of installing wrong intuitions is higher than the cost of delaying the install — so this document identifies exactly where the stress-test effort should go.

This is **not** a re-verification of every claim in the vault. It targets the specific points where the core **architecture** rests on inference rather than textbook fact. If these hold, the architecture is solid and downstream investment is safe. If any fail, we know exactly where the weakness sits and what it does or doesn't affect.

Governance: changes to the vault triggered by findings here run through [[metabolic_framework/Verification Methodology]] — the three hypotheses, the bar for change, the six-step sequence.

The method for stress-testing each priority, the attack order, dependencies, and documentation standard are in [[Stress Test Plan]]. This document is *what* to test; that document is *how*.

---

## The Foundation at a Glance

| Layer | What it is | Stress-test need |
|---|---|---|
| **Ground** | Life = ordered energy throughput against entropy | None — physics, textbook |
| **Architecture** | Two self-reinforcing basins; brakes degrade with the system | **This is where stress-testing lives** |
| **Instantiation** | Specific biology (thyroid, estrogen, PUFA, liver, etc.) | Absorbed corrections already; lower leverage for the architecture |
| **Application** | Practice, assessment, monitoring | Downstream of architecture; don't verify before the architecture is verified |

---

## What's Textbook (Does Not Need Stress-Testing)

The following are all textbook and not contestable at any serious level:

- Life as ordered energy throughput maintaining itself against entropy (physics — Schrödinger, Prigogine)
- ATP as universal currency of cellular work (~40 kg/day throughput in humans)
- Oxidative phosphorylation ~32 ATP vs. glycolysis 2 ATP (the 18× asymmetry)
- The pyruvate fork at PDH as binary decision point
- Bistability being mathematically possible in multi-loop systems with shared state variables and ultrasensitive responses (Thomas's condition, Gardner-Collins toggle, Brandman coupled ultrasensitivity)
- Individual mechanism pieces: Bohr effect, carbamino bonds, V-ATPase proton pumping, histone lactylation, HIF-1α biology, estrogen's PI3K/AKT glycolytic shift, endotoxin/iNOS/tight junction biology, PUFA peroxidation chemistry, iron-catalyzed Fenton chemistry

Each brick is solid. The stress test concerns how they're assembled into the architecture.

---

## What Rests on Inference (Needs Stress-Testing)

Four load-bearing non-textbook claims, ranked by leverage.

### Core vs Peripheral Classification

The vault's [[metabolic_framework/Verification Methodology]] pre-specifies five **Core Claims**. Anything affecting these is a **Core change**; everything else is **Peripheral**. Mapping the four priorities:

| Priority | What it tests | Scope | If collapsed |
|---|---|---|---|
| **P3** | State-dependent damping as cross-system unifier | **Distinctive contribution, NOT Core** | Refinement — bistability via subsystem mechanisms (ultrasensitivity, mutual inhibition, saturation — all still present); the cross-system unification story weakens but Core Claims 2-3 survive |
| **P1** | Convergence → common cause inference | **Implicates Core Claim 1** most directly | Potential Fail of strong formulation; may require retreat to "metabolism is the common level of convergence" rather than "common cause" |
| **P2** | Remaining self-reinforcement loops | **Peripheral** (per loop) | Refinement-scale; architecture unaffected if enough loops remain (CO₂ demotion precedent) |
| **P4** | Bistability outside diabetes | **Implicates Core Claim 2's generalization** | Refinement — Core Claim 2 becomes scope-qualified (confirmed in metabolic/endocrine disease; hypothesized elsewhere) |

This matters for the attack order: **P1 is most consequential for Core Claims; P3 is the most empirically inferred and highest probability of producing a finding**. We run P3 first for information yield; P1 second for consequence. See [[Stress Test Plan]] for the ordering rationale.

---

### Priority 1 — State-Dependent Damping as Cross-System Unifier (P3)

> [!abstract] Why this is first
> **The most empirically inferred claim in the vault and the framework's distinctive contribution.** It's the reason HPT, HPA, antioxidants, biogenesis, autophagy, immune resolution, hepatic regeneration, and lactate clearance fail *together* under one currency rather than independently. **Not a Core Claim** in the vault's pre-specified sense — the framework itself names state-dependent damping as "one of several mechanisms generating bistability" alongside ultrasensitivity, mutual inhibition, and saturation. If it collapses, the vault doesn't lose the individual feedbacks (each stays valid in its subsystem) and doesn't lose bistability (other mechanisms remain) — it loses the cross-system unifier that makes this framework distinctive.

**The claim.** Every negative feedback mechanism in the organism is ATP-dependent for the machinery that performs it (enzyme synthesis, folding, trafficking, cofactor regeneration), even when the regulatory act itself is thermodynamically free. Therefore, as mitochondrial function (M) falls, all damping systems degrade together. The effective gain of positive feedback rises non-linearly not because positive feedback strengthens, but because negative feedback weakens under a shared currency. This is the threshold mechanism.

**What's textbook.** Each individual example — antioxidant synthesis requires ATP, mitochondrial biogenesis via PGC-1α requires ATP, autophagy requires ATP, hepatic regeneration requires ATP, lactate clearance via oxidation requires ATP, protein synthesis/folding/trafficking all require ATP. Each is well-established in its own literature.

**What's inferred.** The *unifying* claim — that all these feedbacks share this dependence, degrade *together* under a common currency (ATP), and the simultaneity produces the cross-system threshold dynamics. This is structural inference from the pattern across subsystems, not a single measurement.

**What would need to be true.**
- ATP availability must genuinely be the rate-limiting variable for each of these negative feedback systems under disease-state conditions (not just under experimental starvation)
- The systems must degrade on similar timescales for their simultaneity to produce the threshold dynamics claimed
- Alternative currencies (NADPH, redox state, cofactor availability, substrate supply) must not be independently rate-limiting in ways that would decouple the systems

**What would falsify it.**
- Clean demonstration that one or more of the named negative feedback systems degrades *independently* of ATP availability under disease-state conditions
- Discovery that the systems fail on very different timescales (decoupled), such that "they fail together" is artifact of chronic-disease observation rather than shared currency
- Direct measurement showing that at disease-state ATP levels, several of the damping systems still operate at substantial capacity (implying something else is driving their functional failure)

**What would strengthen it.**
- Direct cross-system measurement: graded ATP perturbation (pharmacological or genetic) showing simultaneous degradation of multiple damping systems with correlated kinetics
- A quantitative model deriving threshold behavior from the coupling of damping systems through ATP as shared variable
- Intervention data: restoring ATP availability (via specific pathways) restoring multiple damping systems in lockstep rather than piecemeal

**Open questions to investigate.**
- What direct cross-system measurements exist in the current literature? Has anyone published a graded-perturbation study showing simultaneous damping-system degradation?
- How does the vault handle alternative rate-limiting currencies (NADPH for GSH regeneration, NAD+/NADH ratio for sirtuin activity, etc.)? Are these actually subordinate to ATP or genuinely independent?
- Is there a mathematical/computational treatment of the "coupled damping collapse" that could be pressure-tested?

**Current status.** `not yet investigated`

---

### Priority 2 — Convergence → Common Cause Inference (P1)

> [!abstract] Why this is second
> **The claim most directly implicating Core Claim 1** ("Health is efficient oxidative metabolism; disease is its progressive failure"). The logical step a sophisticated critic attacks first. The observation is documented; the inference from observation to causation is not strict entailment. If this inference collapses, the vault may need to retreat from "metabolic failure is the common *cause*" to "metabolic failure is the common *level* at which disease manifests" — a weaker but still meaningful claim. Expect H1 (am I misunderstanding the vault?) to do significant work here: the vault's "five structural factors" explanation and resmetirom example may handle more of the case than surface reading suggests.

**The claim.** Every chronic disease shows the same metabolic failure signature (elevated lactate, shifted respiratory quotient toward fat oxidation, mitochondrial dysfunction, impaired oxidative capacity). Therefore cellular energy failure is the common *cause*.

**What's textbook.** The observation. Cross-disease metabolic convergence is documented — cancer (Warburg), diabetes (metabolic inflexibility), heart failure (energetic starvation), neurodegeneration (mitochondrial dysfunction + iron + lipid peroxidation), NASH (now treated with thyroid receptor agonist).

**What's inferred.** The inference from convergence to common *cause*. A rigorous critic will say: convergence might indicate common *endpoint* rather than common *cause*. Many different upstream pathologies could converge at a shared downstream metabolic failure signature without metabolism being the driver.

**What would need to be true for the causation claim to hold.**
- Interventions targeting the metabolic failure upstream (rather than disease-specific pathways) should produce benefit across multiple disease categories simultaneously
- Temporal precedence: metabolic failure should appear before (or at least not after) the disease-specific pathology in well-tracked cohorts
- Dose-response: degree of metabolic restoration should correlate with degree of clinical benefit across disease categories

**What would falsify it.**
- Cohort data showing disease-specific pathology temporally preceding the metabolic signature (rather than the reverse)
- Metabolic restoration producing clinical benefit in one disease category but not others where the same signature exists
- Genetic/experimental models where metabolic failure is produced *without* producing the associated chronic disease features

**What would strengthen it.**
- Resmetirom as example: thyroid agonist (metabolic restoration) reverses NASH fibrosis — direct evidence at least in that disease
- Similar single-intervention evidence across other disease categories would close the loop substantially
- Longitudinal data showing metabolic signature predating disease-specific pathology in progressors

**Open questions to investigate.**
- How does the vault currently handle this logical step? Does it defend causation or just present convergence?
- What's the strongest available evidence for metabolic upstream-ness across disease categories? Resmetirom is one; what else?
- Are there disease categories where the convergence claim is weaker (autoimmune? psychiatric? early cancer?)

**Current status.** `not yet investigated`

---

### Priority 3 — Remaining Self-Reinforcement Claims (P2) — Check for CO₂-Style Errors

> [!abstract] Why this is third
> **Peripheral-scope findings mostly.** The CO₂ demotion established that this error mode is real in the vault — the Causal Independence Audit caught it, and may catch others. Each individual loop correction is Refinement-scale; cumulative weight matters more than any single loop. Uses the vault's own Causal Independence Audit (Pearl screening-off + MCA conservation) applied loop-by-loop.

**The claim.** Each state's outputs actively shape the conditions for the next state (not passive byproducts). Health produces CO₂ and ATP that sustain more oxidation; disease produces lactate that actively deepens glycolytic failure.

**What's textbook.** Each individual mechanism. Histone lactylation exists (Zhang 2019, *Nature*). V-ATPase biology is established. HIF-1α-driven M2 polarization is documented. Lactylation-driven collagen production / fibrosis is published.

**What's inferred.** That these mechanisms *causally close the loops* they're placed in. The CO₂ precedent showed that a plausibly causal mechanism could turn out to be a parallel marker of the same underlying metabolic process without specific causal participation in the loop.

**Loops to re-examine for possible CO₂-style errors.**

The CO₂ demotion already happened. Still to check:

- **Lactate → histone lactylation → glycolytic gene expression → more lactate.** Is the epigenetic reprogramming causally closing this loop, or is it a marker of the glycolytic state with causation running through some other variable? Zhang 2019 + subsequent lactylation literature — strong. But worth checking: does lactate-independent intervention (e.g., LDHA inhibition at the level of lactate production) actually reduce lactylation-driven reprogramming, closing the causal chain?
- **ATP → V-ATPase → granule pH → mediator release (Loop 7 refined).** Already the refined version. Is the refinement tight, or could ATP itself be a marker of a deeper variable (e.g., membrane potential) that's the true driver?
- **Estrogen → aromatase → more local estrogen (Loop 4).** Established in the literature. Worth sanity-checking against the newest aromatase biology.
- **Estrogen ↔ histamine (Loop 5).** Bidirectional mechanism claim. Both arms need to be genuinely causal, not parallel-marker.
- **PUFA ↔ estrogen (Loop 3).** PUFA displacement from SHBG increasing free estrogen — verify. Estrogen upregulating desaturases retaining/synthesizing more PUFA — verify tissue-level evidence.
- **Endotoxin ↔ barrier (Loop 10).** iNOS/NO/Complex IV/tight junction mechanism — check whether NO or ATP loss is the dominant driver of barrier failure.
- **Gut ↔ thyroid ↔ motility (Loop 12).** The intervention-tested loop (levothyroxine reducing SIBO risk). Strongest loop. Worth confirming it holds up.

**What would need to be true.** Each proposed mechanism must be genuinely causal (intervention on the mechanism alone must produce the claimed downstream effect), not merely correlational with the underlying state.

**What would falsify specific loops.** Intervention studies targeting the named mechanism that *don't* produce the predicted loop-closing effect (or produce it only weakly compared to intervention on an upstream variable).

**Current status.** `not yet investigated` — Loop 7 already refined, others not systematically re-examined since stress test layer 2.

---

### Priority 4 — Conditional Bistability Outside Diabetes (P4)

> [!abstract] Why this is fourth
> **Qualifies Core Claim 2's generalization.** Bistability is confirmed at four independent levels in diabetes (structural, mathematical, cellular, whole-organism). Generalization to cancer, neurodegeneration, autoimmune, heart failure is more inferential. If weakened, Core Claim 2 becomes scope-qualified — "confirmed in metabolic/endocrine disease; hypothesized elsewhere" — rather than categorically refuted. Refinement-scale, not Fail-scale.

**The claim.** The metabolic system exhibits conditional bistability across chronic disease generally — cancer, neurodegeneration, autoimmune, heart failure, metabolic syndrome — not just type 2 diabetes. Recovery requires crossing a threshold with multi-input intervention.

**What's textbook.** Bistability is mathematically possible (confirmed). In diabetes specifically, it is confirmed at four levels: structural (Thomas/Brandman), mathematical (Topp 2000), cellular (Mulukutla 2014), whole-organism (bariatric remission hysteresis + Tabak critical slowing).

**What's inferred.** That the same bistable architecture operates across other chronic disease categories. The strong confirmations are diabetes-specific.

**What would need to be true.**
- Similar hysteresis evidence (differential forward/reverse thresholds, disease-duration-dependent recovery) in other chronic diseases
- Critical slowing down signatures in longitudinal cohorts for other chronic diseases
- Multi-input threshold nonlinearity in interventions for other diseases

**What would falsify the generalization.**
- Finding that other chronic diseases show monotonic dose-response to metabolic intervention (no hysteresis) — which would suggest the bistable architecture is diabetes-specific, not metabolic-general
- Absence of critical-slowing-down signatures in longitudinal data for other progressive chronic diseases
- Differential forward/reverse thresholds being absent in other recoveries (e.g., early cancer remission, neurodegeneration stabilization)

**What would strengthen it.**
- Hysteresis evidence in cancer remission (stage-dependent recovery likelihood despite equivalent tumor reduction — analog to bariatric C-peptide effect)
- Critical slowing signatures in longitudinal pre-disease cohorts for other conditions
- Evidence of multi-input threshold effects in other chronic diseases

**Open questions to investigate.**
- Does the literature have bariatric-analog hysteresis evidence in other disease categories?
- Are there published critical-slowing analyses outside the Whitehall/Tabak diabetes tradition?
- What does the vault currently claim — categorical bistability for all chronic disease, or diabetes-confirmed with hypothesized generalization?

**Current status.** `not yet investigated`

---

## Lower-Leverage Items (Foundational But Not Core Architecture)

Flagged for completeness — not where primary stress-test effort should go first.

### State variable completeness

The vault identifies 6 state variables: M, T, E, P, L, Λ. Candidates the vault might be missing or subordinating too aggressively:

- **Redox state / NAD+/NADH ratio** — affects sirtuin activity, glycolytic flux regulation, DNA repair. Is the vault correct to subordinate this to M, or is it an independent variable?
- **Microbiome diversity** (beyond endotoxin load) — affects inflammation, bile acid signaling, neurotransmitter precursors. Endotoxin load captures part but not all.
- **Immune tone** — baseline inflammatory state independent of acute endotoxin. Not cleanly reducible to any of the 6.

Worth checking: does the vault make the subordination explicit, or is it implicit?

### Slow/fast timescale separation

The vault claims M and P are slow (days-weeks, weeks-months); T, E, L, Λ are fast (hours-days). The "sudden decline after gradual drift" prediction depends on this separation being clean empirically.

Worth checking: is the separation genuinely as clean as claimed, or are there intermediate-timescale variables that blur it?

---

## Priority Order for Effort

1. **P3 — State-dependent damping.** Highest information yield. Most empirically inferred. Uses the Causal Independence Audit on the cross-system unifier claim directly. Outcome informs how we read P2 and P4.
2. **P1 — Convergence → causation.** Highest Core-Claim consequence. Tests the logical step most directly implicating Core Claim 1. Placed after P3 for information-ordering rather than consequence-ordering; could be first if preferred.
3. **P2 — Remaining self-reinforcement claims.** Error mode known real (CO₂ precedent). Applies the same Causal Independence Audit loop-by-loop. Peripheral-scale but cumulative.
4. **P4 — Bistability outside diabetes.** Qualifies Core Claim 2's generalization. Benefits from P3 settled (cross-system damping signature as additional evidence axis).

After these four, the lower-leverage items are worth quick passes but unlikely to be foundational.

---

## Tracking

| Priority | Claim | Status | Started | Findings |
|---|---|---|---|---|
| P3 | State-dependent damping as cross-system unifier | **Complete — Refinement (triangulated + verified + guardrail-reviewed + triangulation additions)** | 2026-04-17 | Phase 1-6 complete. Three independent agents converged: "ATP as single shared currency" refuted; shared basis is mitochondrial respiratory capacity producing multiple coupled currencies (energy charge per Atkinson 1968/AMPK; NADPH; NAD+ in stressed contexts; Δψ_m — dissociable via uncouplers per PINK1/Parkin biology). Framework's "distinctive contribution" scoped — concept exists in frailty literature (Fried/Walston/Cohen 2020), genuine novelty is chronic-disease generalization + bistability-mechanism formalization. Phase 6 triangulation additions: (a) NADPH has indirect ATP coupling via hexokinase substrate supply (narrower independence than first claimed); (b) Δψ_m dissociation from ATP is primarily experimental (CCCP/FCCP) and per-organelle (mitophagy), not typical whole-cell steady-state in disease; (c) missing currencies to include: acetyl-CoA (for histone acetylation) and broader α-KG role (TET/JmjC demethylation); (d) SAM actually reinforces ATP-centrality (ATP-dependent synthesis); (e) Chubanava 2025 (85% NAD+ depletion with preserved function AND preserved mitochondrial respiration) is harder on NAD+ independence than initial incorporation. Verdict holds — Refinement, Peripheral scope. Core correction (ATP as single currency → mitochondrial function as shared basis with coupled currencies) stands. Compatible with P1's final scoped Pass verdict. See `stress_test/P3 — State-Dependent Damping.md` Phases 4-6. |
| P1 | Convergence → common cause inference | **Complete — Pass with SCOPED observations (after two corrections)** | 2026-04-17 | Iterated verdict: Original (wrong — Refinement weakening Core Claim 1) → First correction (too generous — Pass unrestricted) → Second correction (Pass with SCOPED observations — after triangulation caught overcorrection). Triangulation agents identified: (1) NLRP3 has non-metabolic triggers (bacterial toxins, crystals, asbestos, K+ efflux) — CANTOS chain is context-specific to atherosclerosis, doesn't generalize universally; (2) senescence has non-metabolic primary modes (OIS, developmental, telomere mechanical); (3) proteostasis has ATP-independent components (sHSPs); (4) disease categories where metabolism is genuinely NOT upstream: primary-autoimmune (HLA/TCR specificity), monogenic structural/channel (CF, sickle cell, Marfan), primary mental illness (bidirectionally entangled), primary neuropathic pain (ion channel). Agent 3's key critique: I decomposed "ATP" via Causal Independence Audit in P3 but failed to apply the same audit to "metabolism" as umbrella term in P1 — the NLRP3 triggers are heterogeneous, not a single "metabolic" variable. **Final verdict:** Core Claim 1 preserved at definitional level. Substantive Reading C (CF-1.A.1) holds for aging-associated/acquired chronic disease, explicitly scoped OUT for primary-autoimmune, primary-monogenic structural, primary mental illness, primary neuropathic pain categories. Guardrails 5 (overcorrection pass) and 6 (umbrella-term audit) added to Stress Test Plan. See `stress_test/P1 — Convergence to Causation.md` Phase 5. |
| P2 | Remaining self-reinforcement claims | not yet investigated (low-leverage, may skip) | — | — |
| P4 | Bistability outside diabetes | **Complete — Refinement (scope note added)** | 2026-04-17 | All 8 guardrails locked in pre-commitment for first time. G8 (source reading discipline) caught multiple abstract-vs-methods mismatches (CTMC memoryless explicitly excludes bistability; "bifurcation" in cardiology is anatomical not dynamical; "tipping point" in CKD literature is clinical metaphor not formal bifurcation). Per-disease: **Diabetes** (reference, not re-tested) — bistability empirically established via bariatric hysteresis + Tabak 2009 CSD. **Sarcopenia/Frailty** — strongest conceptual convergence (Fried/Walston 2021 Nature Aging independently identifies energetics as central driver of multisystem threshold-crossing) but formal bistability not demonstrated. **NAFLD/NASH** — insufficient data; asymmetric reversal compatible with structural irreversibility of fibrosis. **CVD** — tilts AWAY from bistability; field attributes asymmetry to cardiomyocyte loss (explicitly structural irreversibility). **Aging-associated neurodegeneration** — tilts AWAY; dominant frameworks are prion-like propagation + cognitive reserve exhaustion (both monostable). **CKD** — clearly AWAY; textbook nephron reserve exhaustion; multi-trajectory model explicitly forbids basin-switching. **Verdict:** Refinement, Core scope. Bistability empirically established in diabetes, inferred by analogy elsewhere. Alternative lock-in forms (structural, reserve, nucleation) are themselves downstream of metabolic failure — metabolism remains the upstream driver; the distinction is only which form of lock-in emerges. Practical architecture (multi-input, duration-dependent recovery, early-intervention leverage) follows from bistability AND alternative lock-in forms, so survives regardless. Core Claim 2 scope note + hysteresis prediction scope note applied to vault. Structural lock-in paragraph added to The System.md. See `stress_test/P4 — Bistability Outside Diabetes.md`. |
| — | State variable completeness | flagged, lower leverage | — | — |
| — | Slow/fast timescale separation | flagged, lower leverage | — | — |

---

## Governance

Findings from this stress test are evaluated against the vault through [[metabolic_framework/Verification Methodology]]:

- **Default position:** the vault is correct until proven otherwise with evidence that survives deep reading
- **Three hypotheses** for apparent contradictions (misreading / mechanism correction / integration error)
- **Asymmetry principle:** wrong change > wrong non-change — the bar for correction is high
- **Six-step verification sequence** before any proposed change to the vault

Findings that clear this bar produce proposed refinements. Findings that don't clear it are documented here with their evaluation, so the reasoning is preserved even when no vault change follows.
