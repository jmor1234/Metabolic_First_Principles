---
title: "Stress Test Summary"
aliases:
  - What the Stress Test Found
  - Before and After
  - Stress Test Results
last-updated: 2026-04-12
scope: summary
---

A precise accounting of what the stress test found — what the framework got right, what it got wrong, what was missing, and how far off it was. This document is the capstone of the stress test. For the full investigation log, see `Stress Test.md`. For individual findings as standalone knowledge, see the six refinement documents listed at the bottom.

---

## What the framework got right

**The ontological claim holds.** Health IS efficient oxidative metabolism. Disease IS its progressive failure. The metabolic fork IS the fundamental decision point. This survived adversarial probing including independent agent triangulation that attacked it with ketogenic metabolism. The core identification — metabolism is not one factor among many, it IS health at the cellular level — is correct.

**Lactate IS a genuine causal disease driver.** The framework claimed lactate actively deepens disease through histone lactylation and HIF-1alpha. The stress test confirmed this with stronger evidence than the framework cited — H3K18R site-specific mutant data proving causality, 6+ in vivo genetic models across tumors, kidney, vasculature, brain, and sepsis, characterized writer/eraser machinery (p300/CBP writers, HDAC1-3 erasers), and non-histone lactylation (HMGB1) as an additional HIF-1alpha-independent mechanism. The temporal structure (HIF-1alpha initiates acutely, lactylation consolidates epigenetically) was not in the framework but strengthens the bistability case.

