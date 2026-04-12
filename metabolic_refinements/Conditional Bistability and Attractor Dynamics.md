---
title: "Conditional Bistability and Attractor Dynamics"
aliases:
  - Layer 3 Bistability Finding
  - Two Attractors Refinement
  - State-Dependent Damping
status: proposed
last-updated: 2026-04-12
refines:
  - "The System.md"
  - "Foundation.md"
source: "Stress Test Layer 3 — formal bistability analysis with independent agent triangulation"
classification: refinement-substantial
triangulation: own-research+independent-agents
dependencies:
  - "13-Loop Causal Independence Audit.md (the audited loop inventory Layer 3 operates on)"
  - "Loop 7 — Metabolism-Mediator Coupling.md (refined Loop 7 mechanism)"
  - "Sub-test 2.B (Loop 9 conditional resolved — lactylation causally validated)"
  - "CF-L3.1 through CF-L3.5 (open questions from Layer 3)"
---

The framework's claim that the metabolic system has "two self-reinforcing stable states" represents genuine dynamical-systems bistability, not metaphor. But the claim needs modification: bistability is *conditional* on the organism's parameter values falling within the bistable region of parameter space, not an unconditional property of every organism at every time. An organism with low PUFA tissue burden, excellent thyroid function, and robust negative feedback may be monostable — the healthy state is the only attractor and perturbations always return to health. Bistability emerges when parameters (PUFA burden, iron load, chronic stress, endotoxin exposure) shift enough to create a disease basin.

This refinement constrains the framework's strongest architectural claim and generates six new testable predictions. Core Claims 2 and 3 survive in modified form. The deepest structural finding is that the negative feedback mechanisms the framework under-emphasizes are not opponents of bistability — they *participate* in it, because they are themselves energy-dependent and weaken when the system needs them most.

Triangulated via two independent agents, both classifying REFINEMENT with matching reasoning chains.

## Original Claim

`The System.md` states:

> The metabolic system has two stable states. Each maintains itself through its own outputs. Once sufficiently established, each state persists — not because of a single cause, but because every output reinforces every other.

And:

> These cycles are not descriptions of what *might* happen. They are descriptions of what *does* happen when the system is sufficiently established in either state.

The framework presents bistability as an unconditional fact — the system HAS two stable states. It describes 13 interlocking positive feedback loops across 5 architectural layers as the mechanism producing this bistability. The emergent properties (progressive disease, single-intervention failure, context-dependence, threshold dynamics) are presented as deducible consequences of this attractor architecture.

`Foundation.md` states:

> These are not points on a spectrum. They are **attractors** — stable states that, once sufficiently established, maintain themselves through their own outputs.

"Attractor" is a rigorous concept in dynamical systems. Layer 3 tested whether this use is dynamics or metaphor.

## What Layer 3 Found

### The system formalization

The framework's 15 components reduce to 6 essential state variables based on dynamical independence and timescale:

| Variable | Symbol | Timescale | Role |
|---|---|---|---|
| Mitochondrial function | M | Days–weeks | The fundamental state — oxidative capacity |
| Active thyroid hormone | T | Hours | Master throttle for M |
| Free estrogen | E | Hours–days | Glycolytic shift driver |
| PUFA tissue content | P | Weeks–months | Hardware damage substrate |
| Endotoxin load | L | Hours | Gateway stressor |
| Chronic lactate | Λ | Hours–days | Epigenetic reprogramming driver |

The 10 audited clean loops (post-13-loop audit + Sub-test 2.B resolution) map onto signed interactions between these variables. The interaction graph contains **at least 10 independent positive circuits** in **3 canonical bistability motifs**:

- **Mutual inhibition (toggle switches):** T ⊣ E ⊣ T, T ⊣ L ⊣ T, M ⊣ Λ ⊣ M
- **Positive autoregulation:** E → E, Λ → Λ, L → L, M → M
- **Mutual positive feedback:** P ↔ E, L ↔ E, T ↔ M

### Structural conditions: abundantly satisfied

