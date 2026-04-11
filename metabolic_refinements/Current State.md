# Current State

**Last updated:** 2026-04-11

This is the single canonical source for what is being actively worked on in this project right now. It is small by design and updated as work progresses. Other files (`Stress Test.md`, the refinement documents, `Refinement Diff Catalog.md`) are the substance; this file is the pointer.

If you are a new agent picking this up, read this file first, then follow the "Where to Read for Context" pointers at the bottom.

---

## Where We Are Right Now

**Mid stress test of `metabolic_foundations/`. Layer 2 in progress — 13-loop causal-independence audit Round 1 AND Round 2 COMPLETE.** The audit tool has been applied across all 13 loops by the context-holder (Round 1) and then triangulated via two independent general-purpose agents (Round 2) working from a self-contained research brief with no access to Round 1 classifications. Both Round 2 agents independently confirmed the predicted architectural findings and caught several findings Round 1 missed, including one framework-level citation deployment error. The contracted loop inventory is now ready as the prerequisite substrate for Layer 3.

**Net post-Round-2 architectural count:**
- **9 unambiguously clean closed PFB loops:** L1, L3, L4 (with single-variable structural note), L5, L7-refined, L9 (conditional on Sub-test 2.B), L10, L11, L12
- **1 multi-armed hub (Loop 6)** contracted to 1 clean arm (6c estrogen), 1 gated arm (6d progesterone via estrogen opposition), 1 indeterminate arm (6b serotonin); 2 arms removed (6a parallel marker, 6e not-a-closed-arm)
- **2 structurally half-closed loops** with contradicted or unnamed closure arms: L2 (CF-CI.10, closure direction-reversed by cited source), L8 (CF-CI.8, closure mechanism unnamed)
- **1 periodic external forcing function** (L13, CF-CI.9)

| Layer | Claim under attack | Status |
|---|---|---|
| Layer 0 — Bedrock | ATP requirement, ~18× difference, both pathways real | NOT TESTED (would mean overturning textbook biochemistry) |
| Layer 1 — Ontological move | Health IS efficient oxidative metabolism of glucose to CO₂ | **COMPLETE — REFINEMENT (substantial)** |
| Layer 2 — Product-activity | CO₂ and lactate are active, not inert | **IN PROGRESS** — Sub-test 2.A COMPLETE; causal-independence audit tool triangulated and integrated 2026-04-11; **13-loop audit Round 1 + Round 2 COMPLETE 2026-04-11**; Sub-test 2.B narrowed to mechanism verification only |
| Layer 3 — Attractor dynamics | 13 interlocking loops generate genuine bistability | **READY TO BEGIN.** Audited substrate in place: 9 closed PFB loops + Loop 6 hub (1 clean + 1 gated + 1 indeterminate) + 2 half-closed loops + 1 forcing function. Shared state variables identified (free estrogen, cellular ATP, PUFA, LPS, lactate). Will use MCA loop gain calculations with conservation relations / control coefficients as the quantitative tooling. |
| Layer 4 — Cross-disease convergence | Every chronic disease shows the same metabolic signature | NOT STARTED |
| Layer 5 — Epistemic meta-claim | "The integration is the missing step" | NOT STARTED |
| Layer 6 — Falsifiability meta-test | (subsumed into Verification Methodology Rules 1–3) | SUBSUMED |

Five standalone refinement documents now live in this vault. None have been applied to `metabolic_foundations/` — the original integration is preserved as written, refinements sit beside it as parallel knowledge per the asymmetry principle. The newest is `13-Loop Causal Independence Audit.md`, which is the Round 1 application of the causal-independence audit tool to the framework's full loop architecture.

---

## What Just Happened

**Most recent substantive move (2026-04-11, late evening):** The 13-loop causal-independence audit Round 2 triangulation has been completed. Two independent general-purpose agents were dispatched in parallel per `Independent Agent Research Protocol.md`, each given the same self-contained research brief (`Research Brief - 13 Loop Causal Independence Audit.md`) without access to Round 1 classifications. Both reports were then critically assessed against first principles, with load-bearing corrections verified directly against primary sources (WebFetch). The synthesis has been transcribed into `13-Loop Causal Independence Audit.md` as a new "Round 2 Triangulation Synthesis" section, and the one-shot artifacts (brief, agent reports) are being deleted per the Protocol's housekeeping rules.

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

