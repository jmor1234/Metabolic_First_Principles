# Current State

**Last updated:** 2026-04-11

This is the single canonical source for what is being actively worked on in this project right now. It is small by design and updated as work progresses. Other files (`Stress Test.md`, the refinement documents, `Refinement Diff Catalog.md`) are the substance; this file is the pointer.

If you are a new agent picking this up, read this file first, then follow the "Where to Read for Context" pointers at the bottom.

---

## Where We Are Right Now

**Mid stress test of `metabolic_foundations/`. Layer 2 in progress.**

| Layer | Claim under attack | Status |
|---|---|---|
| Layer 0 — Bedrock | ATP requirement, ~18× difference, both pathways real | NOT TESTED (would mean overturning textbook biochemistry) |
| Layer 1 — Ontological move | Health IS efficient oxidative metabolism of glucose to CO₂ | **COMPLETE — REFINEMENT (substantial)** |
| Layer 2 — Product-activity | CO₂ and lactate are active, not inert | **IN PROGRESS** — Sub-test 2.A COMPLETE, Sub-test 2.B NOT STARTED |
| Layer 3 — Attractor dynamics | 13 interlocking loops generate genuine bistability | NOT STARTED |
| Layer 4 — Cross-disease convergence | Every chronic disease shows the same metabolic signature | NOT STARTED |
| Layer 5 — Epistemic meta-claim | "The integration is the missing step" | NOT STARTED |
| Layer 6 — Falsifiability meta-test | (subsumed into Verification Methodology Rules 1–3) | SUBSUMED |

Three refinements have landed so far. All are documented as standalone refinement documents in this vault. None have been applied to `metabolic_foundations/` — the original integration is preserved as written, refinements sit beside it as parallel knowledge per the asymmetry principle.

---

## What Just Happened

**Most recent substantive finding (2026-04-10):** Sub-test 2.A — Loop 7 mechanism refinement. The framework's stated mechanism (extracellular CO₂ → carbonic acid → granule pH → mediator release) is first-principles incompatible with V-ATPase biology. The refined mechanism is **ATP → V-ATPase activity → granule pH → V₁-V₀ sensor → mediator release**. CO₂ becomes a parallel marker of oxidative metabolism rather than the causal driver. Two independent agents converged on the *identical* rescue mechanism via matching first-principles reasoning — strongest triangulation signal so far.

**Structural consequence:** Loop 7 was the only formalized loop in the 13-loop architecture where CO₂ was the causal driver. After this refinement, **no formalized loop has CO₂ as causal variable.** The framework's "CO₂ is an active product" claim survives biologically (Bohr effect, carbamino, neuroprotection) but loses its sole formalized loop support.

**Most recent project action (2026-04-11, commit 6112d5b):** The `metabolic_refinements/` vault was created. Stress test findings now live here as a parallel knowledge layer. `Stress Test.md` and `Refinement Diff Catalog.md` were moved into this vault. Three standalone refinement documents were created. Workspace orientation files (root `CLAUDE.md`, `Overview.md`) were updated to describe the three-vault structure. **`metabolic_foundations/` was not modified.**

---

## What's Next

### Immediate next move

**Sub-test 2.B — Lactate-active claim / Loop 9 / histone lactylation causality.** Completes Layer 2.

The structural question mirrors Sub-test 2.A: is lactate an active driver of disease state, or a reliable marker of underlying metabolic failure? The histone lactylation literature (Zhang et al. 2019, *Nature*) is stronger than the CO₂-granule-pH literature was — so this may resolve asymmetrically. Possible outcomes:

- **PASS** — lactate's active driver role survives scrutiny; Layer 2 completes with one half PASS and one half REFINEMENT
- **REFINEMENT** — like Sub-test 2.A, the directional claim survives but the specific mechanism gets corrected
- **FAIL** — would be the largest finding so far; would force significant retreat in the framework's "active product" framing

Triangulate via independent agents (matches the established pattern from 1.B and 2.A).

### After Sub-test 2.B

In rough order of leverage:

1. **Resolve CF-2.A.5** — independent verification of Bolevich & Kogan 2016 (the strongest remaining "CO₂ as active protector" non-loop claim). This is a focused single-paper verification, not a full sub-test. Required before the broader Foundation.md / Metabolic Fork.md "CO₂ is an active product" reframing can proceed.
2. **Layer 3 — Attractor architecture as genuine dynamics.** The most consequential remaining layer. Tests whether the 13-loop architecture is real dynamical-systems bistability or a precise metaphor for clinical bimodality. The loop-gain question CF-2.A.2 (do any of the directional couplings actually achieve loop gain > 1?) gets formally tested here. **If Layer 3 fails, the "two attractors" framing collapses to metaphor — the largest possible finding of the stress test.**
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

The only edit applied to `metabolic_foundations/` from the entire stress test so far is the **CF-2.A.4 methodology improvement** (citation deployment audit added to `metabolic_foundations/Verification Methodology.md` Step 5). This is a methodology improvement, not a claim change.

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

### 5. Framework context
Only read if not already familiar with the metabolic_foundations framework being attacked:
- `metabolic_foundations/CLAUDE.md` — vault structure, navigation strategy
- `metabolic_foundations/Foundation.md` — the thesis and first-principles argument (~3,500 words)
- `metabolic_foundations/The System.md` — the architecture, two attractors, 13 feedback loops (~4,500 words)

### 6. Methodology
Required reading before attempting any new sub-test or proposing any change:
- `metabolic_foundations/Verification Methodology.md` — the discipline. Three Hypotheses, Six-Step Verification Sequence, Three Rules, Default Position, citation deployment audit (CF-2.A.4 addition).

### 7. Per-vault navigation (as needed)
- `peat_claims_verified/CLAUDE.md` — only if you need to trace something back to the original Peat verification audit trail.

---

## Recent Commits

Most recent at top. Run `git log --oneline -20` for full history.

```
6112d5b  Create metabolic_refinements vault — refinements layer separate from the original integration
7c1022c  moving the first principles der to a different vault for a clean separation of concerns
7b32f9b  Add First Principles Derivation charter — independent bottom-up experiment
fa1b58f  Expand Vault Edit Proposal with Layer 1 edits, rename to cover all layers
9295d97  Sub-test 2.A: Loop 7 REFINEMENT — mechanism is ATP→V-ATPase, not CO₂→pH
98e7c6d  Add Independent Agent Research Protocol for triangulation methodology
1f68c4f  Add Carry-Forward Items section tracking deferred Layer 1 questions
2e488d6  Complete Layer 1 stress test: 1.A PASS, 1.B substantial REFINEMENT
14782da  Add Stress Test tracking doc for systematic vault verification
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
