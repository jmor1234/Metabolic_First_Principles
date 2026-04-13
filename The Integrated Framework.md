# The Integrated Framework

**What this document is:** The project's current best understanding of what health and disease are at the metabolic level — incorporating everything learned across the verification, extraction, and stress testing phases. This is the single document a reader should start with if they want the most accurate picture the project has produced.

**What this document is not:** It is not a replacement for the three source vaults. Each vault captures a different epistemic stance and remains the authoritative reference for its domain. This document synthesizes them.

**Traceability:** Every claim here traces to one or more source vaults:
- `peat_claims_verified/` — the original claim-by-claim verification against peer-reviewed research
- `metabolic_foundations/` — the pre-stress-test extraction as standalone biology (14 documents)
- `metabolic_refinements/` — the stress test findings, refinement documents, and audit trail

Where the stress test refined a claim, the refinement document is cited. Where the original holds unchanged, the foundations document is the reference. The reader can trace any claim to its evidence chain.

---

## The Thesis

At the deepest resolution currently available, health is efficient oxidative metabolism — glucose and other Krebs-cycle substrates fully oxidized through the mitochondria to CO2, producing abundant ATP. Disease is the progressive failure of that process: cells produce less ATP, generate more lactate, and lose the capacity to maintain themselves.

This is not "metabolism is one factor among many." Metabolism IS health at the cellular level. Every function a cell performs — maintaining membranes, repairing DNA, mounting immune responses, producing hormones, transmitting signals — requires ATP. When ATP production is adequate, these functions work. When it fails, they don't. What we call "disease" is what cellular energy failure looks like from different angles, in different tissues, at different stages.

The metabolic fork — the decision point where pyruvate either enters the mitochondria (producing CO2 and ~32 ATP) or stays in the cytoplasm (producing lactate and 2 ATP) — is the fundamental branching point. An 18-fold energy difference that determines whether a cell can maintain itself or must triage.

**What the stress test refined:** The original framework specified "of glucose" as essential. The stress test (Sub-test 1.B) demonstrated that ketone bodies are a biochemically distinct third fuel category with CO2/ATP ratios matching glucose — not inferior like raw fatty acid oxidation. The invariant is Krebs-cycle CO2 production, not the specific substrate. Glucose is preferred under normal conditions; ketone bodies are equivalent at the Krebs cycle; raw fatty acid beta-oxidation produces less CO2 per ATP and is the Randle-pathology pathway. Adapted ketosis (ketone bodies as fuel, no glucose available to divert) is biochemically distinct from Randle pathology (fatty acids blocking PDH while glucose IS available, forcing pyruvate to lactate). The original framework collapsed these two states under "fat oxidation."

*Traceability: `metabolic_foundations/Foundation.md` for the original thesis; `metabolic_refinements/Krebs-Cycle Invariance and Ketone Bodies.md` for the refinement.*

---

## The Architecture

The metabolic system has 6 essential state variables that define its condition at any moment:

| Variable | Timescale | Role |
|---|---|---|
| **Mitochondrial function (M)** | Days-weeks | The fundamental state — oxidative capacity, hardware quality |
| **Active thyroid hormone (T)** | Hours | The master throttle — sets the rate of M's maintenance and biogenesis |
| **Free estrogen (E)** | Hours-days | The glycolytic shift driver — reprograms cells away from oxidation via PI3K/AKT |
| **PUFA tissue content (P)** | Weeks-months | The hardware damage substrate — peroxidizes in mitochondrial membranes |
| **Endotoxin load (L)** | Hours | The gateway stressor — gut-derived LPS that activates every disease mediator |
| **Chronic lactate (Lambda)** | Hours-days | The epigenetic reprogramming driver — locks in the glycolytic shift via histone lactylation |

These variables interact through **10 clean closed positive feedback loops** plus a multi-armed hub, 2 half-closed loops, and a periodic forcing function. The loops organize into three canonical bistability motifs:

### Toggle switches (mutual inhibition)

Three pairs of variables mutually suppress each other. Each toggle can flip between two states — whichever variable is currently dominant suppresses the other, maintaining its own dominance.

**T and E (thyroid-estrogen toggle).** Adequate T3 supports hepatic glucuronidation that clears estrogen. Estrogen increases TBG that sequesters T3. When T3 is dominant, estrogen stays low; when estrogen is dominant, T3 stays suppressed. This is Loop 6c — the cleanest surviving arm of the framework's "Thyroid-Everything Loop."