Thomas's necessary condition for bistability (1981) — a regulatory network must contain at least one positive circuit — is satisfied with extreme redundancy. The graph contains 10+ positive circuits across all three standard bistability motifs. This is structurally a *very strong* candidate. Thomas's condition is necessary but not sufficient — the quantitative question (are loop gains high enough?) is separate.

### Demonstrated sub-system bistability

The framework's sub-systems are not just structurally compatible with bistability — several are demonstrably bistable with experimental data:

**The glycolysis/OXPHOS switch is bistable.** Mulukutla et al. 2014 (*PLOS ONE*, PMC4049617) built a 12-metabolite ODE system with experimentally measured kinetic parameters modeling the glycolysis/OXPHOS decision. It produces two stable steady states with **experimentally validated hysteresis** — forward and reverse transition thresholds differ. This IS the framework's metabolic fork, operating as a real bistable switch at the cellular level. Key requirement: PKM2 (not PKM1), the isoform re-expressed under metabolic stress.

**ROS-induced ROS release is formally bistable.** Zorov et al. (2000, 2006) demonstrated that ROS from one mitochondrion trigger permeability transition in neighbors — a positive feedback with threshold behavior that maps onto Loop 1.

**Macrophage M1/M2 polarization shows experimental hysteresis.** Smith et al. showed that M1 pretreatment potentiates M2 response but M2 pretreatment blocks M1 response — classic bistable history-dependence. ODE models (Nickaeen et al.) show multistability via STAT1/STAT6 mutual inhibition.

**Important distinction:** HIF-1α oxygen sensing is ultrasensitive (steep dose-response) but NOT bistable — one steady state per oxygen level, no hysteresis (Qutub & Popel 2006-7). Ultrasensitivity is not bistability. The framework's Loop 9 depends on lactylation (confirmed causal in Sub-test 2.B), not on HIF-1α, for its bistability contribution.

### Collective bistability through coupled loops

Brandman et al. 2005 (*Science*) demonstrated that coupled positive feedback loops with individually insufficient nonlinearity produce bistability collectively. The effective Hill coefficient of the composite loop is approximately the **product** of the individual loops' ultrasensitivities for serial cascades, and the **sum** for convergent inputs at shared nodes.

The framework's architecture has exactly the coupling structure this principle requires. The Round 2 audit identified shared state variables: free estrogen couples 4 loops, cellular ATP couples 3 loops, PUFA couples 3 loops, LPS couples 3 loops. These shared variables create the mathematical coupling where individual loop contributions compound.

This means no single loop needs to independently achieve the bistability threshold. The coupled system exceeds it through composition. This is the formal mechanism behind the framework's intuitive claim that "thirteen interlocking loops compound."

### Quantitative loop gain evidence

At least 4 loops have strong quantitative evidence for bistability-compatible gain:

- **Loop 1 (PUFA-Peroxidation):** Chain propagation length 3-10 per initiating radical in depleted membranes; gain is state-dependent — < 1 with adequate vitamin E, > 1 when depleted. The vitamin E / PUFA ratio is a bifurcation parameter.
- **Loops 4+5 (Estrogen autoregulation):** 10-50× tissue amplification; binary promoter switch (I.4 → I.3/PII); CYP19A1 gene amplification under aromatase inhibitor pressure.
- **Loop 10 (LPS-Barrier):** Cascaded ultrasensitivity: NF-κB switch (n_eff 3-5) × ATP threshold for tight junctions (n_eff 2-3) = composite n_eff >> 2.
- **Loop 12 (Gut-Thyroid-Motility):** 54%/5% SIBO prevalence in hypothyroidism (Lauritano 2007); directional reversal by levothyroxine intervention.

### State-dependent negative feedback: the deepest finding

Every negative feedback mechanism identified — HPT axis, HPA axis, HIF-1α degradation, lactate clearance, antioxidant defenses, mitochondrial biogenesis (PGC-1α), autophagy/mitophagy, immune resolution (SPMs) — is **state-dependent**: strong in the healthy attractor, weak in the disease attractor.

The reason is structural: the negative feedback mechanisms are *themselves energy-dependent*. Antioxidant synthesis (GSH) requires ATP. Mitochondrial biogenesis (PGC-1α) is suppressed by NF-κB under inflammation. Immune resolution (SPMs) requires PUFA substrate that peroxidation diverts. Hepatic regeneration is consumed by simultaneous insults. When M is low, the organism lacks the energy to run its own damping systems.

