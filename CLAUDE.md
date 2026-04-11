# Workspace: Three Obsidian Vaults

This workspace contains three independent Obsidian vaults. Each has its own CLAUDE.md with vault-specific navigation, conventions, and agent instructions.

**For the full project narrative** — what the project is, why it was built this way, what it found, and how the three vaults relate — read `Overview.md` in this directory.

## ⚡ Current Work — Read This First

The project is currently mid stress test of `metabolic_foundations/`. The single canonical file for what is being actively worked on, what just happened, what's next, and what's blocking is:

**→ `metabolic_refinements/Current State.md`**

Read it before doing anything else. It is small by design, it points to the right files for picking up the work, and it is the only file in the project guaranteed to reflect the current active state.

The three sub-vault CLAUDE.mds and `Overview.md` describe the project's *structure and history*. `Current State.md` describes the *active work*. Both kinds of orientation are needed — but if you only have time for one before acting, read `Current State.md`.

## Metabolic Foundations (`metabolic_foundations/`)

A first-principles understanding of what health and disease are at the metabolic level. 14 documents. Verified against peer-reviewed research, organized around biology itself, independent of any single person's framework. Includes a verification methodology governing how the vault is tested and changed.

**Start here:** `metabolic_foundations/CLAUDE.md`

## Metabolic Refinements (`metabolic_refinements/`)

The refinements layer. Captures refinements to the Metabolic Foundations framework discovered through stress testing and other independent triangulation, presented as standalone knowledge. **Does not modify Metabolic Foundations** — the original integration stays intact, and the refinements sit beside it as a separate epistemic layer. A reader who wants the most current understanding reads both vaults.

Contains the live stress test working files (`Stress Test.md`, `Refinement Diff Catalog.md`) plus standalone refinement documents derived from each completed sub-test.

**Start here:** `metabolic_refinements/CLAUDE.md`

## Peat Claims Verification (`peat_claims_verified/`)

The verification archive. Systematic claim-by-claim verification of Ray Peat's biochemistry against modern research. 16 topic documents with three-phase methodology. This vault produced the knowledge that Metabolic Foundations extracts and presents as standalone science.

**Start here:** `peat_claims_verified/CLAUDE.md`

## Relationship

The three vaults form a trajectory of epistemic stance on the same underlying biology:

1. **`peat_claims_verified/`** is the deepest audit trail — raw claim extractions, research landscape analysis, individual assessments, corrections.
2. **`metabolic_foundations/`** is the extracted knowledge — organized by biology, not by claims, person-independent. Built FROM the Peat verification vault.
3. **`metabolic_refinements/`** is the refinements layer — what stress testing found needs refinement in the extracted knowledge, presented as standalone knowledge that does not modify the original.

The three vaults are independent. **Do not cross-link between them via wikilinks.** Each has its own conventions, callout types, frontmatter fields, and navigation strategy. When working in one vault, use that vault's CLAUDE.md.

The one allowed exception is `metabolic_refinements/`, which is inherently *in dialogue with* `metabolic_foundations/` — it references specific files and passages by name in prose, but does not use wikilinks across the boundary. This preserves each vault's standalone integrity while allowing the refinements to point at what they refine.

## How to Approach All Three Vaults

All three vaults are integrations, not databases. The meaning of any specific claim depends on its connections to others through the wikilink network within that vault. Reading individual statements at face value produces shallow conclusions and false contradictions. Before evaluating evidence, proposing changes, or answering complex questions, trace the reasoning chain through the connections — and if you cannot, study the vault more deeply before drawing conclusions. Each vault's CLAUDE.md provides the specific discipline for doing this properly.

The asymmetry principle applies across all three: the cost of wrongly changing an integration is higher than the cost of wrongly leaving it unchanged. This is why `metabolic_refinements/` exists as its own vault rather than being applied as edits to `metabolic_foundations/` — refinements are real, the methodology is correctly catching them, but the original integration is preserved as written and the refinements sit beside it as parallel knowledge.
