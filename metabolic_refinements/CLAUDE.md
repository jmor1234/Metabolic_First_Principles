# Metabolic Refinements Vault

A standalone knowledge layer that captures refinements to the `metabolic_foundations/` framework discovered through stress testing and other independent triangulation. This vault does not modify metabolic_foundations — it presents the refinements as parallel standalone knowledge so the original integration stays intact and the refinement reasoning is preserved.

## Why This Vault Exists

The metabolic_foundations vault is an integration that took rigorous work to build. Per its Verification Methodology's asymmetry principle, the cost of wrongly changing it is higher than the cost of wrongly leaving it unchanged. Stress testing surfaces refinements, but those refinements should not silently overwrite the original — they should sit beside it as a separate epistemic layer.

This vault is that layer. A reader who wants the most current understanding of the framework reads metabolic_foundations *and* this vault. Each is independent. Neither replaces the other.

## Relationship to Other Vaults

Three vaults form a trajectory of epistemic stance on the same underlying biology:

| Vault | Role | Stance |
|---|---|---|
| `peat_claims_verified/` | Audit trail | Verification of Peat's biochemistry against modern research |
| `metabolic_foundations/` | Extracted standalone knowledge | The verified findings, organized around biology, person-independent |
| **`metabolic_refinements/`** (this vault) | Refinements layer | What stress testing found needs refinement in the extracted knowledge |

The three vaults are independent. Each captures a different epistemic stance and stands on its own. The refinements vault is *in dialogue with* metabolic_foundations (it references specific files and passages by name) but does not modify it and does not cross-link via wikilinks.

## Conventions

### Cross-vault links

- **Wikilinks within this vault**: yes, encouraged
- **Wikilinks across vault boundaries** (to `metabolic_foundations/` files): **no**
- **Prose references to metabolic_foundations files by name and section**: yes — this is how refinement documents point at what they refine, consistent with how `Stress Test.md` and `Vault Edit Proposal.md` already reference them
- **The metabolic_foundations vault should not link back to this vault either** — it must remain standalone

### Refinement document structure

Each refinement document follows this template:

1. **Original Claim** — what metabolic_foundations currently says, cited by file and section
2. **What [Sub-test X] Found** — the investigation findings, evidence, first-principles reasoning
3. **Refined Claim** — the standalone refined version, readable without flipping back to the original
4. **Structural Consequences** — what else this refinement affects, including the architecture-level implications
5. **Open Questions** — carry-forward items, dependencies, what evidence would resolve outstanding questions
6. **Audit Trail** — pointer to the relevant section in `Stress Test.md` and `Vault Edit Proposal.md`

### Frontmatter fields

- `title` — refinement name
- `aliases` — alternative names (optional)
- `status` — `proposed` (drafted, under review) or `accepted` (finalized as standalone refinement in this vault)
- `last-updated` — date
- `refines` — list of metabolic_foundations files affected
- `source` — which sub-test produced the finding (e.g., "Stress Test Sub-test 2.A")
- `classification` — `pass` | `pass-with-observation` | `refinement` | `refinement-substantial` | `fail`
- `triangulation` — `own-research` | `own-research+independent-agents`
- `dependencies` — other refinements or carry-forward items this depends on

### Status semantics

- **`proposed`** — drafted, may still change pending review
- **`accepted`** — finalized as the canonical standalone refinement in this vault. Does NOT mean metabolic_foundations is changed; it means the refinement is the current best understanding of this specific claim within this vault.

## Vault Contents

### Working files (audit trail)

- **`Stress Test.md`** — the active investigation log. Layer-by-layer adversarial probes against metabolic_foundations' load-bearing claims. Includes sub-test results, classifications, carry-forward items. This is where the work happens.
- **`Vault Edit Proposal.md`** — the diff-form catalog of edits the stress test would apply *if* the decision were to overwrite metabolic_foundations. **These edits are not going to be applied.** The proposal is preserved here as the precise reference for what each refinement consists of at the file/passage level. Useful for anyone who wants to see exactly which words would change in which file.

### Refinement documents (standalone knowledge)

- **`Convergence Point Reading.md`** — clarifies that the framework's ontological claim is Reading C (metabolism as universal convergence point), not Reading A (strong reduction). Adds Huntington's as a non-circular example of "genetics operating through metabolism." Source: Stress Test Sub-test 1.A.

- **`Krebs-Cycle Invariance and Ketone Bodies.md`** — softens "of glucose" specificity toward "Krebs-cycle CO₂ production as the invariant"; introduces ketone bodies as a biochemically distinct third fuel category; distinguishes Randle pathology from adapted ketosis; introduces the cerebral perfusion non-dominance finding and the hepatic ketogenesis shunt as a Rule-1 controlled deployment. Source: Stress Test Sub-test 1.B (six findings R1.B.1 through R1.B.6).

- **`Loop 7 — Metabolism-Mediator Coupling.md`** — replaces direct CO₂→pH→granule mechanism with ATP→V-ATPase→granule pH→V₁-V₀ sensor coupling. Structural consequence: no formalized loop in the 13-loop architecture has CO₂ as causal driver after this refinement. Includes the deeper conceptual implication that CO₂/ATP are stoichiometrically co-produced and CO₂ cannot be an independent feedback participant. Source: Stress Test Sub-test 2.A.

## How New Refinements Get Added

The discipline follows the metabolic_foundations Verification Methodology, adapted for this vault's role:

1. **Stress test the load-bearing claim.** Document the probe and findings in `Stress Test.md`. Apply the six-step verification sequence, the three hypotheses (in order), and the three rules (acute/chronic, context-dependence, pass/refinement/fail).
2. **Draft proposed edits in diff form** in `Vault Edit Proposal.md`. This is the precise file/passage-level reference — preserved here regardless of whether anything is overwritten in metabolic_foundations.
3. **Synthesize as a standalone refinement document** in this vault following the template above. The refinement document is the knowledge object — it presents the refined claim with full reasoning, readable without flipping back to the original.
4. **Mark status `proposed`** until reviewed; promote to `accepted` once finalized.

The original metabolic_foundations vault is never modified. Its `last-verified` dates do not update from this vault's activity. The integration the methodology was built to protect stays as originally written.

## Working Files vs Standalone Refinements

The split matters:

- **Working files** (`Stress Test.md`, `Vault Edit Proposal.md`) are process artifacts. They preserve *how* the refinements were derived. Someone auditing the work, running the next sub-test, or wanting the precise file-level diff starts here.
- **Standalone refinements** (the topic-named documents) are knowledge artifacts. They present *what* the refinement is, in a form a reader can engage with without following the entire investigation chain. Someone who wants to understand "what is the current refined view of Loop 7" starts here.

Both are needed. Neither replaces the other. The working files generate the refinement documents; the refinement documents stand on their own.

## Where the Stress Test Currently Is

Layer 1 complete (REFINEMENT substantial). Layer 2 in progress — Sub-test 2.A complete (REFINEMENT substantial mechanism-level), Sub-test 2.B not yet started. Layers 3, 4, 5 not started. Layer 6 subsumed into the protocol via Rules 1–3.

See `Stress Test.md` for the live status of every layer and sub-test.