**T and L (thyroid-endotoxin toggle).** Adequate T3 drives gut motility that prevents bacterial overgrowth. Endotoxin damages the liver where 70-90% of T4-to-T3 conversion occurs. When T3 is dominant, the gut is clean; when endotoxin is dominant, T3 conversion is impaired. This is Loop 12 — the framework's most cleanly intervention-tested loop (levothyroxine reduces SIBO risk; hypothyroidism produces ~10x SIBO prevalence).

**M and Lambda (metabolism-lactate toggle).** Adequate oxidative capacity clears lactate by oxidizing it. Chronic lactate drives histone lactylation that reprograms gene expression toward glycolytic enzymes and away from oxidative enzymes — producing more lactate. When M is dominant, lactate stays low; when lactate is dominant, M is epigenetically suppressed. This is Loop 9 — causally validated in vivo across 6+ disease models by site-specific mutant data, genetic knockouts, and pharmacological interventions.

*Traceability: `metabolic_foundations/The System.md` for the original 13-loop architecture; `metabolic_refinements/13-Loop Causal Independence Audit.md` for the classified inventory; `metabolic_refinements/Stress Test.md` Sub-test 2.B for lactylation causal validation.*

### Positive autoregulation (self-amplifying loops)

Four variables amplify their own production when elevated, creating lock-in once they reach sufficient levels.

**Estrogen (E -> E).** Estrogen upregulates aromatase (CYP19A1) in local tissues, producing more local estrogen independent of ovarian production. Tissue estrogen reaches 10-50x serum levels. The promoter switch from I.4 to I.3/PII is binary (switch-like), and CYP19A1 gene amplification occurs under aromatase inhibitor pressure — the genome itself resists suppression. Estrogen also triggers histamine release from mast cells, and histamine stimulates ovarian estradiol synthesis — a co-driver loop that adds to the autoregulatory gain. These are Loops 4 and 5.

**Lactate (Lambda -> Lambda).** Chronic lactate modifies histones via lactyl-CoA and p300, shifting gene expression toward glycolytic enzymes (LDHA, HK2, PKM2) that produce more lactate. The temporal structure matters: HIF-1alpha drives the acute gene expression response (hours, oxygen-reversible); lactylation consolidates it epigenetically (hours-days, persistent). Lactylation is the slow lock-in mechanism — the variable that creates history-dependence and hysteresis. This is Loop 9's self-amplifying arm.

**Endotoxin (L -> L).** LPS triggers iNOS in intestinal epithelial cells, producing NO that inhibits Complex IV, depleting the ATP that maintains tight junctions. The barrier becomes permeable. More endotoxin enters. The barrier is destroyed by the substance it exists to exclude. This is Loop 10.

**Mitochondrial function (M -> M).** Adequate ATP maintains V-ATPase activity in mast cell and platelet storage granules, keeping serotonin and histamine sequestered. When ATP falls, mediators are released and suppress oxidative metabolism further. This is the refined Loop 7 — the original framework attributed this to CO2/pH, but the stress test demonstrated the actual mechanism is ATP at the V-ATPase catalytic site (CO2 is a parallel marker of the same metabolic process, not the causal agent).

*Traceability: `metabolic_refinements/Loop 7 — Metabolism-Mediator Coupling.md` for the CO2 -> ATP refinement; `metabolic_foundations/The System.md` for the original loop descriptions.*

### Mutual positive feedback (co-amplification)

Three pairs of variables amplify each other when both are elevated.

**P and E (PUFA-estrogen co-amplification).** PUFA displaces estrogen from SHBG, increasing free estrogen. Estrogen upregulates desaturase enzymes, retaining and synthesizing more PUFA. Loop 3.

**L and E (endotoxin-estrogen co-amplification).** LPS inhibits hepatic glucuronidation, so estrogen accumulates. Estrogen reduces gut motility, allowing more bacterial overgrowth and endotoxin production. Loop 11.

**T and M (thyroid-metabolism mutual support).** T3 drives respiratory enzyme expression at both nuclear and mitochondrial genomes, building the hardware that produces ATP. Adequate mitochondrial function supports T3 production via hepatic T4-to-T3 conversion and cholesterol-to-pregnenolone conversion. Each sustains the other.

### The hardware damage chain

**PUFA peroxidation (P -> damage to M).** PUFA in mitochondrial cardiolipin is vulnerable to iron-catalyzed peroxidation (Fenton chemistry). The peroxidation chain propagates — each radical damages 3-10 more PUFA molecules in vitamin-E-depleted membranes. The damaged electron transport chain leaks electrons, generating more radicals. Three inputs sustain this: PUFA (the substrate, peroxidation susceptibility: oleic acid = 1, DHA = 320), iron (the catalyst), and vitamin E deficit (the absent chain-breaker). This is Loop 1.

