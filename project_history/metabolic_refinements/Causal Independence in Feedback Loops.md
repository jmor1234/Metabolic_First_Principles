---
title: "Causal Independence in Feedback Loops"
aliases:
  - Screening-Off Test for Feedback Loops
  - Causal Participant vs Parallel Marker
  - Structural Causal Independence Check
  - The Causal Independence Audit
status: proposed
last-updated: 2026-04-11
refines:
  - "The System.md"
  - "Foundation.md"
  - "The Metabolic Fork.md"
  - "Verification Methodology.md"
source: "Stress Test Sub-test 2.A (upstream observation); triangulation round 2026-04-11 (refinement of first-pass generalization)"
classification: refinement-substantial
triangulation: own-research+independent-agents
dependencies:
  - "Sub-test 2.A — Loop 7 refinement (upstream source of the observation)"
  - "Superseded first-pass generalization: the original Co-Production and Independence document (deleted)"
---

An audit tool for distinguishing *causal participants* from *parallel markers* among the metabolites named as drivers in the framework's positive feedback loops. The audit is a biochemical application of two established tools: **Pearl's do-calculus / screening-off test** from causal inference, and **conservation relations in stoichiometric network analysis** (Reder 1988; Heinrich & Schuster 1996; Palsson 2003). The operational question is whether a named metabolite can be varied independently of its stoichiometric partners through a realizable intervention, and whether it acts on the loop's downstream target through a mechanism distinct from any partner's mechanism.

This document is a rewrite of an earlier proposal (the original `Co-Production and Independence.md`, now deleted) that over-generalized from one case (Loop 7) into a universal "stoichiometric coupling → parallel marker" rule. Independent agent triangulation identified three problems with that first-pass generalization, all of which this rewrite addresses:

1. The concept is a partial re-derivation of established work in Metabolic Control Analysis and causal inference that should be cited directly rather than re-invented.
2. The universal "only if" form is falsified by at least two counterexamples: soluble adenylyl cyclase as a bicarbonate-specific regulator of OXPHOS, and AMP as an AMPK-specific signal despite adenylate-pool conservation.
3. The correct operational criterion is Pearl's screening-off test (with stoichiometric coupling serving as a diagnostic flag rather than a definition), and the three-category taxonomy should expand to include gated drivers and co-drivers.

The refinement preserves the Loop 7 finding that triggered the original insight and preserves the pre-specified CO₂/lactate asymmetry prediction. The generalization beyond Loop 7 is narrower, more rigorous, and grounded in existing formal machinery.

## Origin and the refinement of the refinement

The Loop 7 refinement in Sub-test 2.A surfaced a structural observation: CO₂ and ATP are stoichiometrically co-produced by OXPHOS at approximately fixed ratio (~6 CO₂ : ~30–32 ATP per glucose at completed oxidation). Therefore the framework's original Loop 7 mechanism — extracellular CO₂ → carbonic acid → granule pH → mediator release — could not have been closing a feedback loop through CO₂ specifically at the OXPHOS level, because any variation in CO₂ at OXPHOS output co-varies with ATP, and ATP has its own independent mechanism (V-ATPase) that accounts for the granule pH effect through a specific binding site.

A first-pass generalization of this observation was drafted: *a metabolite can act as an independent causal participant in a positive feedback loop only if its production is not stoichiometrically tied to the same upstream process the loop is supposed to influence.* That generalization was sent to two independent agents for stress-testing before being added to the Verification Methodology.

Both agents independently classified the first-pass principle as **Refinement**, identifying three critical problems addressed in the rewrite below.

### Problem 1 — The concept is not novel

The first-pass principle is a partial re-derivation of concepts established between 1973 and 2009. Specifically:

