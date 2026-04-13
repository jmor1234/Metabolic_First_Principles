# Current State

**Last updated:** 2026-04-12 (end of session)

This is the single canonical source for what is being actively worked on in this project right now. It is small by design and updated as work progresses. Other files (`Stress Test.md`, the refinement documents, `Refinement Diff Catalog.md`) are the substance; this file is the pointer.

If you are a new agent picking this up, read this file first, then follow the "Where to Read for Context" pointers at the bottom.

---

## Where We Are Right Now

**The truth-seeking phase of the project is COMPLETE.** The stress test (Layers 1-3), the mechanism citation audit (all 9 documents), and 5 corrections to mechanism documents are all done. The framework is verified at both the structural and mechanism levels. The synthesis document (`The Integrated Framework.md` in workspace root) presents the complete current understanding.

**The next phase is building the application layers** — the bridge from "what is true about biology" to "what does this specific person do to be healthier." See "What's Next" below.

**Verification status across the full stack:**

| Level | What it covers | Status |
|---|---|---|
| Structural architecture (Layers 1-3) | Ontological claim, product-activity, bistability | **Stress-tested, triangulated, empirically confirmed.** All REFINEMENT. |
| Mechanism documents (9 docs) | Detailed biochemistry of each component | **Citation-audited (221 citations). 4 confirmed errors corrected in vault. 73% clean, 11% flagged.** |
| Synthesis | The complete current understanding | **`The Integrated Framework.md` written. Single standalone read.** |
| Traceability | How we got here | **3 source vaults + Stress Test Summary + Mechanism Citation Audit + refinement documents. Full chain preserved.** |
| Assessment protocol | "Where is THIS person in the system?" | **NOT DONE — this is the next build.** |
| Intervention framework | "What does THIS person do?" | **PARTIALLY DONE.** Practice.md exists but is pre-stress-test. Needs conditional bistability, slow/fast variable prioritization, state-dependent damping. |
| Agent protocol | "How does a human-AI pair use this?" | **NOT DONE.** |

