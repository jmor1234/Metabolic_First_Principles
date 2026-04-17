---
priority: P3
claim: "State-dependent damping as cross-system unifier of negative feedback collapse"
scope: "Peripheral in strict Core-Claims sense; supports Core Claims 2 and 4; framework's distinctive structural contribution"
status: complete
verdict: refinement
confidence-change: increased overall (direction confirmed, specific ATP attribution narrowed to multi-currency framing)
started: 2026-04-17
completed: 2026-04-17
gaps-remaining:
  - "L8 (multiplicative coupling) — requires ODE modeling (CF-L3.4)"
  - "Cross-system kinetic correlation measurements under intervention — literature search not performed"
  - "Primary-source verification of NAD+ vs ATP depletion magnitude and NR/NMN dissociation effects"
vault-sources:
  - "metabolic_framework/The System.md — State-dependent negative feedback section"
  - "metabolic_framework/Foundation.md — Self-reinforcing states section"
  - "metabolic_framework/Practice.md — State-dependent damping: why restoring M is the universal priority"
  - "project_history/metabolic_refinements/Conditional Bistability and Attractor Dynamics.md — deepest treatment"
---

# P3 — State-Dependent Damping as Cross-System Unifier

## Phase 1 — Define the Target

### 1.1 Restatement of the Claim

**Crispest form.** The organism's named negative feedback systems share ATP-dependent machinery; they therefore fail together under a shared coupling currency (ATP) as mitochondrial function falls, producing cross-system correlated damping collapse that is distinctive to this framework.