- **Conservation relations / moiety-conserved cycles in Metabolic Control Analysis.** Reder 1988; Heinrich & Schuster 1996 (*The Regulation of Cellular Systems*); Palsson 2003 on the left null space of the stoichiometric matrix. The left null space specifies exactly which linear combinations of concentrations are fixed by the reaction structure and cannot vary by flux alone. This is the rigorous mathematical formalization of "variables stoichiometrically coupled by the generating process."
- **Flux and concentration control coefficients in MCA.** Kacser & Burns 1973; Heinrich & Rapoport 1974; Fell's subsequent work. These quantify how much varying a specific enzyme or metabolite moves a flux or concentration at steady state. The concentration control coefficient of a parallel marker with respect to its own loop target is zero by construction; the control coefficient of a genuine driver is nonzero.
- **Pearl's do-calculus and screening-off test.** Pearl 2000 / 2009 *Causality*. The do-operator formalizes "intervene on X while holding everything else fixed." If X is stoichiometrically tied to Y, then do(X) is not a well-defined intervention without co-intervening on Y — X and Y are effectively one joint node in the causal graph. The screening-off test (d-separation under conditioning on a common cause) is the normatively correct test for distinguishing genuine causal participants from epiphenomenal markers.
- **Epiphenomenalism in philosophy of causation.** Jackson 1982; Kim 1993 on causal exclusion. The concept that a state can covary with causally efficacious states without itself being causally efficacious is the philosophical ancestor of the parallel-marker category.

The right methodological move is to **ground the audit in these existing frameworks** rather than propose it as a new primitive. The contribution is the specific *application* to the framework's feedback-loop architecture, not the underlying logic.

### Problem 2 — The universal form is falsified

**Counterexample A: Soluble adenylyl cyclase (sAC).** sAC is a cytoplasmic and intramitochondrial cyclase directly activated by bicarbonate via a specific allosteric site (Arg176; salt bridge disruption; active-site closure; metal recruitment — Chen et al. 2000; Litvin et al. 2003; Steegborn et al. 2005; Kleinboelting et al. 2014 crystal structures in *PNAS*). Acin-Perez et al. 2009 (*Cell Metabolism*) and Valsecchi et al. 2014 (*BBA*, PMC4257896) describe mitochondrial sAC phosphorylating Complex I NDUFS4 and Complex IV COX subunit IV-1 via PKA, enhancing OXPHOS activity. ATP is substrate, not allosteric activator. The pathway is carbonic-anhydrase-dependent and can be experimentally dissociated from ATP by CA inhibition.

The first-pass principle as stated would misclassify CO₂/bicarbonate in this pathway as a parallel marker of ATP. The biochemistry says CO₂/bicarbonate is an independent causal variable with a specific mechanism that ATP cannot substitute for.

**Important caveat verified against primary source (Valsecchi 2014):** The review frames the sAC pathway as **feedforward metabolic matching / gain control**, not as explicit closed positive feedback. The authors describe it as "coupling CO₂ generation in the Krebs cycle with the activity of the oxidative phosphorylation machinery" — substrate-supply-to-ATP-production matching. The paper does not document a self-amplifying bistable loop with CO₂ as causal participant.

This weakens the counterexample's directness: the framework does not currently formalize any feedback loop that corresponds to the sAC pathway, so the first-pass principle's misclassification is hypothetical rather than actualized within the framework. But the deeper point survives — the sAC pathway demonstrates that CO₂/bicarbonate *can* have a mechanism-specific causal effect on OXPHOS that is not reducible to ATP, which falsifies any universal claim that CO₂ cannot act independently when OXPHOS is the downstream target. The first-pass principle's universal form is wrong; the sAC biochemistry is the clearest demonstration that it is wrong.

**Counterexample B: AMP / AMPK.** AMP is in the conserved adenylate pool with ATP and ADP (the adenylate kinase equilibrium 2 ADP ⇌ ATP + AMP keeps the total approximately constant over short timescales). By strict stoichiometric reading, the first-pass principle would classify AMP as a parallel marker of ATP. But the AMPK γ-subunit CBS domains bind AMP specifically, and AMP activates AMPK in a way that ATP cannot (Gowans, Hawley, Ross, Hardie 2013 *Cell Metabolism*; Hardie 2012 *Nature Reviews Molecular Cell Biology*). The adenylate kinase equilibrium produces a ~quadratic amplification of AMP relative to ATP changes: a ~10% drop in ATP produces an ~8-fold rise in AMP, making AMP a more sensitive signal than ATP itself.