### What was removed from the original architecture

**CO2 as causal driver.** The original framework named CO2 as an active product that drives feedback loops. The stress test's causal-independence audit (applying Pearl's screening-off test and MCA conservation relations) found that CO2 is stoichiometrically co-produced with ATP at OXPHOS and has no specific molecular mechanisms at any loop target — only non-specific bulk pH effects. ATP has specific mechanisms (V-ATPase catalytic site, tight junction maintenance, smooth muscle contraction) at every target where CO2 was claimed to act. CO2 is a parallel marker of oxidative metabolism, not a causal driver. Its non-loop roles (Bohr effect for oxygen delivery, carbamino protein protection) are real but not formalized as feedback loops.

**Three loop arms removed.** Loop 6a (CO2 -> thyroid suppression): parallel marker. Loop 6e (cholesterol -> thyroid suppression): not a closed feedback arm, just a downstream marker of impaired conversion. Loop 13 reclassified from closed loop to periodic forcing function (the day-night cycle that probes the system's recovery capacity nightly).

*Traceability: `metabolic_refinements/Causal Independence in Feedback Loops.md` for the audit methodology; `metabolic_refinements/13-Loop Causal Independence Audit.md` for the full classified inventory.*

---

## Why the System Is Bistable

The architecture produces two self-reinforcing stable states — genuine dynamical-systems bistability, not metaphor. This is the framework's most consequential structural claim, and the stress test confirmed it at four independent levels.

### The structural argument

The 6-variable interaction graph contains at least 10 independent positive circuits in 3 canonical bistability motifs. Thomas's necessary condition for bistability (at least one positive circuit) is satisfied with extreme redundancy.

The Gardner-Collins toggle switch conditions require both arms of a mutual inhibition pair to have Hill coefficients > 1 (cooperative/switch-like response). Several loops meet this: Loop 1 has state-dependent chain propagation (gain < 1 with vitamin E, gain > 1 without — the vitamin E / PUFA ratio is a bifurcation parameter). Loops 4+5 have binary promoter switching. Loop 10 has cascaded ultrasensitivity (NF-kB switch x ATP threshold). When multiple loops share state variables — and they do: free estrogen couples 4 loops, ATP couples 3, PUFA couples 3, LPS couples 3 — Brandman et al. 2005 (*Science*) showed that the effective cooperativity of the coupled system is approximately the product (for serial cascades) or sum (for convergent inputs) of the individual loops' ultrasensitivities. The system exceeds the bistability threshold collectively even if no single loop reaches it alone.

### The mathematical confirmation

Topp et al. 2000 (*J Theoretical Biology*) built an ODE model of beta-cell mass, insulin, and glucose dynamics and found a **saddle-node bifurcation**: as insulin resistance increases past a threshold, the healthy steady state disappears and the system transitions to a high-glucose state. Ha and Sherman extended this with more physiological detail and also found bistability and hysteresis. These researchers were modeling diabetes progression, not testing this framework — the confirmation is independent.

### The cellular confirmation

Mulukutla et al. 2014 (*PLOS ONE*) built a 12-metabolite ODE model of the glycolysis/OXPHOS decision with experimentally measured kinetic parameters. Two stable steady states with **experimentally validated hysteresis** — HeLa cells precultured in high glucose maintained glycolytic flux at intermediate glucose where cells precultured in low glucose stayed oxidative. Forward and reverse transition thresholds differ. This IS the metabolic fork operating as a real bistable switch.

### The whole-organism confirmation

**Bariatric surgery remission data shows hysteresis** — the one signature a monostable system cannot produce. Diabetes remission depends on disease duration, not just on the degree of metabolic improvement: shorter duration produces high remission rates; longer duration produces low rates; very long duration produces near-zero rates — even with equivalent weight loss and insulin sensitivity improvement. The forward transition (healthy -> diabetic) occurs at one insulin resistance level; the reverse transition requires harder correction. The asymmetry widens with time as beta-cell function (the slow variable) degrades. C-peptide is the strongest predictor: severely depleted beta-cell function predicts remission failure regardless of intervention. Early diabetes involves reversible beta-cell de-differentiation (genuine bistability); late diabetes involves irreversible cell death (a "point of no return" where the disease basin becomes inescapable).

**Longitudinal critical slowing down** (Tabak et al. 2009 *Lancet*, Whitehall II cohort, replicated across Ely, ARIC, Framingham, MESA): fasting glucose rises gradually for ~10 years, then accelerates sharply in the final ~3 years before diabetes diagnosis. The acceleration is specific to progressors — non-progressors show flat trajectories. This is the longitudinal fingerprint of a system approaching a tipping point.

### The conditionality

Bistability is not unconditional. An organism with low PUFA tissue burden, excellent thyroid function, and robust negative feedback may be monostable — the healthy state is the only attractor and perturbations always return to health. Bistability emerges when parameter conditions (PUFA burden, iron load, chronic stress, endotoxin exposure) shift enough to create a disease basin. This means single interventions CAN work for organisms in the monostable regime. The framework's prediction that "single interventions often fail" applies specifically to organisms in the bistable regime, where multiple reinforcing loops must be overcome simultaneously.

*Traceability: `metabolic_refinements/Conditional Bistability and Attractor Dynamics.md` for the full Layer 3 analysis, six predictions, and empirical confirmation.*

---

## The Deepest Structural Insight: State-Dependent Damping

The framework originally emphasized positive feedback and barely mentioned what opposes it. The stress test found that this omission hid the deepest mechanism.

Every negative feedback system in the organism — the HPT axis (thyroid homeostasis), the HPA axis (cortisol regulation), antioxidant defenses (GSH, SOD, GPx), mitochondrial biogenesis (PGC-1alpha), autophagy/mitophagy (PINK1/Parkin), immune resolution (resolvins, protectins), hepatic regeneration, lactate clearance — is **energy-dependent**. These systems require ATP to function. When mitochondrial function (M) is high, the damping systems are strong and perturbations are absorbed. When M is low, the damping systems fail — the organism lacks the energy to run its own defense mechanisms.

This means the positive feedback loops don't just oppose the negative feedback. They operate **by weakening it**. As the disease state deepens, the energy-dependent damping mechanisms lose power, which allows the positive feedback to strengthen further, which weakens the damping further. This is multiplicative, not additive — the effective gain of the positive feedback increases as the negative feedback it degrades falls away.

This is precisely the nonlinear gain function that produces bistability: strong damping at the healthy fixed point (stable), weak damping at the disease fixed point (also stable, because the positive feedback is now uncontested), and a threshold in between where the damping can no longer contain the positive feedback.

The negative feedback is not an opponent of bistability. It is a participant.

---

## The Two States

### The healthy attractor

M high, T high, E low, P low (or diet-controlled), L low, Lambda low. Each variable reinforces the others:

- High M -> adequate ATP -> V-ATPase sequesters mediators, tight junctions hold, antioxidants synthesized, mitochondria replaced
- High T -> respiratory enzymes expressed, estrogen cleared by liver, gut motility prevents SIBO
- Low E -> no glycolytic shift, progesterone opposition intact
- Low L -> barrier intact, liver functional, T4-to-T3 conversion operating
- Low Lambda -> no epigenetic reprogramming toward glycolysis
- Damping systems at full strength -> perturbations absorbed

### The disease attractor

M low, T low, E high, P high (accumulated), L high, Lambda high. Each variable worsens the others:

- Low M -> ATP deficit -> mediators released, barrier fails, antioxidants depleted, biogenesis suppressed
- Low T -> respiratory enzymes decline, estrogen accumulates (liver can't clear), gut slows (SIBO)
- High E -> PI3K/AKT glycolytic shift, estrogen-aromatase autoregulation engaged
- High L -> iNOS damages barrier further, liver overwhelmed, T3 conversion impaired
- High Lambda -> histone lactylation locks in glycolytic gene expression
- Damping systems energy-depleted -> positive feedback uncontested

### The threshold

The transition between states involves the slow variables (M, P) crossing through the parameter region where the bistable structure opens. The fast variables (T, L, Lambda, glucose dynamics) then snap to the corresponding attractor equilibrium. Clinically, this appears as gradual deterioration over years (the slow variables drifting) followed by sudden-appearing decline (the fast variables crossing their threshold) — exactly the pattern documented in the Tabak longitudinal data.

Recovery requires pushing the system back across the threshold, which means addressing multiple loops simultaneously — reducing PUFA burden (the hardware substrate), restoring thyroid function (the master throttle), opposing estrogen (the glycolytic driver), clearing endotoxin (the gateway stressor), and providing the energy substrate for the damping systems to re-engage. This is a structural requirement of the bistable architecture, not a philosophical preference for comprehensive treatment.

---

## The Temporal Dimension

Every 24 hours, the organism oscillates between the two states. Darkness activates the conservation program — melatonin, cortisol, free fatty acid mobilization, metabolic rate suppression — moving the system partially toward the disease attractor. Light reverses it each morning through two pathways: circadian entrainment (blue light -> SCN -> melatonin suppression) and mitochondrial activation (red/NIR light -> cytochrome c oxidase -> ATP production).

Health is not a fixed state. It is the capacity to enter the nightly conservation dip shallowly and exit it completely each morning. Disease is when the dip gets deeper, the reversal gets slower, and the system spends progressively more time in the disease attractor.

This daily oscillation is not one of the closed feedback loops — it was reclassified by the stress test as a periodic forcing function that probes the organism's recovery capacity. The forcing function's impact depends on which attractor the organism occupies: in the healthy state, the nightly dip is brief and fully reversed; in the disease state, each cycle leaves a residual deficit.

*Traceability: `metabolic_foundations/The Temporal Dimension.md` for the full circadian biology; `metabolic_refinements/13-Loop Causal Independence Audit.md` for the Loop 13 reclassification.*

---

## What This Predicts

The stress test generated six testable predictions from the formal bistability analysis. Two are already observed in existing clinical data.

**1. Hysteresis (OBSERVED).** Recovery from the disease state requires greater metabolic correction than what originally caused the transition. Bariatric surgery remission data confirms: diabetes remission depends on disease duration, with equivalent metabolic improvement producing different outcomes based on how long the slow variables have been in the disease basin.

**2. PKM2 conditionality (OPEN).** The glycolysis/OXPHOS bistable switch requires the PKM2 isoform (not PKM1). PKM2 is re-expressed under metabolic stress, making the bistable switch conditionally available — it emerges when the system is transitioning toward disease. PKM1-dominant tissues should show more reversible metabolic shifts.

**3. Critical slowing down (OBSERVED).** Recovery from standardized metabolic stressors slows as an organism approaches the threshold. Tabak et al. (Whitehall II, 5 replicating cohorts) show ~10-15-fold acceleration in glucose rise rate in the final 3 years before diabetes, specific to progressors. The OGTT disposition index shows the same nonlinear acceleration.

**4. Multi-input threshold nonlinearity (OPEN).** Addressing 1 loop should produce modest improvement; addressing 3+ simultaneously should produce disproportionate improvement as the system crosses the separatrix.

**5. Slow-variable intervention durability (OPEN).** Resetting slow variables (PUFA displacement over months, mitochondrial biogenesis via sustained exercise) should produce more durable recovery than resetting only fast variables (T3 supplementation alone).

**6. History-dependent bimodality (OPEN).** Populations with identical current inputs but different metabolic histories should show bimodal metabolic state distributions in the previously-stressed group.

---

## The Evidence That Already Exists

The research confirming this integrated picture is published across endocrinology, hepatology, oncology, neurology, cell biology, and immunology. No discipline has assembled the pieces. Five structural factors — disciplinary fragmentation, financial architecture (>$100B annually in industries dependent on the fragmented disease model), diagnostic infrastructure measuring proxies rather than mechanism, chemical conflation (synthetic progestins studied as "progesterone," conjugated equine estrogens as "estrogen"), and premature closure via meta-analysis — explain the gap.

The integration itself is the contribution. The evidence was always there. The stress test confirmed that the integration is structurally sound, empirically grounded, and more predictive than the fragmented alternative.

---

## Where to Go for Detail

**For the full mechanism biology:** `metabolic_foundations/` — 9 mechanism documents covering thyroid, glucose/Randle cycle, CO2/lactate, PUFA/iron/vitamin E, estrogen/progesterone, serotonin/histamine, endotoxin/liver, calcium, and circadian biology. Read these alongside the refinements that apply to them.

**For what changed and why:** `metabolic_refinements/Stress Test Summary.md` — precise before/after accounting. Each refinement document has an "Original Claim" section showing verbatim what the pre-stress-test framework said.

**For the original Peat verification:** `peat_claims_verified/` — the claim-by-claim audit trail showing how the knowledge was derived from its starting point.

**For assessment — "where is THIS person in the system?":** `The Assessment Protocol.md` (this directory) — maps a person onto the 6 state variables, estimates metabolic regime (monostable vs bistable), and outputs targeted intervention priorities. The bridge from this document to Practice.md.

**For practical application:** `metabolic_foundations/Practice.md` — interventions, monitoring framework, implementation sequence. Note: not yet updated with the conditional bistability finding. The Assessment Protocol incorporates these findings and provides the regime-dependent strategy that Practice.md lacks.
