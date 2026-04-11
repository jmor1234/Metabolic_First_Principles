# Current State

**Last updated:** 2026-04-11

This is the single canonical source for what is being actively worked on in this project right now. It is small by design and updated as work progresses. Other files (`Stress Test.md`, the refinement documents, `Refinement Diff Catalog.md`) are the substance; this file is the pointer.

If you are a new agent picking this up, read this file first, then follow the "Where to Read for Context" pointers at the bottom.

---

## Where We Are Right Now

**Mid stress test of `metabolic_foundations/`. Layer 2 in progress — causal-independence audit tool now triangulated and rewritten.** The deeper implication of Sub-test 2.A's Loop 7 finding (CO₂ and ATP are stoichiometrically co-produced by OXPHOS) was promoted to an architecture-level principle, stress-tested via two independent agents, substantially refined, and re-grounded in existing formal machinery (Pearl's screening-off test + Palsson's conservation relations in MCA). The refined audit is now ready to run across all 13 loops.

| Layer | Claim under attack | Status |
|---|---|---|
| Layer 0 — Bedrock | ATP requirement, ~18× difference, both pathways real | NOT TESTED (would mean overturning textbook biochemistry) |
| Layer 1 — Ontological move | Health IS efficient oxidative metabolism of glucose to CO₂ | **COMPLETE — REFINEMENT (substantial)** |
| Layer 2 — Product-activity | CO₂ and lactate are active, not inert | **IN PROGRESS** — Sub-test 2.A COMPLETE; causal independence audit tool triangulated and ready; 13-loop audit pending; Sub-test 2.B deferred pending audit |
| Layer 3 — Attractor dynamics | 13 interlocking loops generate genuine bistability | NOT STARTED (prerequisite: clean audited loop inventory from Layer 2 audit) |
| Layer 4 — Cross-disease convergence | Every chronic disease shows the same metabolic signature | NOT STARTED |
| Layer 5 — Epistemic meta-claim | "The integration is the missing step" | NOT STARTED |
| Layer 6 — Falsifiability meta-test | (subsumed into Verification Methodology Rules 1–3) | SUBSUMED |

Four refinements have landed so far. All are documented as standalone refinement documents in this vault. None have been applied to `metabolic_foundations/` — the original integration is preserved as written, refinements sit beside it as parallel knowledge per the asymmetry principle.

---

## What Just Happened

**Most recent substantive move (2026-04-11, afternoon):** The causal-independence audit tool has been triangulated via two independent agents, substantially refined, and rewritten. Current standalone document: **`Causal Independence in Feedback Loops.md`**. The earlier first-pass document (`Co-Production and Independence.md`) was superseded and deleted.

**The triangulation outcome:** Both agents independently classified the first-pass principle as **Refinement**. Both independently identified that the concept is a partial re-derivation of established work — specifically **conservation relations / left null space of the stoichiometric matrix in Metabolic Control Analysis** (Reder 1988; Heinrich & Schuster 1996; Palsson 2003) and **Pearl's do-calculus / screening-off test** from causal inference (Pearl 2000, 2009). Both independently identified **AMP/AMPK as a counterexample** (AMP is in the conserved adenylate pool with ATP but is a genuine causal participant because AMPK γ-subunit CBS domains are AMP-specific). Agent 1 additionally identified **soluble adenylyl cyclase (sAC) / bicarbonate / OXPHOS** as a counterexample specific to the CO₂/OXPHOS case (Acin-Perez 2009 *Cell Metabolism*; Valsecchi 2014 *BBA* PMC4257896; Kleinboelting 2014 crystal structures). The sAC counterexample was verified against primary sources via WebFetch — bicarbonate is confirmed as the specific allosteric activator via Arg176 with salt bridge disruption and active-site closure; ATP functions as substrate not allosteric activator; the pathway is carbonic-anhydrase-dependent and experimentally dissociable from ATP. Important caveat: Valsecchi 2014 frames the sAC-OXPHOS pathway as feedforward metabolic matching rather than closed positive feedback, which narrows the counterexample's directness but preserves its core structural point.