AMPK is the paradigmatic case of a stoichiometrically locked metabolite that is nonetheless the genuine causal participant, because the mechanism at the target is substrate-specific. The first-pass principle misclassifies this case; the refined audit below handles it correctly.

**Counterexample C (partial / gated): Proton gradient driving reverse electron transport.** The proton motive force is stoichiometrically coupled to NADH oxidation and ATP synthesis at F1F0 ATP synthase, but it has an independent causal role at Complex I via reverse electron transport when the CoQ pool is reduced (succinate-dominant substrates, LPS-activated macrophages). Mills et al. 2016 *Nature* on succinate/RET/IL-1β in inflammatory macrophages. Under uncoupling, proton gradient and ATP separate quantitatively while both remaining biologically active. The first-pass principle would miss this; the refined audit classifies it as a *gated driver* (parallel marker at baseline, independent driver when coupling breaks).

### Problem 3 — The correct operational criterion is Pearl's screening-off test

Both agents independently recommended replacing "stoichiometric coupling → parallel marker" with Pearl's screening-off / do-calculus as the operational test. The formal question is:

> **Can the metabolite be varied independently of any stoichiometrically co-produced partner through a physiologically realizable intervention, and does it act on the loop's downstream target through a specific molecular mechanism distinct from the partner's mechanism?**

This is mathematically rigorous, widely used in mature empirical sciences for exactly this kind of question, and correctly classifies all the cases where the first-pass principle fails.

## The refined audit

### The operational question

For each metabolite named as a causal driver in a positive feedback loop, the audit asks the question above. It decomposes into four sub-checks:

**1. Conservation check.** Is the metabolite a member of a conserved moiety pool in the strict MCA sense (left null space of the stoichiometric matrix — Reder 1988; Palsson 2003), or is it approximately stoichiometrically locked to another variable by a dominant shared generating process under the physiological regime the loop is claimed to operate in?

Conservation is a *diagnostic flag*, not a verdict. If conservation holds, proceed to the other checks. If conservation does not hold (the metabolite can vary freely), the metabolite likely passes the audit at this step.

**2. Mechanism specificity check.** Does the metabolite act on the loop's downstream target through a named molecular mechanism — a specific binding site, a specific enzyme substrate role, a specific covalent modification — that is not shared with its stoichiometric partner? Or does the claimed mechanism rely on a *non-specific* effect (bulk pH change, bulk osmolality, bulk thermal effect) that the partner would also produce?

Non-specific mechanism + stoichiometric coupling + a partner with a specific mechanism = **parallel marker**. This is the exact error in the original Loop 7 formulation.

Specific mechanism + stoichiometric coupling = **independent driver** (the coupling becomes a diagnostic flag that the analysis went back to check mechanism specificity; once specificity is confirmed, coupling does not disqualify).

