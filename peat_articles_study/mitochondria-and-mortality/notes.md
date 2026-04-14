---
article: "Mitochondria and mortality: Diet, exercise, and medicine, damaging or repairing respiratory metabolism"
url: https://raypeat.com/articles/articles/mitochondria-mortality.shtml
tier: 1
topic: metabolic-fork (CO₂ + lactate), with Foundation thesis overlay
vault-cross-reference: Foundation.md, The Metabolic Fork.md, The System.md
date-read: 2026-04-14
status: session-in-progress
---

# Mitochondria and mortality

## The Core Argument

Mitochondrial respiratory failure is the common substrate of aging and degenerative disease. Lactate is not a passive marker of that failure — it is an active cause of it, suppressing respiration and degrading mitochondria. CO₂ sits on the opposite side of the fork: the product of successful oxidation that Peat argues also causally sustains the conditions for more oxidation. Therapeutic direction: protect mitochondria by reducing lactate production and supporting oxidative metabolism (thyroid, saturated fat including palmitate, light, progesterone, and avoidance of PUFA/phytoestrogens/stress).

## Status

Session in progress. This file accumulates as we work through the article paragraph by paragraph. Current coverage: MAIN IDEAS / DEFINITIONS / opening paragraphs on exercise, lactate, and CO₂ adaptation. Updated iteratively.

## Real-Time Verification Log

### Claim: "CO₂ limits lactic acid formation" (paragraph on adaptation to hypoxia/hypercapnia)

- **Peat's position:** CO₂ causally suppresses glycolysis and lactate production. Implicit mechanism in this article: CO₂-lysine carbamylation stabilizing mitochondrial "phase," with lactate competing at the same binding sites as a destabilizer.
- **Vault's position:** CO₂ is a parallel marker at formalized feedback loops (Loop 7, V-ATPase/granule pH) but an **independent driver** at specific molecular targets outside the formalized loops — sAC (Kleinboelting 2014 allosteric site at Arg176), Cx26 K125 (Meigh 2013), ubiquitin K48 (Linthwaite 2022). Documented in The Metabolic Fork.md `[!warning]` callout at line 166-167 and Verification Methodology.md "Worked counterexample — soluble adenylyl cyclase" section.
- **Literature searched (two rounds):**
  - PFK-1 allosteric regulation (Nature Commun 2024 cryo-EM; Kaneko Sci Rep 2024 pH/ATP analysis; Dobson 1986 F2,6BP silencing)
  - Hypercapnia and glycolysis in vivo (PMID 2936711 skeletal muscle lactate release; PMID 10904053 acetazolamide forearm 31P-MRS; bicarbonate loading meta-analyses)
  - Non-canonical CO₂ signaling (Acin-Perez 2009 PMID 20049744; Chang 2021 PMID 33412125; Dobson/Linthwaite 2023 PMID 37723562)
- **What the evidence shows:**
  - **At glycolytic enzymes (PFK-1):** No direct CO₂/bicarbonate binding site (2024 cryo-EM, 6 sites mapped, none for bicarbonate). CO₂'s effect on glycolysis runs through pH → H+ → reinforcing ATP's allosteric inhibition. In fed/insulin-stimulated states, F2,6BP releases ATP from PFK's regulatory site and largely silences the pH modulation. Quantitatively small at normal physiological pH swings.
  - **Acetazolamide dissociation is NOT clean as often claimed:** PMID 10904053 shows intracellular pH is similar between Acz and control at end-exercise (6.38 vs 6.43). Lower plasma lactate with Acz is attributable to impaired lactate **efflux** (MCT H+ co-transport disruption), not reduced production.
  - **Bicarbonate loading RAISES lactate (~31% peak: 16.2 vs 12.4 mmol/L) via increased glycolytic activity, not just improved efflux.** Muscle biopsies show increased glycogen utilization and lactate production. Mechanism: extracellular bicarbonate → better H+ efflux → intracellular pH stays higher → PFK stays more active.
  - **At OXPHOS regulation (sAC pathway):** Bicarbonate binds sAC at a specific allosteric site. Matrix cAMP generated. Two downstream arms: (a) **PKA** phosphorylates COX I and COX IV (Acin-Perez 2009), increasing electron flow; (b) **Epac1** regulates Complex I activity and cytosolic NADH/NAD+ redox state (Chang 2021). **Chang 2021 directly demonstrates: suppressing sAC → increased lactate secretion + decreased pyruvate secretion + shift to glycolysis.** This is the experimental confirmation of the vault's structural claim.