**This is the deepest structural insight of Layer 3:** the positive feedback loops operate *by weakening* the negative feedback. This is not additive opposition (positive gain minus negative gain). It is multiplicative: the positive feedback gain increases as it weakens the negative feedback, creating exactly the nonlinear gain function that produces bistability. The negative feedback is strong at the healthy fixed point (eigenvalues negative → stable) and weak at the disease fixed point (positive feedback dominates → also stable). The threshold between them is where the damping can no longer contain the positive feedback.

### Timescale separation and slow-fast bistability

The state variables span 4 orders of magnitude in timescale: ATP turns over in seconds, T₃ and LPS in hours, estrogen and lactate in hours-days, mitochondrial function in days-weeks, PUFA tissue content in weeks-months.

This timescale separation creates **slow-fast bistability**: the fast variables (T, L, Λ) equilibrate to quasi-steady states determined by the slow variables (M, E, P), which then drift in the direction dictated by the fast system's state. This produces hysteresis on the slow timescale — exactly matching the framework's description of progressive disease onset (slow PUFA accumulation, slow mitochondrial degradation) followed by sudden-appearing transition (the slow variables cross the threshold and the fast variables snap to the disease equilibrium).

## Refined Claim

The system can exhibit two self-reinforcing stable states when parameter conditions — PUFA tissue burden, iron load, chronic stress, endotoxin exposure — place the system in the bistable region of its parameter space. An organism with low PUFA, excellent thyroid function, and robust energy-dependent negative feedback may be monostable: the healthy state is the only attractor, and perturbations return to health.

Bistability emerges when parameters shift enough to create a disease basin. The positive feedback loops weaken the energy-dependent negative feedback as the system moves toward disease, creating the nonlinear gain transition that opens a second basin. Once the disease attractor exists and the system enters it, the same state-dependent damping makes the disease state self-sustaining — the weakened negative feedback cannot pull the system back across the threshold.

Recovery requires sufficient perturbation across multiple loops simultaneously to overcome the disease attractor's reinforcement — this is the framework's existing Core Claim 4, and it follows from the conditional bistability exactly as stated.

The "two attractors" framing is dynamics, not metaphor. But it is conditional dynamics, not unconditional fact.

## Structural Consequences

### Core Claims modified

- **Core Claim 2** ("The system has two self-reinforcing stable states"): survives as "The system *can exhibit* two self-reinforcing stable states when parameter conditions create a disease basin."
- **Core Claim 3** ("Positive feedback loops make each state self-maintaining"): survives intact — the mechanism is confirmed.
- **Core Claim 4** ("Recovery requires addressing multiple loops simultaneously"): survives as a deducible consequence of the conditional bistability.

### Loop inventory updated

The framework's nominal 13 loops contract to 10 clean closed PFB loops + 1 multi-armed hub (Loop 6: 1 clean arm, 1 gated, 1 indeterminate) + 2 half-closed loops (L2, L8) + 1 periodic forcing function (L13). The substance is preserved; the architectural precision is substantially increased. See `13-Loop Causal Independence Audit.md` for the full classified inventory.

### The framework's emergent properties are confirmed as consequences

All five emergent properties listed in `The System.md` — progressive disease, single-intervention failure, context-dependence, multi-input recovery requirement, threshold dynamics — are deducible consequences of conditional bistability and follow from the refined claim exactly as stated. The refinement adds *why* each property holds at the dynamical-systems level (eigenvalue structure at fixed points, Brandman coupling, slow-fast hysteresis, state-dependent damping).

### The monostable-excitable alternative

The strongest counter-argument to bistability is monostable-excitable dynamics: the system has one attractor (health) and disease is a sustained-input-driven excursion. This is clinically indistinguishable from bistability for individual patients, because the slow variables (PUFA weeks-months, mitochondrial function days-weeks) create apparent hysteresis even in a monostable system. Both mechanisms may operate simultaneously in different organisms or at different disease stages.

The distinguishing test is **hysteresis** — different forward and reverse transition thresholds. See the empirical confirmation section below: bariatric surgery remission data provides this test.