**3. Realizable intervention check (Pearl's do-operator).** Is there a physiologically realizable experimental intervention that varies the metabolite while holding its partner fixed, or that produces differential effects dissociating the two? Examples: carbonic anhydrase inhibition dissociates bicarbonate from ATP at sAC; uncoupling protein activation dissociates CO₂ from ATP at the whole-cell level; compartmentalization dissociates cytosolic and mitochondrial pools of the same metabolite; non-linear amplification (as in adenylate kinase → AMP) makes a stoichiometrically locked metabolite quantitatively dissociable from its partner across physiological ranges.

If no such intervention is realizable at the physiological regime the loop is claimed to operate in, the case is an **indeterminate** — the distinction cannot be made with current tools and the audit defers.

**4. Quantitative dominance check.** At the concentrations, timescales, and tissue locations where the loop is claimed to operate, does the metabolite's effect magnitude exceed what its partner's effect magnitude would be? This handles cases where both metabolites affect the target via similar mechanisms but at different quantitative scales.

### Classification decision

If the metabolite passes the mechanism specificity check OR the realizable intervention check OR the quantitative dominance check, it is classified as an **independent driver**. If it fails all three (and conservation applies), it is classified as a **parallel marker**. If the relevant checks cannot be answered with current data, it is **indeterminate**.

### The expanded taxonomy

| Category | Meaning | Example |
|---|---|---|
| **Independent driver (specific mechanism)** | A named molecular mechanism binds the metabolite specifically; no partner has an equivalent effect at the same target. | ATP at V-ATPase; AMP at AMPK γ-subunit CBS domains; bicarbonate at sAC allosteric site; lactate at p300 via lactyl-CoA. |
| **Independent driver (quantitative dominance)** | The metabolite acts via a mechanism also accessible to its partners, but at a concentration or timescale where partners are negligible. | — (no clear framework example yet) |
| **Parallel marker** | The metabolite has no specific mechanism and its generic effect is dominated by a stoichiometric partner. The loop actually closes through the partner; the metabolite is a diagnostically useful but causally epiphenomenal readout. | CO₂ in the original Loop 7 formulation (bulk-pH mechanism, ATP at V-ATPase is the actual driver). |
| **Gated driver** | The metabolite is a parallel marker at baseline but becomes an independent driver when coupling to its partner breaks (threshold, compartmentalization, uncoupling, cofactor switch). | Proton gradient driving reverse electron transport / ROS signaling under UCP uncoupling or succinate-dominant conditions. |
| **Co-driver** | Both the metabolite and its partner are simultaneously independent causal participants via distinct mechanisms on the same target, with neither reducible to the other. | Ca²⁺ and IP3 in PLC-based oscillations. |
| **Indeterminate** | The relevant mechanistic question has not been characterized at the level the audit requires. Flag and defer. | Loop 6's "low CO₂ → low T3" arm (no specific mechanism identified; no clean experimental dissociation). |

Six categories rather than the original three. This handles the cases that would force a strict three-category taxonomy to misclassify real biology.

### Scope

The audit applies to **both positive and negative feedback loops.** The causal-independence question — whether a variable is a well-defined intervention target distinct from its stoichiometric partners — is structurally sign-independent. It asks about the variable's ontological status in the dynamical system, not about the direction of its effect.

In practice, the stakes are highest for **positive feedback loops**, because positive feedback can produce bistability or attractor-like dynamics in which the distinction between "driver" and "marker" determines whether the loop can actually close in the formal dynamical-systems sense. In negative feedback loops, a parallel marker is still useful regulatory information — demoting it to "not independently causal" is less consequential because the loop dampens rather than amplifies and the classification does not compound. But the audit's formal result is the same either way.

The audit applies at the level of **structural possibility**, not measurement strategy. A metabolite can fail the audit (classified as parallel marker) and still be the best practical diagnostic measurement available. For instance, ETCO₂ may fail a strict causal-participant audit in most OXPHOS-coupled contexts while remaining the cleanest non-invasive proxy for oxidative metabolic state. The audit concerns whether the metabolite is a causal participant in a formal feedback loop, not whether it is useful to measure.

### Relationship to existing frameworks

**Metabolic Control Analysis.** The conservation check is a qualitative application of Reder 1988 / Palsson 2003 formalism for conserved moieties. MCA's flux and concentration control coefficients are the quantitative tools for the mechanism-specificity and dominance checks. Where the framework's feedback-loop analysis becomes quantitative (Layer 3, loop gain calculations), MCA's control coefficients are the right formal machinery to reach for.

**Pearl's causal calculus.** The realizable intervention check is Pearl's do-operator applied to biochemical networks. The screening-off test (d-separation under conditioning on a common cause) is the normatively correct test for distinguishing genuine causal participants from epiphenomenal markers. Pearl 2009 *Causality* is the foundational reference.

**Structural identifiability in systems biology.** Villaverde / DiStefano / Walter. Two variables that are structurally non-identifiable from each other cannot be distinguished by any experiment and should not both appear as independent nodes in a causal model. The audit's parallel-marker category is a biological instance of structural non-identifiability.

**Epiphenomenalism.** The parallel-marker category is the biological instance of the philosophical epiphenomenon concept. The audit operationalizes it with a specific test.

The audit is not novel as a concept. It is the application of these established tools to a specific methodological problem: how to ensure the framework's positive feedback loops name real causal participants rather than parallel markers of hidden drivers. That application is useful and worth doing; it is not a new idea at the level of the underlying logic.

## Applied to the framework — sample classifications

The full 13-loop audit is a separate task (Step 3 of the current plan). Three sample classifications are worked out here to demonstrate the audit produces sensible results across structurally different cases and to lock in the Sub-test 2.A and pre-specified-prediction findings.

### Loop 7 (refined): ATP → V-ATPase → granule pH → mediator release

**Conservation check:** ATP is a member of the adenylate conserved pool, so conservation applies. Proceed to mechanism check.

**Mechanism specificity check:** V-ATPase has a specific binding site for ATP as its substrate — V-ATPase hydrolyzes ATP to pump protons across the granule membrane, and no stoichiometrically co-produced partner of ATP (CO₂, NADH, etc.) has any known role at the V-ATPase catalytic site. Poëa-Guyon et al. 2013 additionally shows the V₀ membrane domain is the intragranule pH sensor, with V₁-V₀ dissociation correlating with exocytosis readiness — the sensing operates on the granule lumen side and is coupled to the pumping function itself. The mechanism is ATP-specific.

**Realizable intervention check:** Bafilomycin A1 (specific V-ATPase inhibitor) dissociates V-ATPase activity from cellular ATP levels and produces the expected granule-pH and histamine-release effects (Nunomura et al. 2017). The intervention check passes.

**Quantitative dominance check:** Not needed; mechanism specificity is clear.

**Classification: Independent driver (specific mechanism).** The refined Loop 7 stands as a legitimate ATP-driven positive feedback loop.

### Loop 7 (original): CO₂ → bulk pH → granule pH → mediator release

**Conservation check:** CO₂ is stoichiometrically co-produced with ATP by OXPHOS at the mitochondrial level. Conservation applies.

**Mechanism specificity check:** The claimed mechanism is a bulk-pH effect on granule interior pH. This is a non-specific mechanism — any acid or base could in principle produce an equivalent bulk effect. ATP, via V-ATPase, produces a much larger and more kinetically specific effect on granule pH (~1.9-unit active gradient maintained against passive equilibrium). The original Loop 7 mechanism fails the specificity check — ATP via V-ATPase is the partner with the specific mechanism, and CO₂'s claimed effect is non-specific.

**Realizable intervention check:** Isocapnic voluntary hyperventilation (Barnes & Brown 1981) produces no plasma histamine change in humans, demonstrating that mechanical ventilation at constant CO₂ does not drive mediator release; 100% CO₂ (Strider et al. 2011) suppresses mast cell degranulation at supraphysiological dose via intracellular calcium rather than pH. No realizable intervention at physiological PaCO₂ ranges produces the effect the original mechanism predicts.

**Classification: Parallel marker.** This matches the Sub-test 2.A finding. The original Loop 7 CO₂ formulation is a parallel marker of the underlying ATP/V-ATPase mechanism; the refined Loop 7 correctly names ATP as the driver.

### Loop 6 (CO₂ arm): low T3 → low CO₂ → further low T3

**Conservation check:** CO₂ is stoichiometrically co-produced with ATP by OXPHOS. Conservation applies.

**Mechanism specificity check:** Is there a named molecular mechanism by which CO₂/bicarbonate specifically suppresses thyroid function (deiodinase activity, TRH/TSH release, tissue-level T3 signaling) distinct from the effect of the underlying metabolic rate? Candidates: pH-sensitive deiodinase activity (generic, not CO₂-specific); sAC-mediated PKA effects on thyroid-related proteins (speculative, not documented in this axis). No named protein with a specific CO₂ or bicarbonate binding site in the thyroid axis comparable to sAC in mitochondria has been identified in the literature available at the time of this audit.

**Realizable intervention check:** No human experiment has varied CO₂ while holding ATP/metabolic rate constant and measured tissue T3 signaling. The intervention that would resolve this has not been performed.

**Classification: Indeterminate, leaning parallel marker.** The "low CO₂ → further low T3" arm as currently stated rests on generic pH and metabolic-rate effects. In the absence of a specific mechanism, the arm is likely a re-narration of the underlying low-metabolic-rate feedback that ATP or metabolic rate more directly represents — structurally redundant with Loop 7's refined formulation rather than a distinct loop. This hypothesis (Loop 6's CO₂ arm being a Loop 7 re-narration) is flagged as **CF-CI.1** and should be confirmed or refuted during the full 13-loop audit.