- **Verdict:**
  - **Peat's core claim (CO₂ limits lactate) — confirmed functionally, with corrected mechanism.** Right destination, wrong route. Peat's phase-stability/lysine-competition mechanism is not supported. The actual route is CO₂ ↔ bicarbonate → sAC → matrix cAMP → PKA (COX I/IV phosphorylation) + Epac1 (Complex I) → OXPHOS activation → pyruvate drawn into Krebs cycle → less pyruvate available for LDH → less lactate produced.
  - **Vault's current framing — confirmed.** The scope-limitation already in The Metabolic Fork.md (parallel marker at Loop 7, independent driver at sAC/Cx26/Ub-K48) is correct and supported by the verification.
- **Implications:**
  - No vault refinement of framing needed. The scope-limitation is already correct.
  - Three evidence additions below (not in the vault) strengthen the existing treatment without changing it.

## Candidate Vault Refinements

> None rise to the bar of a framing change. Items below are **citation/evidence additions** that the vault's existing treatment would benefit from incorporating. The vault's framing on CO₂ is already correct; these strengthen the evidence base.

### Citation addition 1: Chang 2021 — experimental confirmation of sAC as glycolysis/OXPHOS switch

- **What:** [Chang et al. 2021, BBA-Bioenergetics, PMID 33412125](https://pubmed.ncbi.nlm.nih.gov/33412125/). Pharmacological and genetic suppression of sAC (ADCY10) in multiple cell lines and primary hepatocyte/cholangiocyte cultures increased lactate secretion, decreased pyruvate secretion, and elevated cytosolic NADH/NAD+ ratios. Authors explicitly characterize sAC as *"effectively a bioenergetic switch between aerobic glycolysis and oxidative phosphorylation at the post-translational level."*
- **Why it matters:** The vault's current sAC treatment (The Metabolic Fork.md line 167; Verification Methodology.md line 239) cites structural/mechanistic papers (Acin-Perez 2009, Valsecchi 2014, Kleinboelting 2014) that establish bicarbonate as an independent driver. Chang 2021 adds the **functional confirmation**: actually turn sAC off, and cells shift to glycolysis with more lactate. This is direct experimental evidence for the functional prediction the vault already makes structurally.
- **Location:** Suggested insertion: The Metabolic Fork.md, into the `[!warning]` callout at line 167 (append after the existing sAC citation), and into Verification Methodology.md "Worked counterexample — soluble adenylyl cyclase" section (as functional confirmation of the structural mechanism).

### Citation addition 2: Chang 2021 — the Epac1 arm at Complex I (distinct from PKA arm at COX)

- **What:** Chang 2021 specifically found that **Epac1, not PKA, was the downstream effector** for sAC's regulation of Complex I activity and cytosolic redox state. This is distinct from the PKA arm (Acin-Perez 2009) that phosphorylates COX I/IV subunits.
- **Why it matters:** The vault's sAC description currently references only the PKA → COX arm. The Epac1 arm represents a second distinct downstream mechanism, extending the biological reach of bicarbonate signaling at mitochondria.
- **Location:** Same locations as citation addition 1. Frame as "two distinct downstream arms of sAC-derived matrix cAMP: PKA at Complex IV, Epac1 at Complex I."

### Citation addition 3: Dobson/Linthwaite 2023 macrophage carbamylome — extends CO₂ anti-inflammatory reach

- **What:** [Dobson/Linthwaite et al. 2023, PMID 37723562](https://pubmed.ncbi.nlm.nih.gov/37723562/). TEO chemoproteomic mapping identified 8,923 carbamylated peptides in macrophages. Functional demonstration: carbamylation of linear di-ubiquitin blocks OTULIN, producing a direct CO₂-inflammation link with metabolic implications via NF-κB.
- **Why it matters:** The vault's current ubiquitin K48 citation (Linthwaite 2022, Frontiers Mol Biosci) established the K48-polyubiquitination mechanism. The 2023 follow-up extends this into the inflammatory/metabolic axis by identifying OTULIN as a carbamylation target and placing the mechanism in primary immune cells. Relevant to the vault's inflammation/immunity claims across multiple documents.
- **Location:** The Metabolic Fork.md `[!warning]` callout (expand the ubiquitin K48 citation); potentially cross-reference from Conservation Signaling.md if NF-κB modulation intersects with MCAS/histamine claims.

### Formalization gap: sAC as a feedback loop

- **What:** Verification Methodology.md line 239 explicitly notes: *"The sAC pathway is currently framed in the literature as feedforward metabolic matching rather than closed positive feedback, and is not currently a formalized loop in the vault."* This is the vault's own flagged gap.
- **Argument for formalization:** Chang 2021 shows sAC is bidirectional — suppression shifts toward glycolysis, activation shifts toward OXPHOS. Combined with the fact that OXPHOS produces the bicarbonate that activates sAC (via matrix CA V), this has the topology of a closed positive feedback loop: OXPHOS → CO₂/bicarbonate → sAC → cAMP → PKA/Epac1 → COX phosphorylation + Complex I activation → more OXPHOS.
- **Counter-argument for keeping it unformalized:** The literature still frames it as feedforward metabolic matching. Formalizing as a closed loop would require demonstrating that the loop gain is sufficient for self-reinforcement, which Chang 2021 suggests but does not quantify.
- **Recommendation:** Flag but do NOT formalize. Higher bar for vault changes than a single 2021 paper provides. Worth monitoring as follow-up literature develops.

## Session Notes

### Meta-lesson logged (captured separately in Reading Protocol)

My first-round synthesis claimed "the vault's 'parallel marker' framing needs explicit scope-limitation" as a candidate refinement. This was wrong — the scope-limitation already exists in The Metabolic Fork.md at lines 166-167 as a dedicated `[!warning]` callout, and in Verification Methodology.md at lines 239-241 as a worked counterexample. I had read the CLAUDE.md summary (line 150: "CO2 is a parallel marker, not a causal driver in any feedback loop") as a global claim rather than following it to the mechanism document where the scope-limitation is explicit. Captured in Reading Protocol as a general rule: before flagging a vault gap or proposing a refinement, trace the claim to the mechanism document, not just the summary.

### Reasoning-chain observations (from current reading)

1. **Peat explicitly states bistability** in the phase-stability paragraph: *"the system would have two possible states, one, the glycolytic stress state, and the other, the carbon dioxide producing energy-efficient state."* This is Peat stating the two-attractor architecture in 2000, decades before the vault formalized it via Mulukutla and Topp. Worth preserving as an integration-that-holds example.

2. **Peat's specific mechanism proposal (CO₂-lysine carbamylation competing with lactate at protein binding sites) is remarkably close to the later-discovered Cx26 K125 carbamylation (Meigh 2013) and ubiquitin K48 carbamylation (Linthwaite 2022).** He got the chemistry right in principle — lysine carbamylation is real. He put it at the wrong target (mitochondrial "phase stability" rather than specific channels and signaling proteins). This is "right destination, wrong route" with unusually specific mechanism-level foresight.

3. **Peat's "concentric" muscular work distinction (contraction with load, relaxation without) mapping to Rule 1 controlled-deployment criteria** — the heart example (heart mitochondria don't decline with aging) is a good illustration of hormesis via controlled-deployment exercise.

### Open items for continued reading

- The palmitate/cardiolipin/COX claim (Bolon 1997 citation) — verify independently when we reach that section.
- The "gene shifting" mitochondrial repair claim (Taivassalo 1999) — citation deployment audit needed.
- The phytoestrogen/tofu/dementia claim in the DEFINITIONS — needs checking.
- The lactated Ringer's mortality comparison claims — specific study verification.