### Empirical confirmation: existing data that tests the predictions

After the structural analysis and triangulation, a targeted check against existing clinical data revealed that several of the predictions are already observable in published evidence. These findings are from well-replicated clinical literature; the directional patterns are robust across multiple independent cohorts. **Specific numbers cited below are from agent training knowledge and require primary-source verification before becoming load-bearing** — the stress test has previously caught agents fabricating specific figures (Mathur "0.33×," PMC4056127 percentages). The directional findings are confident; specific percentages and fold-changes carry a verification flag.

**Longitudinal critical slowing down (Tabák et al. 2009, *Lancet*; Whitehall II cohort).** 6,538 participants tracked over 13 years, 505 of whom developed diabetes. Progressors showed fasting glucose rising gradually for ~10 years, then accelerating sharply in the final ~3 years before diagnosis — an approximately 10-15-fold increase in the rate of glucose rise [specific fold-change requires primary-source verification]. Non-progressors showed flat trajectories over the same period. The acceleration is specific to progressors — the trajectory *shape* diverges, not just the level. Replicated independently in the Ely study, ARIC, Framingham Offspring, and MESA cohorts. This is the longitudinal CSD fingerprint: gradual drift followed by accelerating departure as the system approaches the tipping point.

**Whole-organism hysteresis via bariatric surgery remission data.** Hysteresis — different forward and reverse transition thresholds — is the one signature a monostable system cannot produce. The bariatric surgery literature consistently shows that diabetes remission depends on disease *duration*, not just on the degree of metabolic improvement:

- Shorter duration (<5 years): high remission rates
- Longer duration (>10 years): low remission rates
- Very long duration (>15 years on insulin): remission essentially impossible

[Specific percentages per duration category require primary-source verification.] The pattern is one of the most replicated findings in bariatric surgery research (Schauer STAMPEDE 5-year data *NEJM* 2017; DiaRem score; multiple cohorts). The DiRECT trial (Lean et al. 2018 *Lancet*) confirmed: patients with shorter duration remitted at higher rates than longer duration despite equivalent weight loss.

**The slow variable is identified: beta-cell function.** C-peptide (a direct marker of beta-cell insulin secretion) is the strongest single biochemical predictor of remission across multiple bariatric cohorts. Low baseline C-peptide predicts near-zero remission probability regardless of intervention intensity. This is the slow variable that determines which basin the system occupies — patients with preserved beta-cell function can cross back to the healthy attractor; patients with severely depleted function cannot.