### Loop 9: lactate → histone lactylation → glycolytic gene expression → more lactate

**Conservation check:** Lactate is NOT stoichiometrically co-produced with ATP by OXPHOS. Lactate is produced when pyruvate fails to enter the mitochondrion and is reduced by cytoplasmic LDH. Lactate is tied to the metabolic-fork *failure mode*, not to OXPHOS output. Under Warburg-shifted conditions, lactate rises while OXPHOS outputs fall — the two are negatively correlated, not stoichiometrically locked. Conservation does not apply in any way that would trigger the parallel-marker concern.

**Mechanism specificity check (conditional on Loop 9 mechanism verification):** Histone lactylation requires lactyl-CoA, generated specifically from lactate via AARS1 or p300 acyltransferase activity (Zhang et al. 2019 *Nature*; subsequent literature). The mechanism is lactate-specific. No stoichiometric partner of lactate has an equivalent role at p300.

**Realizable intervention check:** Pharmacological p300 inhibitors dissociate histone lactylation from lactate concentration; genetic manipulation of LDHA can alter lactate levels without changing total ATP production (within limits). The intervention check passes at the molecular level.

**Classification: Independent driver (specific mechanism), conditional on verification that histone lactylation is the actual mechanism of Loop 9's gene expression effects and not a correlate of HIF-1α or another master regulator.** The verification is the appropriate subject of Sub-test 2.B. The audit does not pre-empt 2.B; it establishes that lactate *passes the conservation and mechanism-specificity filters* that CO₂ failed for Loop 7, which is the structural asymmetry the pre-specified prediction identified.