**The rewrite addresses all three problems:** (1) grounded in existing frameworks with explicit citations; (2) the universal "only if" form replaced with a four-check operational audit (conservation, mechanism specificity, realizable intervention, quantitative dominance); (3) the three-category taxonomy expanded to six (adding gated driver, co-driver, and splitting independent driver into specific-mechanism vs quantitative-dominance). The refined audit correctly classifies Loop 7 original (parallel marker), Loop 7 refined (independent driver), Loop 9 lactate (independent driver, conditional on mechanism verification), and the sAC case (independent driver, but not a closed loop in the framework's current architecture).

**The pre-specified CO₂/lactate asymmetry prediction survived triangulation.** CO₂ is stoichiometrically tied to OXPHOS; lactate is tied to the metabolic-fork failure mode. Both agents confirmed the structural asymmetry with matching reasoning.

**Rationale for the pivot held up:** the stress test was right to triangulate the audit tool before methodologizing it. If the first-pass principle had been added to Verification Methodology directly, it would have introduced a universal rule that is falsified by known biology (sAC, AMPK) and that duplicates existing work without citing it. Triangulation caught this cleanly — exactly what the Independent Agent Research Protocol was designed to do.

**Prior substantive finding (2026-04-10):** Sub-test 2.A — Loop 7 mechanism refinement. The framework's stated mechanism (extracellular CO₂ → carbonic acid → granule pH → mediator release) is first-principles incompatible with V-ATPase biology. The refined mechanism is **ATP → V-ATPase activity → granule pH → V₁-V₀ sensor → mediator release**. CO₂ becomes a parallel marker of oxidative metabolism rather than the causal driver. Two independent agents converged on the *identical* rescue mechanism via matching first-principles reasoning. Loop 7 was the only formalized loop in the 13-loop architecture where CO₂ was the causal driver; after this refinement, no formalized loop has CO₂ as causal variable.

**Most recent project action (2026-04-11):** `Causal Independence in Feedback Loops.md` written; `Co-Production and Independence.md` deleted (superseded). `metabolic_foundations/` was not modified.

---

## What's Next

### The plan (current position: first-pass articulated, triangulated, rewritten; ready to methodologize)

1. ✅ **Articulate the causal-independence audit tool as a standalone document.** DONE — first pass `Co-Production and Independence.md` written.
2. ✅ **Triangulate the audit tool via two independent agents.** DONE — both classified as Refinement; counterexamples (sAC, AMPK) identified; existing-literature duplication caught; Pearl's screening-off + Palsson's null space confirmed as the right formal grounding.
3. ✅ **Verify sAC counterexample against primary sources.** DONE — Valsecchi 2014 (PMC4257896) confirmed bicarbonate as specific allosteric activator with ATP as substrate; pathway framed as feedforward metabolic matching rather than closed positive feedback (narrowing the counterexample's directness but preserving its structural point).
4. ✅ **Rewrite and rename the document.** DONE — `Causal Independence in Feedback Loops.md` replaces `Co-Production and Independence.md`. Grounded in existing frameworks, six-category taxonomy, four-check operational audit.
5. ✅ **Integrate the refined audit into `metabolic_foundations/Verification Methodology.md` as a sub-practice under Step 4** (Identify what a resolution would depend on). DONE — added as a substantial sub-practice block mirroring CF-2.A.4's citation deployment audit. Cites Pearl 2009 *Causality*, Reder 1988, Heinrich & Schuster 1996, Palsson 2003, Kacser & Burns 1973, Heinrich & Rapoport 1974 as the formal machinery. Includes the four-check audit, six-category taxonomy, Loop 7 as worked example, sAC as worked counterexample, and an explicit "not a novel principle" closing paragraph. `last-verified` updated to 2026-04-11. This is the second methodology improvement produced by Sub-test 2.A (first was CF-2.A.4). Both are now in the methodology.
6. **Run the causal-independence audit across all 13 formalized loops in `The System.md`** using the refined four-check operational audit. Produce a classified inventory.
7. **Run the citation deployment audit (CF-2.A.4) across all 13 loops** in the same pass where possible.
8. **Triangulate the audited loop inventory** via independent agents (Round 2 triangulation, separate from Round 1 which triangulated the audit tool itself).
9. **Synthesize audit findings into a clean loop inventory.** Each loop classified per the six-category taxonomy. This becomes the prerequisite substrate for Layer 3's formal bistability test.
10. **Decide Sub-test 2.B vs direct-to-Layer-3 based on audit outcome.** If Loop 9 (lactate self-amplification) resolved cleanly in the audit as independent driver with verified mechanism, 2.B may be reduced to confirmation or obviated. If Loop 9 surfaced new questions, run a focused 2.B. Otherwise proceed directly to Layer 3 with the clean loop inventory as substrate.

### Housekeeping pending

- `Research Brief - Co-Production Principle.md` should be deleted (one-shot artifact per Independent Agent Research Protocol) once the work is committed to durable form.
- `agent_1_report.md` and `agent_2_report.md` should be deleted (one-shot artifacts) once the work is committed.
- The git history will preserve all three for future reference.

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

**None.** The Refinement Diff Catalog exists in this vault as the precise file/passage-level reference for what each refinement consists of, but it is **not going to be applied** to `metabolic_foundations/` — that decision has been made (the refinements live in this vault as parallel knowledge instead).

Two edits have been applied to `metabolic_foundations/` from the entire stress test so far. Both are methodology improvements, not claim changes:

1. **CF-2.A.4** — citation deployment audit added to `metabolic_foundations/Verification Methodology.md` Step 5 (2026-04-10). Checks load-bearing citations on species / scenario / endpoint / proposed-mechanism match.
2. **Causal independence audit** — added to `metabolic_foundations/Verification Methodology.md` Step 4 (2026-04-11). Four-check operational audit grounded in Pearl's screening-off test and MCA conservation relations. Classifies metabolites named as causal drivers into six categories (independent driver / parallel marker / gated driver / co-driver / indeterminate). Triangulated via two independent agents before integration; sAC verified against primary sources.

Both methodology improvements emerged from a single sub-test (2.A) and apply to every future verification rather than to one claim — higher total leverage than individual claim refinements.

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
- `Causal Independence in Feedback Loops.md` (this vault) — causal-independence audit tool derived from Sub-test 2.A, grounded in Pearl's screening-off + Palsson/MCA conservation relations. Supersedes the earlier first-pass `Co-Production and Independence.md` which was deleted after triangulation identified it as over-general and a re-derivation of existing work.

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