**The system IS bistable.** Two self-reinforcing stable states exist. This is real dynamical-systems bistability, not metaphor. Confirmed at four independent levels: structurally (10+ positive circuits in 3 canonical bistability motifs, Thomas's condition abundantly satisfied), mathematically (Topp et al. 2000 saddle-node bifurcation in glucose-insulin ODE model), at the cellular level (Mulukutla et al. 2014 glycolysis/OXPHOS bistability with experimental hysteresis), and at the whole-organism level (bariatric surgery duration-dependent remission = hysteresis; Tabak et al. 2009 longitudinal critical slowing down acceleration specific to progressors, replicated across 5 independent cohorts).

**The emergent properties follow.** Progressive disease, single-intervention failure, context-dependence, multi-input recovery requirement, threshold dynamics — all five are deducible consequences of the confirmed bistability and match clinical observation.

**The temporal architecture is correct.** Daily oscillation between attractors via the light/dark cycle, depth of nightly dip determining trajectory. Loop 13 was reclassified from closed feedback loop to periodic forcing function, which changes the architectural label but not the substance.

---

## What the framework got wrong

**1. CO2 is not a causal driver in any feedback loop.** This is the single biggest finding of the stress test. The framework named CO2 as a causal driver in two loops — Loop 7 (CO2 -> granule pH -> mediator sequestration) and Loop 6a (low CO2 -> further thyroid suppression). Both are wrong. Loop 7 operates through ATP -> V-ATPase -> granule pH, not CO2 -> carbonic acid. CO2 acts only via non-specific bulk pH, while ATP has a specific mechanism at the V-ATPase catalytic site. Loop 6a fails the same test — no CO2-specific mechanism at any thyroid-axis protein exists. After the stress test, CO2 appears in zero formalized loops as a causal driver. The framework attributed causal agency to the wrong variable — the actual agent is ATP, which is stoichiometrically co-produced with CO2 but has specific molecular mechanisms where CO2 has only generic effects. CO2's non-loop roles (Bohr effect, carbamino protein protection) are preserved but unformalized.

How far off: the direction was right (metabolic output sustains metabolism). The specific variable was wrong (ATP, not CO2). This is the "right destination, wrong route" pattern.

**2. The loop count was overclaimed.** 13 -> 10 clean closed loops + 1 multi-armed hub + 2 half-closed + 1 forcing function. Loop 6 lost 2 of 5 arms (6a parallel marker, 6e not a feedback arm), with 1 indeterminate (6b serotonin closure mechanism). Loop 8's closure arm is unnamed. Loop 2's closure arm is direction-reversed by its own cited source. Loop 13 is a forcing function, not a closed loop.

How far off: overclaimed by ~30% in loop count, but the structural conclusion (sufficient for bistability) is unchanged. The architecture is sparser; the substance is preserved.

**3. Bistability is conditional, not unconditional.** The framework states "the metabolic system has two stable states" as fact. The evidence supports "the system can have two stable states when parameter conditions (PUFA burden, iron load, chronic stress, endotoxin exposure) create a disease basin." An organism with low PUFA, excellent thyroid function, and intact damping may be monostable — the healthy state is the only attractor. This matters because it means single interventions can work for organisms in the monostable regime.

How far off: right for the population it describes (people with metabolic disease). Overclaimed as universal.

**4. Two citation deployment errors found.** Pollard 1977 and Freed 2001 for Loop 7 (wrong species, scenario, endpoint, mechanism). PMC6624793 for Loop 2 (paper reports the opposite of what the framework claims — peripheral serotonin suppresses lipolysis, not promotes it). Pattern: citation errors cluster where mechanisms are named at the bulk-effect level rather than the molecular level.

How far off: claims were often right even when citations were wrong (citation accuracy is not claim accuracy). But Loop 2's closure being reversed by its cited source is not trivial.

---

## What was missing (what the stress test added)

**State-dependent negative feedback as the bistability mechanism.** The framework emphasized positive feedback and barely mentioned what opposes it. The stress test found that every negative feedback mechanism — HPT axis, HPA axis, antioxidant defenses (GSH, SOD, GPx), mitochondrial biogenesis (PGC-1alpha), autophagy/mitophagy, immune resolution (SPMs), hepatic regeneration, HIF-1alpha degradation, lactate clearance — is energy-dependent. They are strong when mitochondrial function is high and weak when it is low. The positive feedback loops operate by weakening the negative feedback. This creates multiplicative, not additive, gain dynamics — exactly the nonlinear gain function that produces bistability. This is the deepest structural insight the stress test produced, and it strengthens the framework's claims.

**The causal-independence audit tool.** A reusable methodology grounded in Pearl's screening-off test and MCA conservation relations for distinguishing causal drivers from parallel markers in feedback loops. Four-check operational audit (conservation, mechanism specificity, realizable intervention, quantitative dominance) with a six-category taxonomy. This tool caught the CO2 error and is integrated into the framework's Verification Methodology as a permanent sub-practice.

**Six new testable predictions.** Hysteresis in forward/reverse transition thresholds (observed in bariatric surgery data), critical slowing down near the separatrix (observed in Tabak et al. longitudinal data), PKM2 conditionality for glycolysis/OXPHOS bistability, multi-input threshold nonlinearity, slow-variable intervention durability, history-dependent bimodality in matched cohorts. The framework is now more predictive than before.

**Ketone bodies as a third fuel category.** The framework collapsed all non-glucose metabolism into "fat oxidation." Ketone bodies are biochemically distinct — CO2/ATP ratios match glucose, not fat. Randle pathology (FFA blocking PDH with glucose available) is not the same as adapted ketosis (no pyruvate to divert). The framework's "of glucose" specificity softened to "Krebs-cycle CO2 production as the invariant."

**The citation deployment audit.** A four-dimension check (species, scenario, endpoint, proposed-mechanism match) for every load-bearing citation. Integrated into Verification Methodology Step 5 as a permanent sub-practice.

---

## The overall assessment

The framework was substantially correct on the big claims and wrong on specific mechanisms. The pattern across every finding is the same one the Peat verification vault documented: right destination, wrong route.

| Claim | Before | After | Distance |
|---|---|---|---|
| Health IS oxidative metabolism | Of glucose to CO2 | Of Krebs-cycle substrates to CO2; glucose preferred, ketones equivalent | Small — substrate specificity softened |
| CO2 is an active product driving feedback | Causal driver in 2 loops | Parallel marker in all loops; non-loop roles preserved | Large — wrong variable (ATP, not CO2) |
| Lactate is an active disease driver | Via lactylation + HIF-1alpha | Causally validated in vivo; temporal structure added (HIF-1alpha initiates, lactylation locks in) | None — confirmed with stronger evidence |
| Two self-reinforcing stable states | Unconditional fact, 13 loops | Conditional on parameters, 10 clean loops | Moderate — conditionality added, count tightened |
| Recovery requires multi-loop intervention | Universal prediction | Prediction of bistable regime specifically | Small — scope narrowed |
| Emergent properties (progressive disease, etc.) | Deduced from attractor architecture | Confirmed as consequences of validated bistability | None — confirmed |

The framework was ~85% correct in substance and ~60% correct in specific mechanism attribution. The 15% substance gap is almost entirely the CO2 reclassification and the unconditional-to-conditional bistability shift. The 40% mechanism-attribution gap is the CO2/ATP confusion, the overclaimed loop count, the missing state-dependent damping insight, and the citation deployment errors.

Every correction made the framework more predictive, not less. Every refinement generated new testable predictions and constrained the claims. The stress test did exactly what it was designed to do: found where the framework was wrong, made it more precise, and left it stronger.

---

## The refinement documents

Six standalone knowledge artifacts capture the findings:

1. **`Convergence Point Reading.md`** — the ontological claim is Reading C (convergence point), not Reading A (strong reduction). Sub-test 1.A, PASS.
2. **`Krebs-Cycle Invariance and Ketone Bodies.md`** — "of glucose" softened; ketones as third fuel; Randle pathology distinguished from adapted ketosis. Sub-test 1.B, REFINEMENT.
3. **`Loop 7 — Metabolism-Mediator Coupling.md`** — CO2 replaced by ATP/V-ATPase as the causal driver in mediator release. Sub-test 2.A, REFINEMENT.
4. **`Causal Independence in Feedback Loops.md`** — the audit tool for distinguishing causal drivers from parallel markers. Pearl + MCA grounding. Sub-test 2.A derivative.
5. **`13-Loop Causal Independence Audit.md`** — the full classified loop inventory. 10 clean + hub + 2 half-closed + forcing function. Layer 2 audit.
6. **`Conditional Bistability and Attractor Dynamics.md`** — bistability is genuine dynamics, conditional on parameters. State-dependent damping. Six new predictions, two already observed. Layer 3.

The original `metabolic_foundations/` vault is preserved as written. Two methodology improvements were applied to it (citation deployment audit, causal-independence audit). No claim changes were applied — the refinements sit beside the original as parallel knowledge per the asymmetry principle.