### The CO₂/lactate asymmetry prediction survives triangulation

The pre-specified prediction from the first-pass generalization was: CO₂ and lactate will land in different audit categories because of their different structural relationships to OXPHOS — CO₂ stoichiometrically tied to OXPHOS output, lactate tied to OXPHOS failure mode. The refined audit confirms this prediction as applied to the framework's current loops. CO₂ is a parallel marker in Loop 7 as originally stated (confirmed); the refined Loop 7 is ATP-driven; lactate is an independent driver candidate in Loop 9 (conditional on mechanism verification). The asymmetry is not merely "lactate is different from CO₂" — it is the structural fact that lactate is *not* a member of a conserved moiety pool with OXPHOS outputs, whereas CO₂ is.

This is a real finding that survives the refinement of the first-pass principle.

## Structural consequences

### The audit should be methodologized, with proper attribution

The refined audit is useful enough to add to `metabolic_foundations/Verification Methodology.md` as a sub-practice under Step 4 (Identify what a resolution would depend on), since it asks whether a proposed causal relationship can in principle hold before moving to primary-source verification. The integration should cite Reder 1988, Heinrich & Schuster 1996, Palsson 2003, Kacser & Burns 1973, and Pearl 2009 as the formal machinery underlying the audit. It should **not** present the audit as a novel principle; it is an application of established tools to a specific methodological problem.