**Full form (preserving the vault's hedges).** The organism's named negative feedback systems — HPT axis, HPA axis, HIF-1α degradation, lactate clearance, antioxidant defenses (GSH, SOD, GPx), mitochondrial biogenesis (PGC-1α), autophagy/mitophagy (PINK1/Parkin), immune resolution (specialized pro-resolving mediators), and hepatic regeneration — all depend on ATP for the *maintenance of their machinery* (enzyme and receptor synthesis, folding, trafficking, cofactor regeneration), even when the regulatory act itself is thermodynamically free (allosteric inhibition, product inhibition). Because they share this dependence, they weaken *together* under a single coupling currency (ATP) as mitochondrial function falls, rather than failing independently. The coupling is **multiplicative**: positive feedback effective gain increases as damping falls away, not as positive feedback strengthens — producing the nonlinear gain structure characteristic of bistable transitions. This cross-system unification, **not** bistability itself, is the framework's distinctive structural contribution; the vault explicitly names ultrasensitivity, mutual inhibition, and saturation of positive feedback as alternative bistability mechanisms that operate within specific subsystems.

**Two-layer structure of the claim (important for targeting the stress test):**

- **Layer A — Individual system ATP-dependence.** Each of the nine named damping systems has ATP-dependent machinery maintenance. This layer is mostly textbook per system.
- **Layer B — Cross-system unification.** The systems fail *together* under shared ATP currency, producing correlated damping collapse and multiplicative gain structure. This layer is the synthesis inference and the actual target of the stress test.

Attacks on Layer A are useful only insofar as they reveal which systems have ATP as definitively rate-limiting vs. which don't. Attacks on Layer B are the core of P3.

### 1.2 Relationship to Core Claims

The vault pre-specifies five Core Claims in [[metabolic_framework/Verification Methodology]]. State-dependent damping as cross-system unifier is **not itself a Core Claim**. The vault explicitly states:

> "State-dependent damping is one of several mechanisms generating bistability in this architecture, alongside ultrasensitivity, mutual inhibition, and saturation of positive feedback — all of which operate within specific subsystems. What makes it distinctive is cross-system unification." *(The System.md)*

Relationship to each Core Claim:

| Core Claim | Relationship to P3 |
|---|---|
| 1. Health = efficient oxidative metabolism; disease = its failure | Independent; P3 does not implicate Core Claim 1 |
| 2. Bistability conditional on parameters | P3 provides **one** mechanism for bistability (alongside ultrasensitivity, mutual inhibition, saturation) |
| 3. Positive feedback loops make each state self-maintaining | Independent; positive feedback self-maintains regardless of the damping mechanism |
| 4. Recovery requires multi-loop intervention | P3 provides **one** rationale (brakes are degraded); but the prescription also follows from having many reinforcing loops |
| 5. Daily oscillation | Independent |

**If P3 collapses:**
- Core Claim 2 **survives** (other bistability mechanisms remain — ultrasensitivity, mutual inhibition, saturation of positive feedback; these are already present in the architecture and operate within specific subsystems like glycolysis/OXPHOS per Mulukutla 2014)
- Core Claim 3 **survives** (positive feedback mechanism is independent)
- Core Claim 4 **survives** as prescription (multi-loop intervention still needed because many loops reinforce the disease state) but **loses one of its justifications** (the "brakes are degraded" story)
- The framework's **distinctive contribution** weakens: no cross-system unifier for feedback failure; subsystems fail independently rather than together under a shared currency.

**Classification: Refinement, not Fail.** The framework's core architecture survives; the unification claim is demoted to subsystem-specific mechanisms. This matches the Pass/Refinement/Fail criterion: modification that narrows what the framework claims (from cross-system unification to subsystem mechanisms) is a Refinement by the decisive test of specificity.

### 1.3 Prediction Chain (Link by Link)

The claim decomposes into ten links. Each link's status is marked (textbook / well-supported / contested / inferred). Attack effort targets contested and inferred links.

| # | Link | Status | Notes |
|---|---|---|---|
| L1 | Every cellular function requires ATP | **Textbook** | No dispute |
| L2 | Negative feedback systems have machinery (enzymes, receptors, cofactors) that must be synthesized, folded, trafficked, regenerated | **Textbook** | No dispute |
| L3 | This maintenance is ATP-dependent (protein synthesis, folding, trafficking, cofactor regeneration all cost ATP) | **Textbook** | No dispute |
| L4 | Each of the nine named damping systems has ATP-dependent machinery | **Well-supported individually** | Each system is textbook in its own literature; aggregate claim rests on per-system confirmation |
| L5 | ATP availability is rate-limiting for this machinery under disease-state conditions (not just under experimental starvation) | **Contested** | Each system has multiple inputs; which input is rate-limiting under specific conditions is empirical and may vary across systems |
| L6 | These systems fail on correlated timescales when ATP falls (not on independent timescales that only appear correlated in long-run chronic-disease observation) | **Inferred** | Timescales may differ: HPT hours-days, autophagy hours-days, mitochondrial biogenesis weeks, hepatic regeneration months-years |
| L7 | The shared currency is ATP specifically, not a deeper variable (NADPH, NAD+/NADH, redox state, membrane potential, substrate supply) | **Inferred** | This is sub-question 3d; Causal Independence Audit applies directly |
| L8 | The coupling between positive feedback and damping is multiplicative (gain × (1 − damping)), not additive (gain − damping) | **Inferred structural** | Specific mathematical claim with consequences for threshold behavior |
| L9 | The multiplicative coupling produces threshold dynamics that are distinctive to this framework | **Inferred** | Requires distinguishing from subsystem-bistability mechanisms |
| L10 | Other theoretical biology frameworks (Noble, Rosen, Kauffman, network medicine, academic systems biology) do not have this cross-system-damping-collapse concept under different terminology | **Inferred comparative** | Claims distinctiveness without systematic comparison |

**Critical attack targets: L5, L6, L7, L8, L9.** L10 is worth a quick pass for honesty but rarely decisive. L1–L4 are textbook foundation and don't need attack effort.

### 1.4 Adjacent Measurements (Listed Before Searching)

Anchored on the underlying physiology, not the vault's vocabulary. Each is a potential search target.

**For "ATP availability" (Link 5 target):**
- ATP/ADP ratio
- ATP/AMP ratio
- Adenylate energy charge: ([ATP] + 0.5[ADP]) / ([ATP] + [ADP] + [AMP])
- Phosphocreatine/creatine ratio (PCr/Cr) — in muscle and brain
- ³¹P-MRS in vivo ATP measurement
- Mitochondrial membrane potential (Δψ_m) — feeds ATP production
- Oxygen consumption rate (OCR, VO2)
- Extracellular acidification rate (ECAR) — Seahorse Bioanalyzer
- P/O ratio (coupling efficiency)
- Steady-state ATP concentration

**For damping system function (Links 4–6 targets):**
- HPT: TSH response to TRH challenge, T4→T3 conversion rate, peripheral T3, reverse T3
- HPA: cortisol awakening response, dexamethasone suppression, CRH response, DHEA
- Antioxidant: GSH/GSSG ratio, SOD activity, catalase activity, glutathione peroxidase activity, NAD(P)H
- Mitochondrial biogenesis: mitochondrial mass markers (citrate synthase, COX activity), PGC-1α expression, mtDNA copy number, BrdU labeling of new mitochondria
- Autophagy/mitophagy: LC3-II/LC3-I ratio, p62/SQSTM1 levels, autophagic flux via chloroquine block, PINK1/Parkin activity, Mito-Keima imaging
- SPM immune resolution: resolvins (D-series, E-series), protectins, maresins serum/tissue concentrations; inflammation resolution kinetics
- HIF-1α degradation: HIF-1α protein half-life, VHL-mediated hydroxylation rates, PHD enzyme activity
- Hepatic regeneration: liver mass recovery kinetics after partial hepatectomy, Ki67 hepatocyte proliferation index
- Lactate clearance: lactate disappearance rate after standardized load, MCT1/MCT4 expression

**For alternative currencies (Link 7 target):**
- NADPH/NADP+ ratio (GSH regeneration, anabolic reductions)
- NAD+/NADH ratio (sirtuin activity, glycolytic flux regulation)
- Redox state markers (cytosolic, mitochondrial)
- Reduced coenzyme Q pool
- Membrane potential (Δψ_m) independent of ATP concentration
- FADH2/FAD ratio
- Acetyl-CoA concentration (substrate for many processes)

**For correlated failure (Link 6 target):**
- Multi-system longitudinal studies in chronic disease
- Graded metabolic perturbation studies measuring multiple damping systems simultaneously
- Multi-omic datasets capturing multiple pathways in the same individuals

**For threshold dynamics (Link 9 target):**
- Hysteresis loops in clinical measures (bariatric remission literature for glucose-insulin; do similar patterns exist elsewhere?)
- Critical slowing down signatures (autocorrelation, variance increase) before clinical transitions
- Dynamical systems analyses of chronic disease progression

### 1.5 Falsifiers (Explicit)

What would be inconsistent with the claim:

- **F1 (attacks L5).** Clean demonstration that one or more of the nine named damping systems continues to function at normal capacity under disease-state ATP reductions. If HPT axis TSH response to TRH challenge remained fully preserved at ATP levels measured in disease-state conditions, ATP would not be rate-limiting for HPT machinery maintenance in the relevant regime.

- **F2 (attacks L6).** Longitudinal data showing the damping systems fail on such different timescales (e.g., HPT in days, autophagy in hours, hepatic regeneration in months) that "simultaneous degradation" is an artifact of observation at a single chronic-disease time point rather than a shared causal process. The claim requires correlated kinetics, not just co-occurrence after a long time in disease.

- **F3 (attacks L6/L5).** Intervention data showing that restoring one damping system *independently* of the others (e.g., pharmacological restoration of autophagy without raising ATP) produces meaningful recovery that shouldn't be possible if the systems are truly coupled by shared ATP currency.

- **F4 (attacks L7).** Direct experimental evidence that NADPH (or NAD+/NADH, or redox state, or membrane potential, or substrate supply) is independently rate-limiting for a specific damping system in a way that decouples its behavior from ATP variation. The minimal version: an intervention that raises the alternative currency without changing ATP, and restores the damping system — demonstrating ATP was not the binding constraint.

- **F5 (attacks L8).** Experimental data showing the coupling between positive feedback gain and damping is additive (they oppose linearly) rather than multiplicative (gain × (1 − damping)). In an additive system, the effective gain does not surge as damping falls; the threshold behavior would be weaker, and bistability would require stronger positive feedback to compensate.

- **F6 (attacks L9).** Mathematical modeling or empirical demonstration that threshold dynamics in the framework's predicted scenarios are fully accounted for by subsystem-specific bistability mechanisms (ultrasensitivity, mutual inhibition, saturation) without requiring cross-system damping collapse. If the threshold behavior can be produced by the subsystem mechanisms alone, cross-system unification is not needed to explain the observed phenomena.

- **F7 (attacks L10).** Discovery that the cross-system damping collapse concept (under terminology like "coupled homeostatic failure," "shared-currency control theory," "network feedback collapse," etc.) is already present in adjacent frameworks and has been empirically tested or refuted there. Does not by itself refute P3 but would change the distinctiveness claim.

### What would NOT falsify (preventing goalpost moves)

The claim is scoped, and the stress test must respect that scope:

- **Not falsifying:** Finding that a specific damping system has non-ATP regulatory inputs. The vault does not claim ATP is the *only* input — it claims ATP is rate-limiting for machinery *maintenance* under disease-state conditions.
- **Not falsifying:** Finding that one system can fail independently in a specific pathology. The claim is about the general pattern under progressive metabolic decline, not universality across every possible disease state.
- **Not falsifying:** Finding that single-input interventions produce partial improvement. The claim is that multi-input intervention is needed to cross a threshold into the healthy attractor, not that single-input has zero effect.
- **Not falsifying:** Finding evidence of subsystem bistability mechanisms. These don't exclude cross-system damping; the vault explicitly names them as co-operating.
- **Not falsifying:** Finding that individual damping systems have ATP-dependent machinery. This is the textbook Layer A that is not contested.

### 1.6 Notes on Pre-Existing Vault Calibration

The vault already acknowledges several openings relevant to P3:

- **CF-L3.4 (open).** No integrated 6-variable ODE model with computed bifurcation diagram exists. A minimal 3-variable model (M-T-E core) would be the tractable first step. The kinetic data to parameterize exists scattered across the sub-system literature. This is a computational project the vault flags as open.
- **CF-L3.5 (open).** What specific parameter values (PUFA %, iron, cortisol, endotoxin) place an organism in the bistable vs. monostable region is unknown.
- **Explicit acknowledgment from the refinement doc:** "The generalization to the full 6-variable metabolic system remains structural inference — the other toggle switches (T-E, T-L) have not been independently tested for hysteresis — but the core metabolic fork (the M-Λ axis, the glucose-insulin dynamics) is empirically grounded."

**What this means for the stress test.** The vault openly acknowledges state-dependent damping as structural inference for systems beyond glucose-insulin. The stress test is not "discovering" that the claim is inferred — the vault says so. What the stress test needs to determine:

1. **Is the inference justified** by the evidence that does exist? (Not "is it proven?" — that's not the bar.)
2. **Are there specific pieces of evidence** that would materially strengthen or weaken the inference?
3. **Are there plausible alternative explanations** (especially regarding the shared currency — Link 7) that the vault hasn't engaged with?
4. **Is the specificity/predictiveness of the claim appropriate** given the evidence, or is the vault claiming more than it can support?

### 1.7 Phase 1 Completion Check

- [x] Claim restated in crispest form; hedges preserved in full form
- [x] Relationship to Core Claims classified: **Peripheral (supports 2 and 4; distinctive but not core)**
- [x] Prediction chain unpacked: **10 links; critical targets L5-L9**
- [x] Adjacent measurements listed before searching
- [x] Falsifiers stated explicitly (F1-F7)
- [x] Non-falsifiers stated (preventing goalpost moves)
- [x] Pre-existing vault calibration noted

Target is defined. Ready for Phase 2.

---

## Phase 2 — Attack

### 2.1 Verification Sequence

#### Step 1 — Deeply Understand What the Vault Predicts

The vault's claim generates specific predictions about what should be observed:

1. **Multiple damping systems simultaneously impaired in chronic disease**, not just one or two
2. **Correlation with cellular ATP/mitochondrial function**, not disease-specific pathology
3. **ATP restoration should restore multiple damping systems** with correlated kinetics, not just the targeted one
4. **Single-system interventions should plateau** because the system is maintained by other failing loops
5. **Threshold behavior** — damping should fail abruptly past some ATP level rather than linearly
6. **Cross-disease similarity** — different chronic diseases should show similar multi-system damping profiles where metabolic impairment overlaps
7. **Experimental ATP restoration** (mitochondrial biogenesis, Complex IV activation, PCr supplementation) should restore multiple damping systems with correlated kinetics

These are the predictions to test. The vault's case is strengthened where these are observed; weakened where they aren't.

#### Step 2 — Check the Framework's Own Metrics

Vault's metrics: V'CO₂, ETCO₂, RQ, blood lactate, body temperature, resting pulse, mitochondrial function markers.

**For state-dependent damping specifically, the relevant metrics are:**
- ATP/PCr ratio (direct cellular energy state)
- Mitochondrial membrane potential Δψ_m (functional)
- **Multiple damping system readouts in the same individuals** (cross-system correlation)
- **Temporal correlation across systems under intervention** (kinetic coupling)
- NAD+/NADH ratio (since sirtuins affect multiple damping systems)
- NADPH/NADP+ ratio (since GSH regeneration depends on it)

**What has actually been measured, systematically?**

The vault itself acknowledges the gap: CF-L3.4 (no integrated 6-variable ODE model with bifurcation diagram), CF-L3.5 (parameter-region boundaries unknown). The glucose-insulin subsystem has empirical hysteresis (bariatric remission, Tabak CSD); the cross-system damping claim has no equivalent direct empirical test. This is the honest starting point.

#### Step 3 — State the Contradiction (If One Survives)

At this step, no contradiction with external evidence surfaces because the claim is largely untested at the cross-system level. But Step 4 reveals an **internal tension**: the vault names ATP as *the* shared currency, while biochemistry shows multiple distinct coupled currencies (ATP, NAD+, NADPH, Δψ_m) each with specific mechanisms. This is the attack surface.

#### Step 4 — Identify Resolution Dependencies + Causal Independence Audit on Sub-Question 3d

**Load-bearing sub-claims the vault depends on:**

1. ATP is specifically the shared currency (Link 7)
2. Correlated failure across systems has shared kinetic basis (Link 6)
3. Coupling is multiplicative (Link 8)
4. Threshold dynamics distinctively attributable to cross-system coupling (Link 9)

**Causal Independence Audit on Link 7 (the core of sub-question 3d).**

Applying the four sub-checks from [[metabolic_framework/Verification Methodology]] Step 4:

**Sub-check 1 — Conservation.** ATP is stoichiometrically coupled to multiple variables in mitochondrial OXPHOS:
- Adenylate pool: ATP + ADP + AMP (conserved)
- O₂ consumption (ATP produced per O₂ consumed — P/O ratio)
- NADH/FADH₂ oxidation (electron donors at Complex I/II)
- Δψ_m (the proton-motive force that ATP synthase uses)
- NADPH via NNT (which uses Δψ_m, not ATP directly)
- PCr/Cr (creatine kinase buffer)

ATP is part of a tightly coupled network of mitochondrial outputs — not an isolated variable.

**Sub-check 2 — Mechanism specificity, system by system:**

| System | ATP mechanism specific? | Alternative currency with specific mechanism? |
|---|---|---|
| Protein synthesis (all machinery) | **Yes** — amino acid activation, GTP regeneration | — |
| Autophagy/mitophagy | **Yes** — LC3 lipidation, fusion | AMP/ATP ratio regulates via AMPK (sensor is ratio, not absolute ATP) |
| GSH regeneration | **No** — NADPH-specific at GSR | **NADPH** (from PPP, malic enzyme, IDH1 — not directly ATP-dependent) |
| SOD, GPx catalytic activity | **No** — uses metal cofactors, selenium | Cofactor supply |
| PGC-1α activation (biogenesis) | Partial (synthesis) | **NAD+ via SIRT1 deacetylation**; AMP/ATP via AMPK |
| SIRT3 mitochondrial regulation | **No** | **NAD+-dependent specifically** |
| SPM immune resolution | Protein synthesis only | EPA/DHA substrate availability |
| Hepatic regeneration | Synthesis costs | Amino acids, nucleotides, lipid substrates, growth factor signaling |
| HPT/HPA axis maintenance | Synthesis | mTOR signaling integration, substrate supply |
| HIF-1α degradation | VHL pathway — ATP for ubiquitination | **O₂, Fe²⁺, α-KG for PHD hydroxylation — not ATP** |

**Critical finding: ATP is system-specific, not universal.** For several damping systems, NADPH or NAD+ are independent rate-limiting currencies with their own specific mechanisms. The vault's claim that "ATP is the shared currency" is empirically inaccurate at the mechanism level.

**Sub-check 3 — Realizable intervention.** Can ATP be dissociated from alternative currencies? Yes:
- **NAD+ precursors** (nicotinamide riboside NR, nicotinamide mononucleotide NMN) raise cellular NAD+ without changing ATP; literature shows specific restoration of sirtuin-dependent functions (SIRT1, SIRT3) including mitochondrial biogenesis and autophagy regulation
- **PPP flux enhancement** raises NADPH without changing ATP; directly supports GSH regeneration capacity
- **Mild UCP-mediated uncoupling** dissociates Δψ_m from ATP (membrane potential consumed for heat rather than ATP production)
- **Creatine supplementation** buffers ATP via PCr without raising mitochondrial output

Each of these interventions, if they restore a specific damping system independent of ATP changes, refutes the "ATP is the shared currency" claim for that system.

**Sub-check 4 — Quantitative dominance.** Tissue-specific and disease-state-specific:
- In aging/chronic disease, **NAD+ depletion is well-documented** (Verdin, Sinclair literature) and often **more pronounced than ATP depletion** — ATP in chronic disease typically falls 10-30%, while NAD+ can fall 50%+
- NADPH dysfunction is central to oxidative stress pathology (Ying 2008 *Antiox Redox Signal*)
- Sirtuin dysfunction is implicated across multiple chronic diseases as a distinct mechanism from ATP depletion

**Classification of ATP as the "shared currency" via Causal Independence Audit:**
- For some systems (protein synthesis universally, autophagy mechanics): **ATP is an independent driver**
- For others (GSH regeneration, sirtuin-dependent regulation, HIF-1α hydroxylation): **ATP is NOT the rate-limiting driver; NADPH, NAD+, or O₂/Fe/αKG are**
- Overall: ATP is a **co-driver with other coupled currencies** (NAD+, NADPH, Δψ_m), all downstream of mitochondrial OXPHOS function

**The deeper shared variable is mitochondrial OXPHOS function** (the vault's variable M), which produces ATP, regenerates NAD+ via Complex I, maintains Δψ_m, and supports NADPH production via NNT. ATP is the most visible currency but not uniquely privileged among the coupled outputs.

#### Step 5 — Verify Dependencies Against Primary Sources

**Citation status flag.** The analysis above draws on textbook biochemistry (NADPH production pathways, sirtuin biology, mitochondrial coupling). Specific claims that would benefit from primary-source verification before being used as load-bearing:

- **Magnitude of NAD+ depletion vs ATP depletion in aging/chronic disease** — I cited "50%+ vs 10-30%" from training knowledge; specific cohort studies should be checked (Gomes et al. 2013 *Cell*, Camacho-Pereira et al. 2016 *Cell Metab*, Yoshino et al. 2011)
- **NR/NMN restoration of damping systems without ATP change** — the specific dissociation claim needs primary-source verification (e.g., Martens et al. 2018 *Nat Commun*, Dollerup et al. 2020 *Am J Clin Nutr*)
- **PPP flux as an independent NADPH restorer** — clinical/preclinical data on targeted intervention

These are flagged as verification-needed before any vault modification. The Phase 2 conclusion stands on the biochemistry (which is textbook) and can be strengthened by primary-source confirmation of magnitude claims.

**Citation Deployment Audit is not applicable here** — the vault doesn't cite specific papers for the ATP-as-shared-currency claim; it's stated as structural inference. So there's no citation to audit for species/scenario/endpoint/mechanism match.

#### Step 6 — Construct and Stress-Test the Resolution

**Proposed resolution:** Refine "ATP as shared currency" to "mitochondrial OXPHOS function as shared basis, producing ATP, NAD+, NADPH, and Δψ_m as coupled but dissociable currencies. Specific damping systems depend on different currencies: protein synthesis and autophagy are ATP-specific; antioxidant regeneration is NADPH-specific; sirtuin-mediated regulation (biogenesis, SIRT-driven autophagy) is NAD+-specific; HIF-1α hydroxylation requires O₂/Fe²⁺/α-KG."

**Stress-test of the resolution:**

- **Weakest link:** the empirical claim that NAD+ and NADPH can genuinely be dissociated from ATP in disease states with differential restoration of damping systems. NR/NMN literature supports this directionally but controlled cross-system measurements are sparse. If the currencies turn out to be tightly slaved together in practice (even if biochemically distinct), the refinement loses force.
- **Generosity check:** Am I being more generous to my alternative than to the vault's claim? The vault's "ATP as shared currency" is simpler and operationally useful (restoring M restores ATP and in practice ATP is a reasonable proxy for multiple downstream effects). My refinement is more precise but adds complexity. A rigorous observer would need to see that the added precision generates new testable predictions.
- **Precision vs. flexibility:** The refinement *narrows* the claim (not "ATP" but "ATP AND NAD+ AND NADPH AND Δψ_m as coupled currencies with specific system dependencies"). This is more specific, more falsifiable. **Passes the decisive test.**
- **New predictions generated:**
  - Prediction: NAD+ precursor supplementation should improve sirtuin-dependent damping systems (mitochondrial biogenesis, SIRT-mediated autophagy) with different kinetics than ATP-targeting interventions (thyroid hormone, Complex IV activation)
  - Prediction: Patients with NAD+ depletion (measured) should show selective impairment of sirtuin-dependent functions, dissociable from ATP-level impairment
  - Prediction: PPP-flux-enhancing interventions should selectively improve antioxidant function
  - Prediction: Multi-currency measurement should show partial dissociation across damping systems in cross-sectional clinical data

These predictions are novel relative to the current vault and testable.

### 2.2 H1 → H2 → H3 Escalation

**H1: Am I misunderstanding the vault?**

I traced the reasoning chain through The System.md, Foundation.md, Practice.md, and the Conditional Bistability refinement doc. The canonical claim in The System.md is explicit: "single coupling currency (ATP)." Practice.md is operational: "Restoring ATP production re-enables self-correction across systems simultaneously." The refinement doc is slightly broader ("energy-dependent"), introducing mild inconsistency with The System.md.

I am not misunderstanding. The specific ATP attribution is the vault's claim. The refinement I'm proposing doesn't require re-reading the vault; it requires accepting the biochemistry showing ATP is one of several coupled currencies.

**H2: Does the evidence measure the variables the vault's claims operate on?**

Yes. The analysis is directly about:
- ATP production and consumption (vault's named variable)
- Mitochondrial function (vault's M variable)
- Protein synthesis machinery (vault's "machinery maintenance")
- Damping system function (vault's named systems)

These are the vault's own variables. The finding is not artifact of measuring proxies.

**H3: The vault is wrong — at what level?**

- **Core thesis (cross-system unification exists):** NOT wrong. Damping systems *are* coupled through shared mitochondrial basis.
- **Specific attribution (ATP is the single currency):** Yes, this is narrowly wrong. The deeper variable is mitochondrial OXPHOS function; ATP is one of several coupled currencies.
- **Operational implication (restoring M restores multiple systems):** Directionally correct; practical interventions that restore M do improve multiple systems.

**The finding is Refinement-scale, not Fail.** The architecture survives. The claim is narrowed to be more precise.

### 2.3 Steel-Man Critique

The strongest version of the critique an informed theoretical biologist would make:

> "The state-dependent damping claim is clever but teetering on unfalsifiability. Almost every biological system is ATP-dependent in some way — naming ATP as 'the shared currency' is nearly tautological. The claim that systems fail 'together' is vague: they all do decline in chronic disease, but so does everything else. The multiplicative coupling claim requires ODE modeling the vault admits doesn't exist (CF-L3.4). The 'cross-system unifier' framing dresses up a banal observation (chronic disease involves multiple system failures) in dynamical systems language without delivering predictive specificity beyond what subsystem-level biology already provides. It also ignores NADPH and NAD+ biology entirely, despite those being central to damping system function in the literature (sirtuin field, redox biology). Without direct cross-system measurements, this is speculative structural inference, not tested hypothesis."

**How the vault currently answers:**
- Testable predictions (CSD, hysteresis, multi-input durability) provide falsifiable targets; two of six already observed
- Multiplicative coupling is standard multi-loop dynamical systems result (Brandman 2005), not ad hoc
- Pre-specifies what would constitute falsification

**How the refinement I propose strengthens the vault against this critique:**
- By acknowledging multiple coupled currencies (not just ATP), the claim becomes more biochemically accurate and generates system-specific testable predictions
- Distinguishes the framework's genuine contribution (shared *mitochondrial* basis coupling otherwise independent damping systems) from a weaker version ("they all need ATP")
- Gives pharmacology traction: NAD+ precursors, NADPH support, ATP-targeting all become distinguishable interventions testable in controlled studies

### 2.4 Alternative Explanations

**Alternative 1: Pure subsystem independence (no cross-system coupling).**

Each damping system has its own regulation and fails/recovers independently. The appearance of "multiple systems failing together in chronic disease" is because the same environmental drivers (PUFA accumulation, endotoxin, stress) affect multiple systems, but the systems aren't causally coupled through a shared currency — they're independently responding to the same inputs.

**Distinguishing evidence:** If true, single-system interventions would produce sustained improvement often (observed: mostly they plateau — consistent with coupling). Multi-omic profiling would show heterogeneous failure patterns across patients (observed: there is heterogeneity but also substantial common signature — partial coupling). Restoration of M alone would show uncorrelated damping recovery kinetics (partial data suggests correlated kinetics for many systems, uncorrelated for others).

**Current assessment:** Pure independence is refuted by the single-intervention plateau pattern. Full coupling is refuted by patient heterogeneity. **Reality is partial coupling** — the refinement I propose captures this (shared mitochondrial basis with dissociable currencies producing partial coupling).

**Alternative 2: The shared variable is not ATP specifically but mitochondrial function broadly.**

This is in fact what I'm proposing as the refinement. It's less an "alternative" than a more precise formulation.

**Alternative 3: NAD+ depletion is the primary driver, not ATP.**

Some in the aging/longevity field (Sinclair, Verdin) argue NAD+ is the primary currency driving sirtuin-mediated damping, and ATP depletion is downstream of NAD+ depletion (since NAD+ drives Complex I electron transport).

**Distinguishing evidence:** NR/NMN supplementation in aging improves multiple endpoints (biogenesis, autophagy, inflammation) but produces less dramatic recovery than expected if NAD+ were the primary driver. ATP-targeting interventions (T3, Complex IV activation) also work. The most parsimonious reading: **both NAD+ and ATP are co-drivers, along with NADPH and Δψ_m, all downstream of mitochondrial function.**

### 2.5 Rule Compliance Check

**Not applicable.** The proposed refinement does not invoke acute/chronic distinction or context-dependence to rescue the claim. The refinement is a direct biochemical narrowing: "ATP" → "mitochondrial OXPHOS function producing ATP and other coupled currencies."

---

## Phase 3 — Adjudicate

### 3.1 Verdict

**REFINEMENT.**

Not Pass — the specific ATP attribution is biochemically inaccurate. Not Fail — the cross-system unification *direction* is confirmed and the architecture survives. The claim needs narrowing, not abandonment.

**Precise characterization:**
- **Cross-system coupling via shared mitochondrial basis:** confirmed. Strengthened by this stress test.
- **ATP as THE single shared currency:** refuted. Shown to be oversimplified — multiple distinct coupled currencies (ATP, NAD+, NADPH, Δψ_m) operate downstream of mitochondrial OXPHOS function, each with system-specific mechanisms.
- **The framework's distinctive contribution:** real, but requires restatement to reflect multi-currency coupling rather than single-currency unification.

### 3.2 Decisive Test (More or Fewer Specific Predictions After Refinement?)

**More specific. Passes the Refinement bar.**

Before refinement:
- "ATP is the shared currency" — operational but biochemically imprecise; generates broad predictions

After refinement:
- "Mitochondrial OXPHOS function is the shared basis, producing ATP, NAD+, NADPH, Δψ_m as coupled but dissociable currencies with system-specific mechanisms" — generates **specific** new testable predictions:
  - NAD+ precursor supplementation should improve sirtuin-dependent damping (biogenesis via PGC-1α, SIRT-driven autophagy) with different kinetics than ATP-targeting interventions
  - Patients with measurable NAD+ depletion should show selective impairment of sirtuin-dependent functions, dissociable from ATP-level impairment
  - PPP-flux-enhancing interventions should selectively improve antioxidant function (GSH regeneration capacity)
  - Cross-sectional multi-currency measurement should show partial dissociation across damping systems, not lockstep co-variation

The refined claim is **narrower, more falsifiable, and generates new predictions**. This is the textbook definition of a refinement vs. an accommodation.

### 3.3 Scope

**Peripheral.**

The refinement affects:
- The specific currency attribution in The System.md's State-dependent negative feedback section
- The operational claim in Practice.md (Restoring M section)
- The cross-system unification framing in the Conditional Bistability refinement doc

None of the five Core Claims is modified:
- Core Claim 1 (health = oxidative metabolism) — untouched
- Core Claim 2 (bistability conditional on parameters) — untouched; state-dependent damping remains one of several bistability mechanisms
- Core Claim 3 (positive feedback self-maintenance) — untouched
- Core Claim 4 (multi-loop intervention required) — untouched; if anything strengthened by explicit multi-currency framing
- Core Claim 5 (daily oscillation) — untouched

### 3.4 Change Bar Assessment

Per [[metabolic_framework/Verification Methodology]]:

| Criterion | Met? | Notes |
|---|---|---|
| **Verified evidence** | Partially | Biochemistry is textbook (NADPH production pathways, sirtuin biology, NNT mechanism). Specific magnitude claims (NAD+ depletion vs ATP depletion; NR/NMN dissociation effects) flagged for primary-source verification before load-bearing use |
| **Measures vault's variables** | Yes | Analysis is directly about ATP, M, damping system function, NAD+/NADPH/Δψ_m — all vault-level variables |
| **Survives deep reading** | Yes | Traced The System.md, Foundation.md, Practice.md, Conditional Bistability refinement doc; the specific ATP attribution is the vault's claim and the refinement is at that level |
| **Precisely stateable** | Yes | Vault says "single coupling currency (ATP)"; refinement says "shared mitochondrial basis producing multiple coupled currencies" — specific, differential, falsifiable |

**The refinement clears the structural bar.** Two items flagged for primary-source verification before being finalized as a proposed vault edit:

1. Magnitude comparison of NAD+ depletion vs ATP depletion in aging/chronic disease (Gomes et al. 2013 *Cell*, Camacho-Pereira et al. 2016 *Cell Metab*, Yoshino et al. 2011)
2. NR/NMN supplementation studies showing damping-system restoration without ATP change (Martens et al. 2018 *Nat Commun*, Dollerup et al. 2020 *Am J Clin Nutr*, and related)

These verifications would promote the refinement from "structural case established" to "fully evidence-backed."

### 3.5 Confidence Change

**Directional, specific:**

- **Confidence in cross-system coupling existing:** INCREASED (from "structural inference" to "biochemically grounded in shared mitochondrial basis")
- **Confidence in ATP as THE shared currency:** DECREASED (from vault's stated formulation to "one of several coupled currencies")
- **Confidence in the framework's distinctive contribution being real:** INCREASED (the cross-system unifier story survives with a more precise formulation)
- **Confidence in practical recommendations (restoring M restores multiple systems):** INCREASED (but with added nuance — multi-currency targeting may outperform ATP-only)
- **Confidence in the multiplicative coupling specific claim (L8):** UNCHANGED (CF-L3.4 still open; requires ODE modeling to resolve)

**Net effect for the vault's foundational integrity:** marginally increased. The stress test strengthened the direction while narrowing the specific attribution. The refined claim is more accurate and more predictive than the original.

### 3.6 Proposed Refinement

**For [[metabolic_framework/The System]] — State-dependent negative feedback section:**

Replace:
> "the damping across otherwise independent systems weakens together under a single coupling currency (ATP), rather than failing independently"

With:
> "the damping across otherwise independent systems weakens together as mitochondrial OXPHOS function fails, coupled through multiple downstream currencies — ATP (for protein synthesis, autophagy mechanics), NAD+ (for sirtuin-mediated regulation including PGC-1α-driven biogenesis and SIRT-driven autophagy regulation), NADPH (for cofactor regeneration, particularly GSH), and membrane potential Δψ_m (for substrate import and NADPH production via NNT). These currencies are biochemically distinct with system-specific mechanisms and are dissociable by targeted interventions (NAD+ precursors, PPP enhancement, mild uncoupling, creatine buffering), but share the mitochondrial OXPHOS origin — producing correlated but not identical damping system degradation when M fails."

**For [[metabolic_framework/Practice]] — State-dependent damping section:**

Append after the existing paragraph:
> "The currencies are coupled but dissociable. ATP-targeting interventions (thyroid restoration, Complex IV activation via 670nm light, reducing PUFA-driven respiratory chain damage) primarily improve ATP production. NAD+ precursors (nicotinamide riboside, nicotinamide mononucleotide) selectively restore sirtuin-mediated damping. PPP flux support improves NADPH-dependent antioxidant regeneration. In the bistable regime, multi-currency restoration tends to outperform single-currency targeting because different damping systems depend on different currencies."

**For the Conditional Bistability refinement doc** — note that the "single coupling currency (ATP)" framing from The System.md is refined in this P3 stress test finding.

### 3.7 Primary-Source Verification (performed 2026-04-17)

The load-bearing claims flagged in §3.4 were verified via targeted literature search. The verification **partially supports** the refinement and **materially qualifies** parts of the Phase 2 analysis.

#### Verified and confirmed

**Gomes et al. 2013 *Cell* (PMID 24360282)** — "Declining NAD+ Induces a Pseudohypoxic State." Confirmed:
- Declining nuclear NAD+ in aging disrupts nuclear-mitochondrial communication via a **PGC-1α/β-INDEPENDENT** pathway (SIRT1 → HIF-1α pseudohypoxia)
- Raising NAD+ in old mice restores mitochondrial function in a SIRT1-dependent manner
- **Correction to my Phase 2 analysis:** I associated NAD+-SIRT1 specifically with the canonical SIRT1-PGC-1α pathway for biogenesis. Gomes 2013 is actually the alternative PGC-1α-INDEPENDENT pathway. Both pathways exist (Rodgers 2005 is the canonical SIRT1-PGC-1α), and my broader point (NAD+ as independent damping-relevant currency via SIRT1) stands — but the specific mechanistic cite should distinguish the two.

**Camacho-Pereira et al. 2016 *Cell Metabolism* (PMID 27304511)** — Confirmed:
- CD38 expression/activity increases with aging
- 32-month WT mice have ~50% of young NAD+ levels; CD38 KO preserves NAD+ and mitochondrial function
- CD38 is the main in vivo degrader of NMN — directly relevant to NMN supplementation pharmacology
- **SIRT3** (not SIRT1) is the mediator of the preserved mitochondrial function in CD38 KO — another specific mechanism distinct from the SIRT1 pathway

**NADPH production via PPP is ATP-independent (textbook).** Confirmed via standard biochemistry sources:
- PPP generates NADPH via G6PD (rate-limiting) + 6PGD; **no ATP consumed in the oxidative branch**
- Each glucose through PPP yields 2 NADPH
- NADPH supports GSH regeneration and biosynthetic reductions
- **This is the cleanest confirmed case for an independent damping-relevant currency: NADPH is biochemically and mechanistically ATP-independent, and it is specifically required for antioxidant regeneration.**

#### Verified with material qualifications

**Human NR clinical trial evidence is substantially weaker than I implied in Phase 2:**

- **Martens et al. 2018 *Nat Commun*** (healthy adults, 1000mg NR): elevated blood and muscle NAD+, "boosts mitochondrial bioenergetics," decreased inflammatory cytokines — consistent with NR as NAD+ booster
- **Dollerup et al. 2020 *Am J Clin Nutr* (PMID 31710095 / 32463114)** — in obese, insulin-resistant men, 12 weeks of 1000mg NR twice daily: **did NOT alter skeletal muscle NAD+, NADH, NADP+, or NADPH** and did **NOT** alter mitochondrial respiration, content, or morphology. NAMPT was decreased.
- **General consensus (Science Advances 2023 review):** "clinical evidence that raising NAD+ concentrations can improve physiological function is unclear"

**Implication:** my Phase 2 framing that "NR/NMN supplementation reliably dissociates NAD+ from ATP with damping restoration" was too strong. The mouse preclinical literature supports this story; human translation is inconsistent and tissue delivery is unreliable.

**Magnitude claims corrected:**
- NAD+ decline in aging is tissue-specific: 10-30% in human muscle, 10-50% in liver, ~60% in plasma across lifespan
- ATP depletion in chronic disease can be substantial: ~47% reduction in γ-ATP in liver disease models (31P-MRS), significant reductions in hemodialysis patients, altered PCr/ATP in cardiovascular disease
- **My "NAD+ falls more than ATP" framing was not universally supported.** Both can fall substantially; the relative magnitudes are tissue-specific and disease-specific.

#### Material challenge discovered during verification

**Chubanava et al. 2025 *Cell Metabolism* (PMID 40311622)** — "NAD depletion in skeletal muscle does not compromise muscle function or accelerate aging." Published April 30, 2025 — before the vault's `last-verified: 2026-04-15` for The System.md.

Key findings:
- Mouse model with **85% reduction in muscle NAD+** via NAMPT disruption in adult skeletal muscle
- **No functional impairment** — preserved muscle morphology, contractility, exercise tolerance
- **Intact mitochondrial respiratory capacity**
- **Unaltered transcriptomic and proteomic profiles**
- Lifelong NAD depletion did not accelerate muscle aging or impair whole-body metabolism
- Accompanying press coverage framed this as "low NAD+ may not drive aging"

**This is genuinely challenging evidence.** It directly attacks the causal claim that NAD+ depletion drives damping system failure, at least for skeletal muscle. Important caveats before over-interpreting:

- **Tissue-specific.** Only skeletal muscle was tested. Liver, brain, immune cells, cardiac muscle could behave differently (and Gomes 2013 + Camacho-Pereira 2016 findings were on other tissues/systems).
- **Lifelong depletion allows compensation.** Adult-onset acute depletion might show different results; the mouse had time to adapt.
- **Functional endpoints were gross muscle function.** Subtle sirtuin-dependent functions (stress resilience, aging trajectory) might be impaired in ways not captured.
- **NAD depletion mechanism was specific** (NAMPT disruption) — other NAD-depleting mechanisms (CD38 activation, PARP1 consumption) might have different phenotypes.

But it's a significant finding that genuinely constrains the NAD+-as-causal-driver claim. It suggests NAD+ homeostasis has substantial redundancy in skeletal muscle and potentially other tissues.

### 3.8 Revised Verdict and Confidence Assessment

**Verdict remains: REFINEMENT, Peripheral scope.**

The refinement's core claim — "ATP is not the single shared currency; the deeper variable is mitochondrial OXPHOS function with multiple coupled currencies (ATP, NAD+, NADPH, Δψ_m) having system-specific mechanisms" — **survives verification, with revised confidence weighting across the sub-claims:**

| Sub-claim | Pre-verification confidence | Post-verification confidence | Reason |
|---|---|---|---|
| NADPH is an independent damping-relevant currency (GSH regeneration) | Moderate | **High** | PPP biology is textbook; NADPH mechanism for GSH is unambiguous; ATP-independent production confirmed |
| NAD+ is an independent damping-relevant currency (sirtuin-mediated regulation) | Moderate | **Reduced to moderate-low** | Gomes 2013 and Camacho-Pereira 2016 support causal role in aging mice; Chubanava 2025 challenges it for muscle; human NR trials inconsistent |
| Membrane potential (Δψ_m) is distinct from ATP | Moderate | **Moderate** (unchanged) | Uncoupling biology supports dissociation; limited direct evidence for damping-specific effects |
| ATP as sole shared currency (the vault's original claim) | Refuted by Phase 2 analysis | **Refuted** (unchanged) | PPP biochemistry alone refutes "ATP is the single currency" |
| Practical utility of multi-currency interventions (NR/NMN) for humans | Implicit moderate | **Low** | Human NR trials inconsistent; tissue delivery unreliable; Dollerup 2020 null finding material |

**Net effect on P3 conclusion:**

- The refinement is **less aggressive** than my Phase 2 initially suggested. The cleanest case is NADPH (textbook, mechanistically specific, biochemically ATP-independent). The NAD+ case is **contested** — real in some preclinical contexts, challenged in others, poorly translated to humans.
- The **practical intervention claim** (that NR/NMN could selectively restore NAD+-dependent damping) is **materially weakened** for humans. This matters for Practice.md.
- The **ontological claim** (multiple coupled currencies downstream of mitochondrial function) is **strengthened** by the biochemistry verification but requires more careful scoping.

**Revised proposed refinement** (replacing §3.6):

For **The System.md**, replace "single coupling currency (ATP)" with:
> "coupled currencies downstream of mitochondrial OXPHOS function — including ATP (for protein synthesis and autophagy mechanics), NADPH (for antioxidant cofactor regeneration, produced independently via the pentose phosphate pathway), and membrane potential Δψ_m (for substrate import and coupled currency production via NNT). NAD+ is additionally coupled to mitochondrial function via Complex I and is required for sirtuin-mediated regulation, though recent data (Chubanava 2025) suggests the causal role of NAD+ decline in damping system failure may be tissue-specific and not universal. The shared mitochondrial basis produces correlated but not identical degradation of these currencies and the damping systems that depend on them."

For **Practice.md**, replace the "shared currency" framing with:
> "Restoring M is the priority that unlocks every other because it is the shared basis of multiple coupled currencies. In practice, ATP-targeting interventions (thyroid restoration, Complex IV activation via 670nm light, reducing PUFA-driven respiratory chain damage) primarily improve ATP production and the antioxidant pathways NADPH supports. Direct NAD+-targeting interventions (NR, NMN) have shown inconsistent effects in human trials and should not be assumed to reliably translate preclinical findings."

### 3.9 Gaps Remaining

Three items the stress test did not close:

1. **L8 — multiplicative vs additive coupling.** Requires ODE modeling the vault acknowledges doesn't exist (CF-L3.4). Not resolvable by literature search alone.

2. **Cross-system kinetic correlation measurements under intervention.** The ideal test would be simultaneous measurement of multiple damping system functions under graded ATP-targeting vs NAD+-targeting interventions. Scattered fragments exist across disciplines; no systematic cross-system kinetic study identified in this pass.

3. **Tissue-specificity of NAD+ causation.** Chubanava 2025 is skeletal muscle only. The generalization to other tissues (liver, brain, immune cells, heart) is unresolved — Gomes/Camacho-Pereira support causal NAD+ role in their systems; Chubanava challenges it in muscle. Resolution would require tissue-by-tissue examination that this stress test did not perform.

### 3.10 Summary

**P3 verdict: REFINEMENT, Peripheral scope.** The vault's "single coupling currency (ATP)" framing is refuted — biochemistry unambiguously shows NADPH production is ATP-independent via PPP and NADPH is specifically required for antioxidant regeneration. The deeper variable is mitochondrial OXPHOS function producing multiple coupled currencies with system-specific mechanisms. Core Claims 1-5 all survive.

**Key qualification from verification:** the NAD+-as-independent-driver component of the refinement is more contested than the NADPH case. Chubanava 2025 (85% NAD+ depletion in muscle with no functional impairment) and Dollerup 2020 (NR failed to raise muscle NAD+ or function in obese men) are material constraints on how strongly to claim NAD+ as a cross-system independent damping currency. The NADPH component of the refinement is strongly supported; the NAD+ component is directionally supported but tissue-specific and not reliably human-translatable via current supplementation.

**Practical translation for the vault's Practice.md:** the shared-currency claim should be restated without committing to specific non-ATP pharmacological interventions (NR/NMN) as clinical tools, because human evidence does not support their reliable efficacy.

---

## Phase 4 — Independent Agent Triangulation

### 4.1 Method

Three independent `general-purpose` agents were dispatched in parallel with distinct angles, each without knowledge of the others or my P3 conclusion. Each received the vault's **original** claim (ATP as shared currency) and asked to evaluate independently, not to verify my finding.

- **Agent 1 — Biochemistry audit.** Go through each of the 9 named damping systems; identify actual rate-limiting factors; classify whether ATP is the shared currency.
- **Agent 2 — NAD+ causation literature 2020-2026.** State of evidence for NAD+ as causal driver of damping system failure; how key papers fit together; field consensus assessment.
- **Agent 3 — Theoretical biology framings.** Does the concept exist in adjacent frameworks (Noble, Rosen, Kauffman, Barabási, Prigogine, network medicine, control theory)? Is ATP the right shared variable? Bistability mechanism ranking.

### 4.2 Convergence

All three agents independently reached the same core conclusion: **"ATP as single shared currency" needs refinement; the shared basis is mitochondrial competence / respiratory capacity producing multiple coupled currencies.** The convergence across independent angles meaningfully strengthens the P3 finding.

### 4.3 Material Additions from Triangulation

Seven first-principles-relevant additions emerged that were not in my original Phase 2-3 analysis:

**4.3.1 Atkinson's adenylate energy charge (1968) as the theoretical precedent.** (Agent 3). [ATP] itself is heavily buffered near-constant by creatine phosphate, adenylate kinase, and homeostasis — it is a poor state variable because it changes late and abruptly. Atkinson (1968) proposed **energy charge** (ATP + 0.5·ADP) / (ATP + ADP + AMP) as the universal stoichiometric coupling agent for metabolic regulation. AMPK functions as "adenylate charge-regulated protein kinase" (Oakhill et al. 2011 *Science*), which directly confirms Atkinson's 1968 hypothesis in modern form. AMPK senses AMP/ATP ratio, not absolute ATP. **Implication:** the vault's "ATP" is too narrow; the biochemically correct shared variable is energy charge, or more broadly mitochondrial competence producing energy charge + reductive charge + membrane potential in parallel.

**4.3.2 Fried/Walston/Cohen frailty framework (Nature Aging 2020/2021) as the closest existing concept.** (Agent 3). "The physical frailty syndrome as a transition from homeostatic symphony to cacophony" (PMID 34476409, Nature Aging) states: "Physical frailty is conceptualized as a state, largely independent of chronic diseases, that emerges when the dysregulation of multiple interconnected physiological and biological systems crosses a threshold to critical dysfunction" — with "energetics as the key driver." This is very close to the vault's state-dependent damping claim, applied to aging. **Implication:** the framework's "distinctive contribution" framing requires material scoping — the genuine novelty is narrower than "new concept." It is (a) applying the frailty-energetics insight to chronic disease generally rather than only aging, and (b) explicitly formalizing as a bistability-generating mechanism in dynamical-systems terms (rather than a homeostatic-dysregulation concept).

**4.3.3 Δψm as cleanly dissociable from ATP via uncoupling protonophores.** (Agent 1). Mitophagy is triggered by Δψm collapse *specifically* — PINK1 is activated by Δψm depolarization, not by ATP depletion. Experimental dissociation: CCCP and FCCP (protonophore uncouplers) collapse Δψm while glycolytic ATP remains intact, and this triggers Parkin recruitment and mitophagy. This is the cleanest specific-mechanism counter-example to single-ATP-currency — independent experimental evidence that Δψm is a distinct currency from ATP for at least one named damping system.

**4.3.4 Robert Rosen's (M,R) systems as deeper theoretical precedent.** (Agent 3). Rosen's relational biology formalizes the dependence of Repair (R) functions on Metabolism (M) — structurally identical to "damping machinery requires ATP." Rosen never specified ATP, but the relational structure of "repair functions are sustained by metabolic outputs and their failure cascades" is the same. **Implication:** the theoretical precedent is deeper than the framework acknowledges.

**4.3.5 HPA steroidogenesis is NADPH-dependent, not ATP-dependent.** (Agent 1). Cortisol's rate-limiting step is StAR-mediated cholesterol delivery to CYP11A1 on the inner mitochondrial membrane, and CYP11A1 + downstream P450s require NADPH delivered via adrenodoxin reductase/adrenodoxin. The rate-limiting *cofactor* is NADPH. ATP is involved only for StAR phosphorylation and synthesis. My Phase 2 analysis was insufficiently specific — I said "HPA protein synthesis" without identifying NADPH as the rate-limiting steroidogenesis cofactor.

**4.3.6 HPT deiodination / thyroid H2O2 production has specific cofactor requirements.** (Agent 1, with a caveat — see 4.4 below). Thyroid hormone synthesis requires DUOX-generated H2O2 with NADPH as the electron donor. DIO1/DIO2/DIO3 are selenoproteins (selenium-dependent). Iodotyrosine deiodinase (IYD) recycling requires NADPH via ferredoxin reductase. The HPT axis is not primarily ATP-limited at the catalytic level; it is selenium-limited and NADPH-limited for its specific reactions.

**4.3.7 Tissue-specificity of NAD+ causation with authorial self-correction.** (Agent 2). Camacho-Pereira et al. 2023 (PMID 37774804) — the same lab that published the canonical 2016 CD38 paper — revised their brain claim, finding CD38 doesn't dictate brain NAD+ but regulates ROS in brain instead. Additional positive clinical findings in stressed contexts: Yoshino/Mills 2021 *Science* (NMN improved muscle insulin sensitivity ~25% in prediabetic women); NR-COPD 2024 *Nature Aging* (IL-8 reduced ~52%); Shoji 2025 (NR improved arterial stiffness in Werner syndrome). Emerging tissue-specific reconciliation: NAD+ matters in **stressed/disease contexts and specific tissues** (liver, immune, vascular), less so in **healthy unstressed tissue** (Chubanava 2025 skeletal muscle). Frederick/McGaunn/Baur 2025 commentary "Muscle needs NAD, but how much?" frames this explicitly.

**4.3.8 Unfalsifiability risk flagged.** (Agent 1). "Maintenance of machinery" is the framework's escape hatch — at sufficient time scales all protein synthesis is ATP-dependent, so the claim becomes unfalsifiable if interpreted loosely. The boundary between "named molecular mechanism" and "non-specific bulk supply" matters for whether the claim is structural or merely descriptive. **Implication:** the vault's formulation should be specific about *proximal* rate-limiting factors, not just *ultimate* ATP dependence.

**4.3.9 Bistability mechanism ranking.** (Agent 3). In the theoretical/experimental bistability literature, the established mechanisms rank roughly:
1. Positive feedback + ultrasensitivity (Ferrell, Goldbeter-Koshland) — strongest, canonical (Xenopus oocyte, MAPK)
2. Mutual inhibition / toggle switches (Gardner-Collins 2000, Thomas) — strong, experimentally constructed
3. Multisite phosphorylation / saturation of positive feedback — well-established
4. **State-dependent damping / shared currency collapse** — implicit in frailty, hallmarks-of-aging, and ISR literatures, but **not formalized as a bistability-generating mechanism** in dynamical-systems treatments. This is where the framework's genuine contribution sits.
5. Stochastic / noise-induced bistability — separate

### 4.4 Direct Verification of Key Triangulation Additions

Three most first-principles-important additions were directly verified by independent web search (separate from the agents' searches):

**Atkinson energy charge + AMPK (CONFIRMED).** Atkinson 1968 PMID 4972613 is the canonical source. Oakhill et al. 2011 *Science* (PMID 22284532) "AMPK functions as an adenylate charge-regulated protein kinase" confirms the energy charge hypothesis in modern form. AMPK is activated by AMP binding (not ATP directly), and ATP promotes dephosphorylation — the activation responds to energy charge, not absolute ATP. The concept is not historical curiosity; it is the established framing in current systems biology.

**Fried/Walston frailty framework (CONFIRMED).** Fried et al. 2020/2021 *Nature Aging* PMID 34476409 is the canonical modern source. The quoted language is verbatim. The framework explicitly invokes network physiology, threshold dynamics, multisystem energetics, and multi-system convergence to dysfunction — all central to the vault's state-dependent damping claim. **Scoping distinction that preserves vault novelty:** the vault applies to chronic disease generally (not only aging) and formalizes as a bistability mechanism in dynamical systems terms (not only a homeostatic-dysregulation concept). These distinctions are real but narrower than the vault's original framing suggests.

**PINK1/Parkin Δψm specificity (CONFIRMED).** "PINK1 is activated by mitochondrial membrane potential (Δψm) depolarization" (PMC3376738). CCCP and FCCP as protonophore uncouplers dissociate Δψm from ATP. "Cytosolic Parkin translocates to mitochondria upon exposure to 10 μM CCCP or FCCP" (PNAS PMC2806779). This is standard experimental biology and directly demonstrates Δψm ≠ ATP for mitophagy.

**Caveat flagged during verification:** Agent 1's HPT claim conflated IYD (iodotyrosine deiodinase, NADPH-dependent via ferredoxin reductase) with the classical DIO1/2/3 deiodinases (selenium-dependent, different mechanism). Both are involved in thyroid biology but represent different reactions. Not a material error for the P3 conclusion (both NADPH and selenium are independent from ATP) but a precision issue worth noting.

### 4.5 Final Consolidated Refinement

Incorporating all Phase 2-4 findings, the refined claim is:

> **Negative feedback systems in the organism share a dependence on mitochondrial respiratory capacity, which jointly produces multiple coupled currencies — adenylate energy charge (ATP + 0.5·ADP)/(ATP + ADP + AMP), reductive charge (NADPH/NADP+, NAD+/NADH), membrane potential Δψ_m, and proton-motive force — each with system-specific mechanisms. Cellular enzymes sense energy charge, not absolute [ATP], which is heavily buffered by creatine phosphate and adenylate kinase. Damping systems fail together when mitochondrial competence falls because the coupled currencies decline together, though not in kinetic synchrony; specific systems (GSH regeneration via NADPH, mitophagy via Δψ_m, sirtuin-mediated regulation via NAD+ in stressed contexts, steroidogenesis via NADPH, deiodinase via selenium/NADPH) have distinct proximal rate-limiting factors. This cross-system coupling via shared mitochondrial substrate is conceptually related to but more specific than the frailty-energetics framework (Fried, Walston, Cohen 2020 *Nature Aging*) and Atkinson's (1968) adenylate energy charge, explicitly formalizing the phenomenon as a bistability-generating mechanism alongside ultrasensitivity, mutual inhibition, and saturation of positive feedback in the dynamical-systems architecture.**

### 4.6 Updated Proposed Vault Refinement

For **The System.md** (State-dependent negative feedback section), replace "single coupling currency (ATP)" with:

> "coupled currencies downstream of mitochondrial respiratory capacity — adenylate energy charge (the variable enzymes actually sense via AMPK; Atkinson 1968; Oakhill et al. 2011 *Science*), reductive charge (NADPH for antioxidant cofactor regeneration and steroidogenesis; NAD+ for sirtuin-mediated regulation in stressed contexts), and membrane potential Δψ_m (the specific trigger for PINK1/Parkin-mediated mitophagy, dissociable from ATP via uncoupling protonophores). Each damping system has system-specific proximal rate-limiting factors (HPT: selenium + NADPH; HPA: NADPH via adrenodoxin reductase; antioxidants: NADPH + cysteine + trace metals; biogenesis: AMP/ATP ratio + NAD+ in stressed contexts; mitophagy: Δψ_m specifically; SPMs: PUFA substrate; regeneration: growth factor signaling + amino acids/nucleotides). The systems share the mitochondrial respiratory substrate but not identical kinetics; they decline in the same direction when M falls but not on synchronized clocks."

Also add a scoping note relating to existing frameworks:

> "This cross-system unification via shared mitochondrial substrate is conceptually related to the frailty-energetics framework (Fried, Cohen, Walston 2020-2021 *Nature Aging* — 'the physical frailty syndrome as a transition from homeostatic symphony to cacophony'), the hallmarks-of-aging mitochondrial-node framing (López-Otín et al. 2013, 2023), and the adenylate energy charge concept (Atkinson 1968). The framework's specific contribution is the formal treatment of this phenomenon as a bistability-generating mechanism in dynamical-systems terms alongside ultrasensitivity, mutual inhibition, and saturation of positive feedback — applied to chronic disease generally rather than only aging."

For **Practice.md**, update the interventional framing to be explicit about currency-specificity:

> "Restoring mitochondrial respiratory capacity (M) is the priority that unlocks multiple damping systems because they share M as upstream substrate. In practice, ATP-targeting interventions (thyroid restoration, Complex IV activation via 670nm light, reducing PUFA-driven respiratory chain damage) primarily improve adenylate energy charge and, through maintained respiration, also reductive charge and membrane potential. Direct currency-specific interventions (NAD+ precursors NR/NMN) have shown **tissue-selective** effects: meaningful in specific stressed contexts (prediabetes — Yoshino/Mills 2021; COPD inflammation — Brown 2024; Werner syndrome — Shoji 2025) but unreliable for healthy or insulin-resistant muscle (Dollerup 2020; Chubanava 2025). The practical implication: address M upstream rather than chase individual currencies pharmacologically."

### 4.7 Final Verdict and Confidence

**Verdict: REFINEMENT, Peripheral scope.** All three agents independently converged on this. Core Claims 1-5 preserved.

**Confidence change (consolidated across Phase 2-4):**
- Framework direction (cross-system coupling via shared mitochondrial substrate): **strongly increased** — now supported by triangulation, Atkinson theoretical precedent, Fried/Walston empirical precedent, and Δψm dissociation evidence
- Specific ATP-as-single-currency claim: **strongly refuted** — agent 1's biochemistry audit, Atkinson precedent, and Δψm/NADPH mechanistic dissociation all confirm
- Framework's distinctive contribution framing: **materially qualified** — the concept exists in frailty literature; genuine novelty is narrower (chronic disease generalization + bistability-mechanism formalization)
- NAD+ as universal independent driver: **weakened** — tissue-specific, stress-context-dependent; not reliably human-translatable via current supplementation
- Practical interventional implications: **strengthened** in direction, **narrowed** in pharmacological commitment

### 4.8 Overall Assessment for the Vault

Before this stress test, my estimation of the framework's state-dependent damping claim was roughly "moderate confidence structural inference." After Phase 2-4 (including primary-source verification + triangulation + direct verification of triangulation additions), my estimation is **higher confidence in the directional claim with materially refined specific claims**. The framework's central insight — that negative feedback systems in the organism share mitochondrial substrate and fail together when M falls — is real, is grounded in existing theoretical and empirical precedent (Atkinson, Rosen, Fried/Walston, hallmarks-of-aging, ISR, frailty network physiology), and has specific testable biochemistry. The framework's original formulation ("ATP as single coupling currency") is inaccurate in specifics but captures the right direction.

**For the user's original concern** (is the vault worth deep investment?): the state-dependent damping finding **supports yes** with the honest caveat that several claims need refinement at the specific-mechanism level. The architecture is sound; the details need updating. This is exactly what a healthy correctable integration should look like under rigorous stress testing.

---

## Phase 5 — Methodology Guardrail Retrospective (Added 2026-04-17)

Applied to P3 after the Methodology Guardrails were added to `Stress Test Plan.md`. This retrospective verifies whether the P3 analysis holds up under the new guardrails or requires correction.

### 5.1 Guardrail 1 (Causal Chain Tracing Discipline)

**Applicability check:** P3 evaluated a biochemistry/mechanism claim (is ATP the rate-limiting cofactor for each damping system's machinery maintenance?). This is not a causal-direction claim about hallmark interactions; it's a proximal mechanism question about cofactor requirements.

**Guardrail 1 applies partially:** whenever intervention evidence is cited (Dollerup 2020 NR supplementation, Chubanava 2025 NAD+ depletion model), the chain should be traced.

- **Dollerup 2020:** NR supplementation target = cellular NAD+ via NR phosphorylation to NMN to NAD+. Observed: didn't raise muscle NAD+. Chain: supplementation → absorption → tissue uptake → cellular conversion → NAD+ pool → NAD+-dependent enzyme function. Dollerup finding: the tissue-delivery step fails in obese men. This is a pharmacokinetics finding, not a causal-direction finding. **P3's interpretation is correct.**
- **Chubanava 2025:** 85% NAD+ depletion in mouse skeletal muscle via NAMPT KO. Observed: preserved function. Chain: NAD+ levels → NAD+-dependent enzyme activity → function. Chubanava finding: at this level of depletion in this tissue, NAD+ is not rate-limiting for the functions measured. This is a mechanism question about NAD+ rate-limitation, not a causal-direction claim. **P3's interpretation is correct.**

**Verdict:** Guardrail 1 does not change P3's conclusions.

### 5.2 Guardrail 2 (Intervention Specificity Caveat)

**Applicability check:** whenever a metabolic intervention fails, check whether it addressed the specific metabolic mechanism.

- **Dollerup 2020 NR failure** in obese insulin-resistant men: NR targets NAD+ pool via NR-specific pathway. If the NAD+ dysfunction in obese men is primarily via CD38 upregulation (Camacho-Pereira 2016), NR supplementation might be insufficient because CD38 activity degrades NMN before it can raise NAD+. **This is actually a Guardrail 2 consideration I didn't apply explicitly in P3.**
- Partial update to P3: The Dollerup 2020 null finding may reflect NR's insufficient potency against CD38-mediated NAD+ degradation, not a refutation of NAD+ as an independent damping currency. This was noted in P3 ("the tissue-delivery step fails") but the specific CD38 mechanism could be emphasized.
- Chubanava 2025: the intervention (NAMPT KO) directly targets the NAD+ biosynthesis pathway. If NAD+ pool is still maintained at 15% (85% reduction) and function is preserved, that's a genuine mechanistic finding about NAD+ not being rate-limiting for muscle function at that level, not an intervention specificity issue.

**Verdict:** Minor addition to P3 — Dollerup 2020's null finding is compatible with CD38-mediated NAD+ degradation being the bottleneck, not NAD+ supply per se. Doesn't materially change P3's conclusions but adds nuance.

### 5.3 Guardrail 3 (Mechanistic Specificity vs Unfalsifiability)

**Applicability check:** the P3 refinement claim ("mitochondrial OXPHOS function as shared basis, producing multiple coupled currencies") needs to be specific, not hand-wavy.

- P3's refinement IS specific: it names ATP, NADPH, NAD+, Δψ_m as distinct currencies with system-specific mechanisms (NADPH for GSH regeneration; NAD+ for sirtuin-mediated regulation; Δψ_m for PINK1/Parkin mitophagy). Each is mechanistically traceable.
- The refinement avoids the unfalsifiability trap by requiring specific pathway attribution per damping system.

**Verdict:** Guardrail 3 is satisfied in P3. The refinement is specific and falsifiable.

### 5.4 Guardrail 4 (Topology vs Causation)

**Applicability check:** does P3 treat "coupled currencies" as causal peers or as topologically coupled nodes?

- P3's framing: "multiple coupled currencies downstream of mitochondrial OXPHOS function" — correctly frames the currencies as topologically coupled but with specific mechanisms at different nodes. Does not claim they're parallel causal competitors.
- The refinement explicitly preserves mitochondrial centrality: the currencies are all DOWNSTREAM of mitochondrial function. This is causal direction, not peer-level framing.
- The relationship to Fried/Walston frailty framework and hallmarks-of-aging is properly framed (conceptually related but with P3's specific formulation being more precise).

**Verdict:** Guardrail 4 is satisfied in P3. The refinement maintains metabolic centrality rather than fragmenting into peer currencies.

### 5.5 Retrospective Summary

**P3 holds up under the Methodology Guardrails.** The refinement is:
- Mechanistically specific (not hand-waved)
- Preserves causal direction (currencies downstream of mitochondrial function)
- Distinguishes topology from causation correctly
- Acknowledges intervention specificity issues (NR failure due to tissue delivery, not NAD+ irrelevance)

**Minor clarification added:** The "multiple coupled currencies" framing in P3 should be read as "coupled outputs of mitochondrial competence with system-specific mechanisms," not as "parallel causal peers." The refinement strengthens the vault's claim about metabolism as foundational, it doesn't fragment it into competing hallmarks.

**No P3 verdict change.** Still Refinement, Peripheral scope. Still supports vault direction with material sharpening of specific mechanisms.

**The P3 finding remains distinct from P1:** P3 refined a specific mechanism (ATP as single currency → multiple coupled currencies from mitochondrial OXPHOS). P1, after correction, preserves Core Claim 1 intact. The two findings are compatible: metabolism is the dominant convergence point (P1), and the specific currency coupling is via multiple mitochondrial outputs (P3).

---

## Phase 6 — Triangulation Additions (2026-04-17)

After P3 verdict was established, an independent biochemistry agent was dispatched to verify specific mechanistic claims and look for overstatement/understatement. The agent confirmed the P3 direction with three minor additions needed:

### 6.1 NADPH Indirect ATP Coupling

**The refinement's claim** — NADPH production via PPP is ATP-independent at the G6PD oxidative reactions — is textbook-correct. But the refinement should acknowledge **indirect ATP coupling via substrate supply**: G6P entry to the PPP requires G6P, which in most tissues is produced by hexokinase/glucokinase (ATP-consuming step: glucose + ATP → G6P + ADP).

**Updated framing:** NADPH production is ATP-independent *at the oxidative PPP reactions themselves* (G6PD, 6PGD) but is coupled to ATP availability *upstream via substrate supply*. In conditions of severe ATP collapse, G6P supply collapses and PPP flux falls despite NADPH-independent catalysis. The dissociability between NADPH and ATP is real at the reaction level but narrower at the systems level.

**Additional NADPH sources:** cytosolic malic enzyme (ME1), cytosolic IDH1, and mitochondrial NNT (Δψ_m-driven transhydrogenation, not ATP-driven). Multi-source production strengthens independence argument.

### 6.2 Δψ_m Dissociation Is Mainly Experimental

**The refinement cited** CCCP/FCCP dissociation of Δψ_m from ATP as demonstration of currency distinctness. Clean at the experimental level. But triangulation flagged:

**Δψ_m dissociation from ATP is primarily experimental (CCCP/FCCP) and per-organelle physiological (mitophagy trigger), not whole-cell steady-state in typical disease.** In most chronic disease states, Δψ_m and cellular ATP fall together because both depend on intact ETC function. The physiological dissociability is narrower than the experimental dissociation suggests.

**Cleaner framing:** The CCCP/FCCP experiments demonstrate that PINK1/Parkin mitophagy is *mechanistically specific* to Δψ_m rather than ATP. This proves biochemical distinctness at the mechanism level. But in disease, the two typically fall together (coupled outputs of failing ETC). Per-organelle dissociation (healthy mitochondria maintain Δψ_m while damaged ones don't) is the relevant physiological context.

### 6.3 Missing Currencies to Include

Two currencies the refinement should include:

**Acetyl-CoA.** Substrate for histone acetyltransferases (HATs) and protein acetylation — direct epigenetic/signaling regulator. Generated by:
- PDH (pyruvate → acetyl-CoA + CO2, mitochondrial)
- β-oxidation (fatty acids → acetyl-CoA, mitochondrial)
- ACLY (citrate → acetyl-CoA + OAA, cytosolic, **ATP-dependent**)

Acetyl-CoA is tightly coupled to both mitochondrial function (PDH, β-oxidation) AND to ATP (ACLY). Wellen et al. 2009 *Science* showed ACLY-dependent histone acetylation links glucose metabolism to gene regulation. Acetyl-CoA is a **genuine currency for epigenetic damping** that was implicit but not explicitly named in the refinement.

**α-Ketoglutarate (broader role).** The refinement mentioned α-KG for HIF hydroxylation. Broader role: α-KG is cofactor for ~70 αKG-dependent dioxygenases including TETs (DNA demethylation), JmjC histone demethylases (histone methylation), and collagen prolyl/lysyl hydroxylases. α-KG/succinate ratio is a key regulator. Carey et al. 2015 *Nature* showed αKG maintains pluripotency via demethylation. Generated from TCA cycle (IDH2/IDH3/IDH1 family).

### 6.4 Clarification: SAM Reinforces ATP-Centrality

**Worth noting:** SAM (S-adenosylmethionine, universal methyl donor) is generated from methionine + **ATP** via methionine adenosyltransferase. So SAM is NOT an independent currency from ATP — it's a methylation-specific ATP-consuming cofactor. Including SAM in the refinement strengthens rather than weakens the ATP-centrality story at the cofactor-synthesis level.

### 6.5 Chubanava 2025 — More Honest Incorporation

Triangulation noted Chubanava 2025 is harder on the NAD+ component than my P3 fully acknowledged: **85% NAD+ depletion in mouse skeletal muscle with preserved function AND preserved mitochondrial respiration.** This is not just about NAD+ tolerance for damping functions — it's about whether ATP production capacity is preserved at 85% NAD+ depletion. If yes, the muscle has large reserve capacity and NAD+ may not be rate-limiting even for ATP generation in muscle at that depletion level.

**Appropriate scope:** NAD+ as independent damping currency is supported in **stressed/disease contexts** where additional factors (CD38 activation, PARP consumption) drive pathologically low NAD+ and sirtuin dysfunction. In healthy muscle with large NAD+ reserve, the independent-currency case is weaker.

### 6.6 Updated Proposed Refinement (Replacing §3.6 / §4.6 Final Formulation)

For **The System.md — State-dependent negative feedback section**:

> "coupled currencies downstream of mitochondrial respiratory capacity — adenylate energy charge (the variable enzymes actually sense via AMPK; Atkinson 1968; Oakhill et al. 2011 *Science*), reductive charge (NADPH via PPP + NNT — ATP-independent at the reactions themselves though indirectly coupled to ATP upstream via glucose-6-phosphate supply; also NAD+/NADH via Complex I), membrane potential Δψ_m (experimentally dissociable from ATP via uncoupling protonophores per PINK1/Parkin biology; in disease typically falls together with ATP), and metabolic epigenetic cofactors (acetyl-CoA for histone acetylation via ACLY/PDH; SAM for methylation via ATP-dependent synthesis; α-KG for TET/JmjC demethylation via TCA flux). Each damping system has system-specific proximal rate-limiting factors. The currencies are biochemically distinct with specific mechanisms but share the mitochondrial respiratory origin — producing correlated but not identical damping system degradation when M fails. The framework's direction is right: mitochondrial competence is the shared upstream variable; ATP alone is too narrow; but 'multiple currencies' refers to coupled outputs of the shared source, not independent causal peers."

### 6.7 Confidence Update

P3 verdict holds with narrower framing:
- Biochemical distinctness of currencies at the reaction level: CONFIRMED
- Genuine whole-cell dissociability under disease steady-state: NARROWER than I initially implied
- The refinement remains a Refinement (specific mechanistic claim about coupled currencies downstream of mitochondrial function), not an overthrow of metabolic centrality
- The core correction — from "ATP as single currency" to "mitochondrial function as shared basis producing coupled currencies" — stands

**No verdict change.** Still Refinement, Peripheral scope.