### The plan (current position: 13-loop audit Round 1 complete; Round 2 triangulation is the immediate next move)

1. ✅ **Articulate the causal-independence audit tool as a standalone document.** DONE.
2. ✅ **Triangulate the audit tool via two independent agents.** DONE.
3. ✅ **Verify sAC counterexample against primary sources.** DONE.
4. ✅ **Rewrite and rename the document.** DONE — `Causal Independence in Feedback Loops.md`.
5. ✅ **Integrate the refined audit into `metabolic_foundations/Verification Methodology.md` Step 4.** DONE 2026-04-11. Second methodology improvement from Sub-test 2.A (first was CF-2.A.4).
6. ✅ **Run the causal-independence audit across all 13 formalized loops in `The System.md`** using the refined four-check operational audit. DONE 2026-04-11 — `13-Loop Causal Independence Audit.md`. Produced a classified inventory with one section per loop, top-level inventory table, cross-loop findings, and architectural impact summary.
7. ✅ **Run the citation deployment audit (CF-2.A.4) across all 13 loops** in the same pass. DONE 2026-04-11 — included in `13-Loop Causal Independence Audit.md`. No new mis-deployments at the load-bearing level beyond what was already documented in Sub-test 2.A and existing warning callouts.
8. ✅ **Triangulate the audited loop inventory** via independent agents (Round 2 triangulation). DONE 2026-04-11. Two independent general-purpose agents dispatched in parallel per `Independent Agent Research Protocol.md`, each given `Research Brief - 13 Loop Causal Independence Audit.md` with no access to Round 1 classifications. Both reports critically assessed against first principles; load-bearing corrections verified against primary sources via WebFetch. Synthesis transcribed into `13-Loop Causal Independence Audit.md`'s new "Round 2 Triangulation Synthesis" section.
9. ✅ **Synthesize Round 2 findings.** DONE 2026-04-11. Strong convergence on predicted findings; meaningful additions from Round 2 (cross-loop convergence nodes, Loop 6d downgrade, Loop 4 structural note, Loop 2 closure direction-reversal via CF-CI.10, Loop 4 single-variable structural note via CF-CI.11, and four brief-level factual corrections). `13-Loop Causal Independence Audit.md` updated with updated top-level inventory table, consolidated Round 2 synthesis section, new carry-forward items, updated architectural impact summary. Stress Test.md working log and carry-forward items updated. Current State.md updated.
10. **Clean up one-shot artifacts (IMMEDIATE NEXT STEP — pending).** Per `Independent Agent Research Protocol.md` Phase 5: delete `Research Brief - 13 Loop Causal Independence Audit.md`, `agent_1_round2_report.md`, `agent_2_round2_report.md`. Git history preserves them. The durable form is the Round 2 Synthesis section in the audit document and the working log entry in Stress Test.md.
11. **Commit the Round 1 + Round 2 audit state.** Pending. One commit covering the audit document (Round 1 + Round 2 consolidated), Stress Test.md working log + carry-forward items, Current State.md updates, and the artifact cleanup.
12. **Sub-test 2.B (narrowed) — verify histone lactylation is causal in vivo** for Loop 9's gene expression effects vs. an HIF-1α correlate. The audit resolved the structural causal-independence question; what remains is mechanism verification only. Can be run before, alongside, or after Layer 3.
13. **Layer 3 — formal bistability via MCA loop gain calculations** on the Round-2-finalized inventory (9 closed PFB + hub + 2 half-closed + forcing function). The audit's classified inventory is the prerequisite substrate and is now in place. Layer 3 is the most consequential remaining layer. Must handle: closed PFB loops with standard loop gain; the multi-armed Loop 6 hub; the 2 half-closed loops (L2 direction-reversed closure, L8 unnamed closure) whose closure-step loop gain cannot be computed until CF-CI.10 and CF-CI.8 resolve; the Loop 13 forcing function modeled as external drive not as a closed loop; and the shared state variables (free estrogen, ATP, PUFA, LPS, lactate) where contributions are additive without double-counting.
14. **Consider Loop 2 refinement document.** CF-CI.10 surfaced a framework-level citation deployment error analogous to Sub-test 2.A's Loop 7 finding. A Loop 2 refinement document mirroring `Loop 7 — Metabolism-Mediator Coupling.md`'s structure is the natural next output — documents the finding, proposes the central-5-HT salvage mechanism if supporting literature exists, updates the Refinement Diff Catalog. Lower priority than Layer 3 but a natural follow-up if the framework text needs an explicit companion refinement.