### Layer 3 prerequisite

Layer 3 of the stress test asks whether the 13-loop architecture exhibits formal bistability as a dynamical system. Formal bistability testing requires a clean loop inventory where each loop's named causal participants are legitimate independent drivers (or explicitly flagged gated/co-drivers with their coupling conditions specified), not parallel markers. The audit is the prerequisite — applied systematically across all 13 loops before Layer 3 can be run rigorously. The audit also provides the natural bridge to MCA quantitative tools (flux and concentration control coefficients, loop gain calculations) for the Layer 3 dynamical analysis.

### The CO₂-in-the-framework reframing

After Sub-test 2.A and the refined audit, CO₂'s role across the framework needs explicit reframing at both the loop level and the non-loop level:

- **In formalized loops (Loops 1–13):** CO₂ is a parallel marker in any loop where the feedback target involves OXPHOS output and the claimed mechanism is non-specific (bulk pH, bulk perfusion). The only loop where CO₂ was named as the causal driver was Loop 7, which has been refined to ATP-driven. Loop 6's CO₂ arm is likely the same case in different narration (CF-CI.1).
- **In non-loop protective mechanisms:** CO₂'s biological effects are real and not negated by the audit — Bohr effect on tissue O₂ delivery, carbamino protein protection, neuroprotection via NMDA modulation, possibly Bolevich & Kogan 2016 ROS suppression. These are direct physicochemical effects of CO₂/bicarbonate that reinforce the state producing them without closing a formal feedback loop in the dynamical-systems sense. They are real biology; they are just not loops.
- **In hypothetical sAC-based loops not currently in the framework:** CO₂/bicarbonate could in principle be an independent causal participant via a specific allosteric mechanism. The framework does not currently formalize such a loop, and the primary literature describes the sAC-OXPHOS pathway as feedforward metabolic matching rather than closed positive feedback (Valsecchi 2014 PMC4257896). Whether the framework should add a 14th formalized loop based on sAC is a separate question that depends on whether a subsequent experiment documents genuine bistability in the sAC pathway. Until then, sAC is a counterexample to the first-pass principle's universal form but not a concrete addition to the loop architecture.