**The mechanism is bistability, not just irreversible damage — with an important distinction.** The duration-dependence could reflect either (a) bistability (beta cells are dysfunctional but alive — de-differentiated, potentially re-differentiable) or (b) irreversible damage (beta cells are dead). Recent evidence (Taylor's twin cycle hypothesis; DiRECT trial showing beta-cell function restoration with pancreatic fat removal) supports **both mechanisms operating at different timescales**: early-to-moderate diabetes involves beta-cell de-differentiation (a reversible state change — genuine bistability), while late diabetes involves progressive cell death (irreversible damage — a "point of no return" where the disease basin becomes inescapable). The approximately 10-15 year duration boundary [verification needed] where remission rates approach zero may mark the transition from reversible de-differentiation to irreversible destruction.

**Relapse correlates with prior duration** — among patients who achieve remission, those with longer pre-surgical diabetes duration relapse at higher rates. The disease state has "memory" through the slow variable. This is the hysteresis signature: the stability of the recovered state depends on how much slow-variable damage accumulated during the disease period.

**What this means for the bistability claim:** The bariatric surgery data is the whole-organism hysteresis measurement that CF-L3.1 identified as the most valuable test. It was not performed as a bifurcation experiment, but it functions as one: the forward transition (healthy → diabetic) occurs at one insulin resistance level; the reverse transition requires harder correction; and the asymmetry widens as the slow variable degrades. Combined with the Tabák longitudinal acceleration and the Topp et al. saddle-node bifurcation model, the glucose-insulin subsystem has structural, mathematical, and empirical evidence for genuine bistability. The generalization to the full 6-variable metabolic system remains structural inference — the other toggle switches (T-E, T-L) have not been independently tested for hysteresis — but the core metabolic fork (the M-Λ axis, the glucose-insulin dynamics) is empirically grounded.

## New Testable Predictions

Six predictions generated by the formal bistability analysis. Each constrains the framework and is falsifiable.

**1. Hysteresis in forward/reverse transition thresholds.** The correction required to escape the disease basin is greater than the perturbation that entered it, because the disease attractor has its own reinforcing loops. Recovery requires more correction than disease induction. **STATUS: OBSERVED.** Bariatric surgery remission data shows duration-dependent asymmetry between forward and reverse transitions. See empirical confirmation section above. The T-E and T-L toggle switches have not been independently tested for hysteresis — this remains open for non-glucose-insulin subsystems.

**2. PKM2 conditionality.** The glycolysis/OXPHOS bistable switch (Mulukutla 2014) requires PKM2, the embryonic/cancer isoform re-expressed under metabolic stress via HIF-1α and NF-κB. Prediction: PKM1-dominant tissues should show more reversible metabolic shifts. The bistable switch is conditionally available — it emerges precisely when the system is transitioning toward disease. Falsifiable by comparing metabolic reversibility in PKM1- vs PKM2-expressing tissues.

**3. Critical slowing down near the separatrix.** A universal early warning signal for bistability transitions: recovery time from standardized stressors (glucose tolerance test, temperature recovery after cold exposure) should increase as an organism approaches the threshold between attractors. **STATUS: OBSERVED.** Tabák et al. (Whitehall II) showed ~10-15-fold acceleration in glucose rise rate in the final 3 years before diagnosis, specific to progressors, replicated across 5 cohorts. OGTT disposition index shows nonlinear acceleration (the DI hyperbola). Remaining test: whether temperature recovery, HRV, and other non-glucose perturbation recoveries show the same pattern.

**4. Multi-input threshold nonlinearity.** Addressing 1 loop should produce modest improvement. Addressing 3+ loops simultaneously should produce disproportionately large improvement — the system crosses the separatrix. Testable in clinical intervention design by comparing single-intervention vs. multi-intervention recovery trajectories.

**5. Slow-variable intervention durability.** Interventions resetting slow variables (PUFA tissue displacement via dietary change over months, mitochondrial biogenesis via sustained exercise) should show more durable recovery than fast-variable-only interventions (T₃ supplementation alone, acute anti-inflammatory). Testable by comparing relapse rates after different intervention types.

**6. History-dependent bimodality in matched cohorts.** Among a population with identical current environmental inputs but different metabolic histories, the previously-metabolically-stressed group should show a bimodal distribution of metabolic state variables while the never-stressed group should be unimodal. This tests history-dependence — the hallmark of bistability.

## Open Questions

**CF-L3.1 — Whole-organism hysteresis measurement. STATUS: PARTIALLY RESOLVED.** Bariatric surgery remission data provides whole-organism hysteresis evidence for the glucose-insulin subsystem specifically: duration-dependent remission rates, C-peptide as the slow-variable predictor, relapse-duration correlation. **Remaining:** (a) primary-source verification of the specific numbers cited from agent training knowledge; (b) hysteresis testing for non-glucose-insulin subsystems (T-E toggle, T-L toggle); (c) the controlled bifurcation-parameter-sweep protocol (T₃ titration in both directions) has not been performed.

**CF-L3.2 — PKM2 conditionality.** Whether PKM1-dominant tissues show more reversible metabolic shifts. Requires clinical data on PKM isoform expression across the health-disease spectrum. OPEN.

**CF-L3.3 — Critical slowing down. STATUS: PARTIALLY RESOLVED.** Tabák et al. (Whitehall II) and 4 replicating cohorts show longitudinal acceleration specific to progressors in the glucose-insulin subsystem. OGTT disposition index shows nonlinear acceleration. **Remaining:** (a) primary-source verification of specific fold-changes; (b) whether the pattern extends to non-glucose perturbation recoveries (temperature, HRV, exercise); (c) whether the acceleration is distinguishable from a monostable threshold effect (the hysteresis data from CF-L3.1 addresses this for the glucose-insulin case).

**CF-L3.4 — Integrated ODE model.** No 6-variable model with computed bifurcation diagram exists. A minimal 3-variable model (M-T-E core) would be the tractable first step. The kinetic data to parameterize exists scattered across the sub-system literature. This is a computational project.

**CF-L3.5 — Parameter-region boundaries.** What specific parameter values (PUFA tissue %, iron stores, chronic cortisol, endotoxin exposure) place an organism in the bistable vs. monostable region? This is the quantitative question the conditional bistability refinement opens. Currently unknown.

**CF-2.B.3 — Lactylation persistence.** The critical experiment for confirming lactylation as a bistable lock-in mechanism — remove lactate, track mark persistence — has not been published. The half-life of histone lactylation marks is unknown.

## Audit Trail

**Source:** Stress Test Layer 3 — formal bistability analysis (2026-04-12). Six phases: system formalization, published bistability model survey, quantitative loop gain estimation, multi-loop coupling analysis, negative feedback inventory, classification.

**Triangulation:** Two independent general-purpose agents dispatched per `Independent Agent Research Protocol.md`, each given `Research Brief - Layer 3 Bistability.md` (deleted after synthesis — git history preserves). Both agents independently classified REFINEMENT with matching reasoning. Strong convergence on: Thomas's condition abundantly satisfied, Mulukutla 2014 as strongest finding, Brandman coupling as key answer to "no single loop has measured gain > 1", state-dependent damping as genuine. Agent additions adopted: critical slowing down prediction (Agent 2), timescale-induced hysteresis as complementary mechanism (Agent 1), PKM2 conditionality (both), Brandman serial vs convergent distinction (Agent 2, correcting context-holder's Phase 4), autophagy/mitophagy as missed damping mechanism (both).