### Housekeeping pending

- `Research Brief - 13 Loop Causal Independence Audit.md` should be deleted (one-shot artifact per Independent Agent Research Protocol) once the Round 2 synthesis is committed to durable form. **Durable form already in place:** the Round 2 Synthesis section in `13-Loop Causal Independence Audit.md` and the 2026-04-11 Round 2 working log entry in `Stress Test.md`.
- `agent_1_round2_report.md` and `agent_2_round2_report.md` should be deleted once the Round 2 synthesis is committed.
- (The prior `Research Brief - Co-Production Principle.md`, `agent_1_report.md`, `agent_2_report.md` from the Round 1 audit-tool triangulation were already deleted after that round's completion.)
- Git history will preserve all Round 2 artifacts for future reference.

### After the audit (Layer 3 and beyond, in rough order of leverage)

1. **Layer 3 — Attractor architecture as genuine dynamics.** The most consequential remaining layer and the reason the Layer 2 audit exists as a prerequisite. Tests whether the (now-audited) loop architecture is real dynamical-systems bistability or a precise metaphor for clinical bimodality. The loop-gain question CF-2.A.2 (do any of the directional couplings actually achieve loop gain > 1?) gets formally tested here, likely using MCA control coefficients as the tooling. **If Layer 3 fails, the "two attractors" framing collapses to metaphor — the largest possible finding of the stress test.**
2. **Resolve CF-2.A.5** — independent verification of Bolevich & Kogan 2016 (the strongest remaining "CO₂ as active protector" non-loop claim). Required before the broader Foundation.md / Metabolic Fork.md "CO₂ is an active product" reframing can proceed.
3. **Layer 4 — Cross-disease convergence.** Tests the strongest external prediction. Are there chronic diseases that genuinely don't fit the metabolic failure signature?
4. **Layer 5 — Epistemic meta-claim.** Tests whether "the integration is the missing step" survives engagement with what systems biology and integrative physiology have already concluded.

### After the audit (Layer 3 and beyond, in rough order of leverage)

1. **Layer 3 — Attractor architecture as genuine dynamics.** The most consequential remaining layer and the reason the Layer 2 audit exists as a prerequisite. Tests whether the (now-audited) loop architecture is real dynamical-systems bistability or a precise metaphor for clinical bimodality. The loop-gain question CF-2.A.2 (do any of the directional couplings actually achieve loop gain > 1?) gets formally tested here. **If Layer 3 fails, the "two attractors" framing collapses to metaphor — the largest possible finding of the stress test.**
2. **Resolve CF-2.A.5** — independent verification of Bolevich & Kogan 2016 (the strongest remaining "CO₂ as active protector" non-loop claim). Required before the broader Foundation.md / Metabolic Fork.md "CO₂ is an active product" reframing can proceed.
3. **Layer 4 — Cross-disease convergence.** Tests the strongest external prediction. Are there chronic diseases that genuinely don't fit the metabolic failure signature?
4. **Layer 5 — Epistemic meta-claim.** Tests whether "the integration is the missing step" survives engagement with what systems biology and integrative physiology have already concluded.

---

## What's Blocking

**Nothing is blocking active work.** Sub-test 2.B can begin immediately.

Several open questions require literature that doesn't currently exist and are flagged rather than chased:
- **CF-1.B.1** — Free T3 adaptive vs pathological in adapted keto (needs tissue-level T3 signaling data)
- **CF-1.B.4** — Full-panel metabolic-ward crossover study in adapted keto cohorts on framework metrics
- **CF-2.A.2** — Loop gain quantification at physiological ATP variations
- **CF-2.A.3** — Direct in vivo hypocapnic challenge with mediator measurement in humans

See `Stress Test.md` → "Carry-Forward Items" for full list.

---

## Active Decisions Pending Review

**One pending decision: whether the architectural recommendations from the 13-loop audit (CF-CI.1 confirmed; sub-arms 6a and 6e removed; Loop 13 reclassified as periodic forcing function) should be acted on at the `The System.md` level.** Per the asymmetry principle and this vault's role, the framework's text in `metabolic_foundations/` is preserved as-is; the audit findings live in `13-Loop Causal Independence Audit.md` as parallel knowledge. No edit to `The System.md` is being proposed. The Round 2 triangulation will inform whether the architectural findings should also be reflected in any way that crosses the vault boundary.

The Refinement Diff Catalog exists in this vault as the precise file/passage-level reference for what each refinement consists of, but it is **not going to be applied** to `metabolic_foundations/` — that decision has been made (the refinements live in this vault as parallel knowledge instead).

Two edits have been applied to `metabolic_foundations/` from the entire stress test so far. Both are methodology improvements, not claim changes:

1. **CF-2.A.4** — citation deployment audit added to `metabolic_foundations/Verification Methodology.md` Step 5 (2026-04-10). Checks load-bearing citations on species / scenario / endpoint / proposed-mechanism match.
2. **Causal independence audit** — added to `metabolic_foundations/Verification Methodology.md` Step 4 (2026-04-11). Four-check operational audit grounded in Pearl's screening-off test and MCA conservation relations. Classifies metabolites named as causal drivers into six categories (independent driver / parallel marker / gated driver / co-driver / indeterminate). Triangulated via two independent agents before integration; sAC verified against primary sources.

Both methodology improvements emerged from a single sub-test (2.A) and apply to every future verification rather than to one claim — higher total leverage than individual claim refinements. The 13-loop audit Round 1 (2026-04-11) is the first major application of the methodologized causal-independence audit to the framework's loop architecture, and it confirmed the audit's predictive value: CF-CI.1 was correctly anticipated in the audit tool's sample classifications and held under the full pass.

---

## Where to Read for Context

If you are picking this up and need to understand the full state, read in this order:

### 1. Project orientation
- `CLAUDE.md` (workspace root) — three-vault structure, the asymmetry principle
- `Overview.md` (workspace root) — full project narrative

### 2. This vault's structure
- `metabolic_refinements/CLAUDE.md` — vault purpose, conventions, refinement document template, status semantics

### 3. Active stress test state
- `Stress Test.md` (this vault) — the live investigation log. Read in full for first-time pickup. Sections to focus on: Strategy, Protocol, Layer 1, Layer 2, Carry-Forward Items, Working Log
- `Refinement Diff Catalog.md` (this vault) — the diff-form catalog. Skim for understanding of the precise file/passage-level changes each refinement represents
- `Independent Agent Research Protocol.md` (this vault) — required reading before running any sub-test that will use independent agent triangulation. Both completed substantive sub-tests (1.B and 2.A) used this methodology; Sub-test 2.B is expected to use it as well. Specifies when to use it, how to construct self-contained briefings, how to critically assess agent outputs, how to handle convergence vs divergence.

### 4. Substantive findings as standalone knowledge
- `Convergence Point Reading.md` (this vault) — Sub-test 1.A
- `Krebs-Cycle Invariance and Ketone Bodies.md` (this vault) — Sub-test 1.B (six findings consolidated)
- `Loop 7 — Metabolism-Mediator Coupling.md` (this vault) — Sub-test 2.A
- `Causal Independence in Feedback Loops.md` (this vault) — the causal-independence audit *tool* derived from Sub-test 2.A, grounded in Pearl's screening-off + Palsson/MCA conservation relations. Supersedes the earlier first-pass `Co-Production and Independence.md` which was deleted after triangulation identified it as over-general and a re-derivation of existing work.
- **`13-Loop Causal Independence Audit.md`** (this vault) — the Round 1 *application* of the audit tool to all 13 formalized positive feedback loops in `The System.md`. Includes per-loop sections, top-level inventory table, cross-loop findings, citation deployment summary, new carry-forward items (CF-CI.7, 8, 9), and architectural impact summary. This is the prerequisite substrate for Layer 3's formal bistability test.

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
7892aba  Add causal independence audit to Verification Methodology Step 4
eb9f637  Add Causal Independence audit tool — triangulated refinement of Sub-test 2.A
47e4be0  Remove drifting content-volume metadata from orientation files
3e6d3dd  Correct stale word count in Methodology.md
b2156b9  Correct stale word counts across orientation files
08bd281  Remove reading-time estimates — not relevant or accurate
8e17a4b  Rename Vault Edit Proposal.md → Refinement Diff Catalog.md
db1dc19  Post-implementation review fixes — close orphan and discoverability gaps
f48c04a  Add Current State.md as canonical live-state file for active work
6112d5b  Create metabolic_refinements vault — refinements layer separate from the original integration
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