The broader Foundation.md / The Metabolic Fork.md reframing of "CO₂ is an active product" — currently deferred pending CF-2.A.5 — should reflect both the negative finding (no formalized loop has CO₂ as causal driver under the refined audit) and the positive finding (CO₂'s biological effects are real at the non-loop level, and sAC shows at least one mechanism-specific pathway exists that is not reducible to ATP).

### The methodology has evolved twice from one sub-test

Sub-test 2.A produced two methodology improvements, both derived from the same underlying finding:

1. **CF-2.A.4 — Citation deployment audit** (already added to Verification Methodology Step 5). The two-for-two mis-deployment of Loop 7 citations led to a four-dimensional audit check (species / scenario / endpoint / proposed-mechanism match).
2. **The causal independence audit** (this document, pending integration at Step 2 of the current plan). The first-pass generalization was stress-tested and refined before being added to the methodology — the addition was deferred and improved rather than codified in wrong form.

Both improvements sharpen the testing apparatus itself, not just specific claims in the framework. The stress test is producing methodology improvements at a rate comparable to individual refinements, and the methodology improvements appear to have larger total leverage because they apply to every future verification rather than to one claim.

## Open questions

- **CF-CI.1 — Loop 6 CO₂ arm: re-narration of Loop 7 or independent loop?** Apply the audit during the full 13-loop pass. If Loop 6's CO₂ arm has no specific mechanism distinct from ATP/metabolic rate, it collapses into Loop 7 under a different description and the framework's formal loop count drops by one arm.

- **CF-CI.2 — sAC mitochondrial pathway: positive feedback or gain-control?** Valsecchi 2014 describes it as feedforward metabolic matching. If a subsequent experiment documents bistability or self-amplification specifically through the sAC pathway, the framework may add a 14th formalized loop with CO₂/bicarbonate as the first genuinely CO₂-driven loop. Until such a finding, the pathway is a counterexample to the first-pass principle's universal form but not a concrete addition to the architecture. Flag rather than chase.

- **CF-CI.3 — Quantitative MCA tooling for loop gain.** The framework's claim that 13 loops generate bistability through interlocking reinforcement (Core Claim 3) can be tested with quantitative loop gain calculations using MCA control coefficients. Address in Layer 3 with MCA methods.

- **CF-CI.4 — Structural identifiability check across the architecture.** Are there pairs of variables in the framework that are structurally non-identifiable from each other (indistinguishable under any realizable experiment)? A systematic structural-identifiability pass would catch cases the audit might miss. Address if Layer 3 or later stress-test work surfaces ambiguities.

- **CF-CI.5 — Methodology integration citation discipline.** When the audit is added to Verification Methodology, the integration should cite the existing frameworks (MCA, Pearl) rather than presenting the audit as a novel concept. Addressed in Step 2 of the current plan, now updated to reflect triangulation findings.

- **CF-CI.6 — Primary-source verification of sAC allosteric mechanism details.** The structural details cited here (Arg176, salt bridge disruption, active-site closure) are from secondary literature verification. If the audit becomes load-bearing for a specific framework change that involves sAC, a direct read of Kleinboelting et al. 2014 (PNAS) and the Steegborn et al. 2005 structural work would be warranted. Currently flagged but not pursued.

## Audit trail

- **Upstream source:** Sub-test 2.A — Loop 7 mechanism refinement (`Stress Test.md`, `Loop 7 — Metabolism-Mediator Coupling.md`). The structural observation that CO₂ and ATP are stoichiometrically co-produced was noted in passing in the Loop 7 refinement document and flagged as CF-2.A.1.

- **First-pass generalization (superseded):** The original `Co-Production and Independence.md`, written 2026-04-11 as an attempt to generalize the Sub-test 2.A observation into a universal structural principle. Independent agent triangulation identified three critical problems with that first-pass generalization (not novel, universally falsified, wrong operational criterion). The original document has been deleted and replaced by this rewrite.

- **Triangulation round (2026-04-11):** Two independent general-purpose agents were briefed with a self-contained research brief (`Research Brief - Co-Production Principle.md`, deleted as a one-shot artifact) and asked to stress-test the first-pass principle from first principles with no access to other project files. Both agents independently classified as **Refinement**, independently identified the concept as a re-derivation of MCA conservation relations and Pearl's screening-off test, and independently identified AMP/AMPK as a counterexample. Agent 1 additionally identified the sAC/bicarbonate/OXPHOS pathway as a counterexample specific to the CO₂ case. Agent 2 additionally observed that Loop 6's CO₂ arm may be a re-narration of Loop 7. Both proposed expanded taxonomies with a gated-driver category. Convergence was strong on all substantive findings. Agent reports (`agent_1_report.md`, `agent_2_report.md`) deleted as one-shot artifacts after synthesis.

- **Primary-source verification (2026-04-11):** The sAC counterexample was verified against primary sources via WebSearch / WebFetch. The Valsecchi 2014 review (PMC4257896) confirmed bicarbonate as the specific allosteric activator of sAC (not via ATP), the Complex I NDUFS4 and Complex IV COX-IV phosphorylation targets, and the carbonic-anhydrase dependence of the pathway. The review frames the pathway as feedforward metabolic matching rather than closed positive feedback, which narrows Agent 1's framing — the sAC pathway is a counterexample to any universal claim that CO₂ cannot act independently on OXPHOS-related processes, but it is not a documented closed positive feedback loop and therefore does not directly add a 14th loop to the architecture.

- **Current State.md:** Updated 2026-04-11 to reflect the rewrite, the triangulation outcome, and the methodology-integration sequencing change.