**Empirical confirmation check (2026-04-12, post-triangulation):** Targeted search against existing clinical data for CSD signatures and hysteresis evidence. Three findings: (1) Tabák et al. 2009 *Lancet* (Whitehall II) shows longitudinal CSD acceleration specific to progressors, replicated across 5 cohorts; (2) bariatric surgery remission literature shows whole-organism hysteresis via duration-dependent remission rates with C-peptide as the slow variable; (3) Topp et al. 2000 *J Theor Biol* shows saddle-node bifurcation in glucose-insulin ODE model. CF-L3.1 and CF-L3.3 partially resolved. Specific numbers from agent training knowledge flagged for primary-source verification.

**Key references:** Thomas 1981 (necessary conditions); Gardner et al. 2000 *Nature* (toggle switch); Brandman et al. 2005 *Science* (coupled loop bistability); Mulukutla et al. 2014 *PLOS ONE* PMC4049617 (glycolysis/OXPHOS bistability with hysteresis); Ferrell 2002, 2008 (ultrasensitivity and cascaded bistability); Zorov et al. 2000, 2006 (ROS-induced ROS release); Qutub & Popel 2006-7 (HIF-1α ultrasensitivity, NOT bistability); Cherry & Adler 2000 (asymmetric cooperativity); Tyson et al. 2003 (bifurcation analysis); Angeli et al. 2004 (monotone systems); Topp et al. 2000 *J Theor Biol* (glucose-insulin saddle-node bifurcation); Tabák et al. 2009 *Lancet* (longitudinal glucose trajectories before diabetes); Schauer et al. 2017 *NEJM* (STAMPEDE bariatric surgery duration-dependence); Lean et al. 2018 *Lancet* (DiRECT trial duration-dependent remission).

**Depends on:** `13-Loop Causal Independence Audit.md` (the audited loop inventory); `Loop 7 — Metabolism-Mediator Coupling.md` (refined Loop 7); Sub-test 2.B (Loop 9 conditional resolved, documented in `Stress Test.md`).

**Working log:** `Stress Test.md` → 2026-04-12 entries (Layer 3 analysis + Sub-test 2.B).

**Diff catalog:** The precise text-level changes this refinement would apply to `The System.md` and `Foundation.md` if the asymmetry principle were not in effect are documented in `Refinement Diff Catalog.md` (to be updated with the Layer 3-specific diffs).