Seven standalone documents in this vault: 6 refinement documents + Stress Test Summary + Mechanism Citation Audit. Five corrections have been applied directly to `metabolic_foundations/`: 2 methodology improvements (citation deployment audit, causal-independence audit) and 3 claim corrections (rT3 mechanism, Ringer's citation, Ca+VitD mixed evidence, PTH dose qualifier, LPS/D2 nuance).

---

## What Just Happened

**2026-04-12 session completed the entire truth-seeking phase:**

1. **Layer 3 formal bistability analysis** — REFINEMENT (substantial), triangulated. The "two attractors" is genuine dynamics, conditional on parameter values. Six new predictions, two already observed in clinical data (hysteresis via bariatric surgery, CSD via Tabák longitudinal cohorts).
2. **Sub-test 2.B** — PASS. Lactylation causally validated. Loop 9 conditional resolved. M-Λ toggle confirmed.
3. **CSD empirical check** — critical slowing down and hysteresis signatures found in existing clinical data (Tabák et al., bariatric surgery remission).
4. **Layer 3 refinement document** — `Conditional Bistability and Attractor Dynamics.md` written with empirical confirmation section.
5. **Stress Test Summary** — precise before/after accounting of all findings.
6. **The Integrated Framework** — single synthesis document in workspace root presenting the complete current understanding.
7. **Mechanism citation audit** — all 9 mechanism documents audited (221 load-bearing citations). 73% clean, 11% flagged, 4 confirmed errors.
8. **5 corrections applied to metabolic_foundations/** — rT3 mechanism, Ringer's citation, Ca+VitD mixed evidence, PTH dose qualifier, LPS/D2 nuance.

**The stress test is complete.** All three core layers tested (all REFINEMENT). All 9 mechanism documents citation-audited. Confirmed errors corrected. The knowledge is verified at both structural and mechanism levels.

**Round 2 outcome — strong convergence on predicted findings, plus meaningful additions:**

*Confirmed by both agents independently (matching Round 1's predictions):*
1. **CF-CI.1 CONFIRMED.** Loop 6 sub-arm 6a (low T3 → low CO₂ → ↓T3) is a parallel marker via matching first-principles reasoning — no named CO₂-specific mechanism at any thyroid-axis protein; ATP has specific mechanisms everywhere. After this round, **no formalized loop in the framework has CO₂ as a mechanism-named independent causal driver.**
2. **Loop 13 reclassified** as a periodic external forcing function with state-dependent recovery deficit, not a closed PFB loop in the dynamical-systems sense. Both agents used the same dynamical-systems language and reached the same reclassification independently without prompting from the brief.
3. **Loop 8 closure arm flagged (CF-CI.8)**, **Loop 6b indeterminate (CF-CI.7)**, **Loop 6e not-a-closed-arm removed**, **Loop 9 structural pass**, **Loop 12 cleanest intervention-tested loop** — all confirmed.
4. **CO₂/lactate structural asymmetry held** across the full audit pass under independent reasoning.

*Findings Round 1 missed that Round 2 caught (both agents):*
5. **Cross-loop convergence at shared state variables.** Round 1 only had the L6c/L11 overlap at estrogen. Round 2 identified: free estrogen (L5, L6c, L8, L11), cellular ATP (L1, L7, L10), PUFA pool (L1, L2, L3), LPS (L10, L11, L12), potentially lactate (L9 + L8 closure). Shared state variables are additive in Layer 3 loop gain calculations and must not be double-counted.
6. **Loop 6d downgrade** from independent driver (Round 1) to **gated** (Round 2) — the return arm operates via estrogen opposition, not a direct progesterone-receptor-to-thyroid-axis mechanism. Loop 6 contracts further than Round 1 claimed: only sub-arm 6c (estrogen via TBG) is cleanly independent.
7. **Loop 4 structural note (CF-CI.11)** — it is a single-variable autoregulatory production loop, not a two-variable interlocked loop. Matters for Layer 3 loop gain formulation.

*Biggest Round 1 miss (Agent 1 alone, verified against primary source):*
8. **Loop 2 closure arm is direction-reversed by its cited source (CF-CI.10).** `Membrane Damage and Defense.md` cites PMC6624793 for "serotonin promotes lipolysis." WebFetch verification confirms the paper explicitly reports peripheral 5-HT via HTR2A *suppresses* isoprenaline-induced lipolysis, and HTR2B modestly reduces basal lipolysis — the paper's conclusion is that peripheral serotonin promotes "an energy storage phenotype" by suppressing lipolysis. **Loop 2's closure arm does not close as cited.** This is the second framework-level citation deployment error found by the stress test (first was Pollard 1977 / Freed 2001 for Loop 7 in Sub-test 2.A). Pattern: citation deployment errors cluster in loops where the mechanism is named at the bulk-effect / non-molecular level.

*Brief-level factual corrections verified against primary sources (WebFetch 2026-04-11):*
- **Mathur 2025 "0.33×" is fabricated.** ENDO 2025 press release states "mitigated" without a specific reduction multiplier. The 0.33× does not appear anywhere in the press release. Brief-authoring error, not framework error. Directional claim preserved.
- **PMC4056127 percentages wrong.** Primary source (Patil 2014 citing Lauritano 2007 JCEM) reports 54% hypothyroid vs 5% control, not 32.65%/15.17% as the brief stated. The brief conflated Lauritano's original prevalence cohort with Mathur's 2.2-2.4× EHR cohort risk ratio.
- **PMID 17925093 first author is Kaplan, not Chen.** Cosmetic.
- **PMID 17077193 abstract does not contain the 8×/320× peroxidation rate ratios** — those come from the peroxidation index framework (Holman 1954; Cosgrove 1987). Citation source error only.
- **Agents disagreed on the PMC4056127 verification.** Agent 1 claimed clean; Agent 2 said mismatched. Primary-source check (WebFetch) resolved in favor of Agent 2. This validates the Protocol's Phase 3 rule: don't accept agent verifications without checking primary sources.

**Net architectural impact** (see layer status table above): the framework's nominal 13 loops contract to 9 clean + 1 hub + 2 half-closed + 1 forcing function. Substance preserved; architectural precision substantially increased.

**Meta-finding:** the Round 2 triangulation worked exactly as the Independent Agent Research Protocol predicted — predicted findings converged under independent reasoning (not confirmation bias); agents caught findings the context-holder missed (not rubber-stamping); disagreements between agents on specific verifications were resolved by primary-source checks (first principles > consensus); brief-level errors were caught and corrected before they could propagate. The Protocol's design premise held.

**Prior substantive moves:**
- **Round 1 13-loop audit (2026-04-11 afternoon/evening):** Applied the audit tool across all 13 loops by the context-holder, producing the initial classified inventory.
- **Causal-independence audit tool refinement (2026-04-11 afternoon):** Triangulated the audit tool itself via two independent agents, refined from a universal "stoichiometric coupling → parallel marker" rule to Pearl's screening-off test + MCA conservation relations with a four-check operational audit. Current standalone document: `Causal Independence in Feedback Loops.md`. Integrated into Verification Methodology Step 4 the same day.

**The triangulation outcome:** Both agents independently classified the first-pass principle as **Refinement**. Both independently identified that the concept is a partial re-derivation of established work — specifically **conservation relations / left null space of the stoichiometric matrix in Metabolic Control Analysis** (Reder 1988; Heinrich & Schuster 1996; Palsson 2003) and **Pearl's do-calculus / screening-off test** from causal inference (Pearl 2000, 2009). Both independently identified **AMP/AMPK as a counterexample** (AMP is in the conserved adenylate pool with ATP but is a genuine causal participant because AMPK γ-subunit CBS domains are AMP-specific). Agent 1 additionally identified **soluble adenylyl cyclase (sAC) / bicarbonate / OXPHOS** as a counterexample specific to the CO₂/OXPHOS case (Acin-Perez 2009 *Cell Metabolism*; Valsecchi 2014 *BBA* PMC4257896; Kleinboelting 2014 crystal structures). The sAC counterexample was verified against primary sources via WebFetch — bicarbonate is confirmed as the specific allosteric activator via Arg176 with salt bridge disruption and active-site closure; ATP functions as substrate not allosteric activator; the pathway is carbonic-anhydrase-dependent and experimentally dissociable from ATP. Important caveat: Valsecchi 2014 frames the sAC-OXPHOS pathway as feedforward metabolic matching rather than closed positive feedback, which narrows the counterexample's directness but preserves its core structural point.

**The rewrite addresses all three problems:** (1) grounded in existing frameworks with explicit citations; (2) the universal "only if" form replaced with a four-check operational audit (conservation, mechanism specificity, realizable intervention, quantitative dominance); (3) the three-category taxonomy expanded to six (adding gated driver, co-driver, and splitting independent driver into specific-mechanism vs quantitative-dominance). The refined audit correctly classifies Loop 7 original (parallel marker), Loop 7 refined (independent driver), Loop 9 lactate (independent driver, conditional on mechanism verification), and the sAC case (independent driver, but not a closed loop in the framework's current architecture).

**The pre-specified CO₂/lactate asymmetry prediction survived triangulation.** CO₂ is stoichiometrically tied to OXPHOS; lactate is tied to the metabolic-fork failure mode. Both agents confirmed the structural asymmetry with matching reasoning.

**Rationale for the pivot held up:** the stress test was right to triangulate the audit tool before methodologizing it. If the first-pass principle had been added to Verification Methodology directly, it would have introduced a universal rule that is falsified by known biology (sAC, AMPK) and that duplicates existing work without citing it. Triangulation caught this cleanly — exactly what the Independent Agent Research Protocol was designed to do.

**Prior substantive finding (2026-04-10):** Sub-test 2.A — Loop 7 mechanism refinement. The framework's stated mechanism (extracellular CO₂ → carbonic acid → granule pH → mediator release) is first-principles incompatible with V-ATPase biology. The refined mechanism is **ATP → V-ATPase activity → granule pH → V₁-V₀ sensor → mediator release**. CO₂ becomes a parallel marker of oxidative metabolism rather than the causal driver. Two independent agents converged on the *identical* rescue mechanism via matching first-principles reasoning. Loop 7 was the only formalized loop in the 13-loop architecture where CO₂ was the causal driver; after this refinement, no formalized loop has CO₂ as causal variable.

**Most recent project action (2026-04-11):** `Causal Independence in Feedback Loops.md` written; `Co-Production and Independence.md` deleted (superseded). `metabolic_foundations/` was not modified.

---

## What's Next

### The plan (current position: truth-seeking COMPLETE; application layers are next)

**The overall goal:** An integrated knowledge system, built on verified first-principles truth, usable by a human-AI pair, that goes from thermodynamics all the way to "what does this specific person do to be healthier" — and that enables further refinement through use.

**What's next — the application layers, in order:**

1. **Assessment protocol (IMMEDIATE NEXT BUILD).** A structured protocol that maps a person's context (symptoms, labs, history, lifestyle) onto the framework's 6 state variables (M, T, E, P, L, Λ). Determines: which loops are engaged, whether the person is monostable (perturbations return to health) or bistable (trapped in disease basin), and what their slow variables (PUFA burden, mitochondrial function) vs fast variables (T₃, LPS, lactate) look like. Uses critical slowing down metrics (recovery dynamics from standardized stressors) as regime assessment. **Must be built before interventions can be properly recommended.**

2. **Updated intervention framework.** Practice.md exists in `metabolic_foundations/` but needs updating with: conditional bistability (different strategy for monostable vs bistable regime), slow-variable vs fast-variable prioritization (slow resets are more durable), state-dependent damping as highest leverage (restore the self-correcting machinery), CO₂ reclassification (readout to monitor, not mechanism to target), and critical slowing down as a monitoring metric.

3. **Agent protocol.** A structured decision process an AI agent follows when working with a specific person: take context → assess regime → map onto state variables → identify engaged loops → recommend interventions in leverage order → monitor with framework metrics → refine based on response. Not a chatbot script — a decision protocol with traceability back to the evidence chain. Designed so that errors in mechanism documents surface through use and get corrected via the Verification Methodology.

**Lower priority (can be done during or after application layer build):**
- Resolve CF-2.A.5 (Bolevich & Kogan independent verification)
- Species qualifiers for ~12 mechanism citations
- Citations for ~18 currently unsupported specific claims
- Layers 4-5 of the stress test (diminishing returns — the bedrock is tested)

---

## What's Blocking

**Nothing is blocking.** The application layer build can begin immediately. All prerequisite truth-seeking work is complete.

Open carry-forward items from the stress test (see `Stress Test.md` → "Carry-Forward Items" for full list) are flagged for future resolution but do not block the application layer work. Most require experimental data that doesn't currently exist.

---

## Edits applied to metabolic_foundations/

Seven total edits have been applied from the entire project:

**Methodology improvements (2):**
1. CF-2.A.4 — citation deployment audit added to Verification Methodology Step 5 (2026-04-10)
2. Causal independence audit added to Verification Methodology Step 4 (2026-04-11)

**Claim corrections from mechanism citation audit (5, applied 2026-04-12):**
3. rT3 mechanism corrected from "blocks T3 at nuclear receptors" to "competitively inhibits DIO1" (The Master Throttle)
4. LPS/D2 nuance added — central hypothyroidism via paradoxical hypothalamic D2 activation (The Master Throttle)
5. Ringer's lactate citation replaced with correct paper (The Metabolic Fork)
6. Ca+VitD fracture claim updated to reflect mixed evidence (The Cellular Readout)
7. PTH mast cell dose and species qualifiers added (The Cellular Readout)

---

## Where to Read for Context

If you are picking this up and need to understand the full state, read in this order:

### 1. Project orientation
- `CLAUDE.md` (workspace root) — three-vault structure, the asymmetry principle
- `Overview.md` (workspace root) — full project narrative

### 2. This vault's structure
- `metabolic_refinements/CLAUDE.md` — vault purpose, conventions, refinement document template, status semantics

### 3. What was found
- `Stress Test Summary.md` (this vault) — **start here for findings.** Precise before/after accounting.
- `Mechanism Citation Audit.md` (this vault) — citation audit results across all 9 mechanism documents.
- `Stress Test.md` (this vault) — the full investigation log. Layer-by-layer detail, carry-forward items, working log.
- `Refinement Diff Catalog.md` (this vault) — the diff-form catalog of precise file/passage-level changes.
- `Independent Agent Research Protocol.md` (this vault) — required reading before running any sub-test that will use independent agent triangulation. Both completed substantive sub-tests (1.B and 2.A) used this methodology; Sub-test 2.B is expected to use it as well. Specifies when to use it, how to construct self-contained briefings, how to critically assess agent outputs, how to handle convergence vs divergence.

### 4. Substantive findings as standalone knowledge
- **`Stress Test Summary.md`** (this vault) — **start here for findings.** Precise before/after accounting of what the framework got right, wrong, and what was missing. The capstone.
- `Convergence Point Reading.md` (this vault) — Sub-test 1.A
- `Krebs-Cycle Invariance and Ketone Bodies.md` (this vault) — Sub-test 1.B (six findings consolidated)
- `Loop 7 — Metabolism-Mediator Coupling.md` (this vault) — Sub-test 2.A
- `Causal Independence in Feedback Loops.md` (this vault) — the causal-independence audit *tool* derived from Sub-test 2.A, grounded in Pearl's screening-off + Palsson/MCA conservation relations. Supersedes the earlier first-pass `Co-Production and Independence.md` which was deleted after triangulation identified it as over-general and a re-derivation of existing work.
- **`13-Loop Causal Independence Audit.md`** (this vault) — the Round 1 + Round 2 application of the audit tool to all 13 formalized positive feedback loops in `The System.md`. Includes per-loop sections, top-level inventory table, cross-loop findings, citation deployment summary, carry-forward items, and architectural impact summary. This was the prerequisite substrate for Layer 3.
- **`Conditional Bistability and Attractor Dynamics.md`** (this vault) — Layer 3. The framework's "two attractors" is genuine dynamics, not metaphor, but conditional on parameter values. State-dependent negative feedback, Brandman coupling, six new testable predictions. Source: Stress Test Layer 3.

### 5. Framework context
Only read if not already familiar with the metabolic_foundations framework being attacked:
- `metabolic_foundations/CLAUDE.md` — vault structure, navigation strategy
- `metabolic_foundations/Foundation.md` — the thesis and first-principles argument
- `metabolic_foundations/The System.md` — the architecture, two attractors, 13 feedback loops

### 6. Methodology
Required reading before attempting any new sub-test or proposing any change:
- `metabolic_foundations/Verification Methodology.md` — the discipline. Three Hypotheses, Six-Step Verification Sequence, Three Rules, Default Position, citation deployment audit (CF-2.A.4 addition).

### 7. Per-vault navigation (as needed)
- `peat_claims_verified/CLAUDE.md` — only if you need to trace something back to the original Peat verification audit trail.

---

## Recent Commits

Most recent at top. Run `git log --oneline -20` for full history.

```
641c481  Stop tracking .obsidian/ config files — local editor state, not project content
ab372d2  Complete 13-loop causal independence audit — Round 1 + Round 2 triangulation
9fc7484  Documentation maintenance — close cold-start gaps after audit tool work
7892aba  Add causal independence audit to Verification Methodology Step 4
eb9f637  Add Causal Independence audit tool — triangulated refinement of Sub-test 2.A
47e4be0  Remove drifting content-volume metadata from orientation files
```

---

## Updating This File

Update this file whenever:
- A sub-test starts, advances, or completes
- A new finding lands
- The "next move" changes
- A blocker appears or resolves
- A pending decision changes status
- A significant commit lands

Keep it small. If a section grows beyond a few paragraphs, the substance belongs in `Stress Test.md` or a refinement document, not here. This file's job is to be the *pointer*, not the substance.
