# Vault Edit Proposal — Sub-test 2.A Refinements

**Status:** Draft for review. No vault files have been modified yet. Commit pending approval.

**Source finding:** Sub-test 2.A (documented in `Stress Test.md`) classified as REFINEMENT (substantial, mechanism-level). Loop 7's stated mechanism (extracellular CO₂ → granule pH via carbonic acid equilibration) is first-principles incompatible with V-ATPase biology. The refined mechanism is ATP → V-ATPase → granule pH → V₁-V₀ sensor → mediator release. CO₂ becomes a parallel marker of oxidative metabolism rather than the causal driver. This has structural consequences for the vault's broader "CO₂ is an active product" claim, which loses its sole formalized loop support.

**Affected files:**
- `metabolic_foundations/The System.md` (3 passages)
- `metabolic_foundations/The Metabolic Fork.md` (2 passages)
- `metabolic_foundations/Foundation.md` (1 passage)
- `metabolic_foundations/Conservation Signaling.md` (1 passage — dedicated "Shared Triggers" subsection, found via grep after initial draft)
- `metabolic_foundations/The Preferred Substrate.md` (1 passage — single sentence in "Why Glucose" section)

**Summary of changes:**
- Replace direct CO₂-to-granule-pH mechanism with ATP → V-ATPase mechanism throughout
- Rename "CO₂-Serotonin Loop" to "Metabolism-Mediator Loop"
- Add warning callouts acknowledging loop gain has not been measured at physiological ATP variations and that no direct in vivo human study exists
- Remove Freed 2001 citation entirely (mis-cited — canine dry-air model)
- Recontextualize Pollard 1977 (operates during stimulated exocytosis only)
- Add Poëa-Guyon 2013, Nunomura 2017, Möllerherm 2017, Barnes & Brown 1981 as new primary citations
- Retain Strider 2011 with supraphysiological caveat
- Preserve directional claims and clinical/diagnostic implications (ETCO₂ monitoring remains valid)

---

## Edits to `The System.md`

### Edit 1.1 — CO₂-dominant attractor narrative

**Location:** Section "The CO₂-Dominant Attractor (Health)", currently line 31.

**Current text:**

> **High CO₂ production** → CO₂ maintains acidic pH in mast cell and platelet storage granules → **serotonin and histamine remain sequestered** (not released into circulation) → metabolic suppression signal absent → oxidative metabolism continues unimpeded →

**Proposed replacement:**

> **High CO₂ production** (marker of vigorous oxidative metabolism producing cytosolic ATP) → ATP powers V-ATPase, which actively maintains acidic interior pH in mast cell and platelet storage granules → **serotonin and histamine remain sequestered** (not released into circulation) → metabolic suppression signal absent → oxidative metabolism continues unimpeded →

**Rationale:** Preserves the narrative arrow and the directional claim, but routes the causal mechanism through ATP/V-ATPase rather than through direct CO₂/pH chemistry. CO₂ stays in the text as a diagnostic marker because it remains a reliable readout of oxidative metabolism.

---

### Edit 1.2 — Lactate-dominant attractor narrative (mirror image)

**Location:** Section "The Lactate-Dominant Attractor (Disease)", currently line 49.

**Current text:**

> **Low CO₂ production** → pH shifts alkaline → storage granule stability lost → **serotonin and histamine released** → serotonin directly suppresses metabolic rate, promotes vasoconstriction, inhibits mitochondrial function → oxidative capacity falls further →

**Proposed replacement:**

> **Low CO₂ production** (marker of failing oxidative metabolism and falling cytosolic ATP) → V-ATPase pumping slows → granule interior pH rises → V₁-V₀ sensor dissociates → **serotonin and histamine released** → serotonin directly suppresses metabolic rate, promotes vasoconstriction, inhibits mitochondrial function → oxidative capacity falls further →

**Rationale:** Mirror image of Edit 1.1. Maintains the cascade structure of the attractor narrative while correcting the mechanism statement. The "pH shifts alkaline → granule stability lost" causal chain is replaced with "ATP drops → V-ATPase slows → granule pH rises → sensor dissociates → mediators released."

---

### Edit 1.3 — Loop 7 renaming and mechanism replacement

**Location:** Section "System-Wide Regulation", Loop 7 description, currently line 125.

**Current text:**

> **The CO₂-Serotonin Loop.** Low CO₂ production shifts pH toward alkaline, destabilizing the acidic storage granules that sequester serotonin. Serotonin is released into circulation. Serotonin suppresses oxidative metabolism (directly inhibiting mitochondria, promoting vasoconstriction, lowering body temperature). Less oxidative metabolism produces less CO₂. Less CO₂ releases more serotonin. The protective output and the conservation signal are reciprocally linked through pH chemistry.

**Proposed replacement:**

> **The Metabolism-Mediator Loop.** Mast cell and platelet secretory granules maintain acidic interior pH (~5.3–5.5) via [V-ATPase](https://pubmed.ncbi.nlm.nih.gov/24165939/) — an ATP-dependent proton pump that holds a ~1.9-unit gradient against cytosol and simultaneously acts as the granule pH sensor through V₁-V₀ dissociation. When oxidative metabolism falls, cytosolic ATP drops and V-ATPase pumping slows; granule interior pH rises and the V₁-V₀ sensor dissociates, signaling release readiness and triggering [mediator leak](https://www.nature.com/articles/cddis2017206). Released serotonin suppresses oxidative metabolism (directly inhibiting mitochondria, promoting vasoconstriction, lowering body temperature); released histamine drives inflammation and vascular dysregulation. Reduced oxidative metabolism further depletes ATP, compounding V-ATPase failure. The active driving variable in this loop is **ATP availability**; CO₂ production tracks in parallel as a reliable marker of the oxidative state, not as the causal participant. See the warning callout below.
>
> > [!warning] Mechanism refined; loop gain unmeasured at physiological ATP ranges
> > An earlier version of this loop attributed granule destabilization to extracellular CO₂ directly driving intragranule pH via carbonic acid equilibration. That mechanism is biochemically implausible: granule interior pH is maintained against a ~1.9-unit gradient by active V-ATPase pumping, and physiological extracellular pH variation (~0.05–0.15 units from PaCO₂ swings) is buffered through plasma → cytosol (NHE1, AE3) → granule (V-ATPase compensation) and cannot propagate into the granule interior at meaningful magnitude. [Bafilomycin A1 (V-ATPase inhibition) is required to raise granule pH enough to trigger histamine leak](https://www.nature.com/articles/cddis2017206). The ATP → V-ATPase refinement is mechanistically coherent but has not been directly tested in mast cells or platelets at the graded physiological ATP variations relevant to this loop. [Hypoxia (1% O₂) does increase histamine release from mast cells](https://pubmed.ncbi.nlm.nih.gov/28553287/), consistent with the ATP mechanism but at severe metabolic stress. [Isocapnic voluntary hyperventilation does not produce measurable plasma histamine elevation in humans](https://pubmed.ncbi.nlm.nih.gov/7261540/) — the mechanical act of hyperventilation alone is not operative. No study has measured serum tryptase or plasma histamine response to voluntary *hypocapnic* (non-isocapnic) hyperventilation in humans. The loop's directional claim (low oxidative metabolism → mediator activation → further suppression) is likely correct, but whether it achieves loop gain > 1 — required for genuine bistability rather than damped directional response — is unknown.

**Rationale:** This is the most substantial single edit. The loop is renamed because "CO₂-Serotonin" mis-identifies the active variable; the new name ("Metabolism-Mediator") accurately describes what's happening (general metabolic state couples to mediator release). The body of the loop description replaces the pH-chemistry mechanism with the ATP/V-ATPase mechanism, citing the two primary references (Poëa-Guyon 2013 for V-ATPase as sensor, Nunomura 2017 for V-ATPase as maintainer). The warning callout addresses the magnitudes of uncertainty explicitly — including the loop-gain question (CF-2.A.2) and the empirical gap (CF-2.A.3) — so readers understand this is a plausible refinement, not a verified bistable structure.

---

## Edits to `The Metabolic Fork.md`

### Edit 2.1 — "Inflammatory mediator sequestration" subsection

**Location:** Section "CO2 as Active Protector", subsection "Inflammatory mediator sequestration", currently line 69.

**Current text:**

> **Inflammatory mediator sequestration.** Platelet serotonin release is [pH-dependent -- suppressed by acidic conditions](https://pmc.ncbi.nlm.nih.gov/articles/PMC431691/). Mast cell histamine storage follows the same chemistry. CO2 produces carbonic acid, maintaining the slightly acidic conditions that keep serotonin and histamine sequestered in storage granules. When CO2 falls, pH rises, and both mediators leak into circulation. This is why [repeated hyperventilation increases histamine reactivity](https://www.atsjournals.org/doi/full/10.1164/ajrccm.164.5.2003081) and why the cerebral vasoconstriction, anxiety, and panic of hyperventilation are partly serotonin-mediated.

**Proposed replacement:**

> **Mediator sequestration is ATP-dependent via V-ATPase.** Mast cell secretory granules and platelet dense granules maintain acidic interior pH (~5.3–5.5) through [active V-ATPase proton pumping](https://pubmed.ncbi.nlm.nih.gov/24165939/) against a ~1.9-unit gradient from cytosol. The acidic environment keeps serotonin bound to polyphosphate/calcium (platelet dense granules) and histamine bound to heparin (mast cell granules) through electrostatic interaction of protonated amine groups with anionic matrix. When cellular ATP falls, V-ATPase pumping slows, granule interior pH rises, and the V-ATPase V₁-V₀ sensor dissociates — coupling granule destabilization to exocytosis readiness. [Bafilomycin A1 (V-ATPase inhibitor) reproduces this phenotype: granule pH rises, intracellular histamine falls, extracellular histamine rises](https://www.nature.com/articles/cddis2017206). The coupling from systemic metabolic state to mast cell and platelet mediator release therefore runs through ATP and V-ATPase, not through extracellular CO₂ setting granule pH directly. CO₂ production tracks in parallel with ATP as a reliable marker of oxidative metabolism but is not the causal participant in granule stability. [Pollard et al. 1977](https://pmc.ncbi.nlm.nih.gov/articles/PMC431691/) demonstrated that alkaline extracellular pH can accelerate serotonin release from platelets *during stimulated exocytosis* via anion transport and osmotic lysis of the granule-plasma membrane complex — this is a mechanism that operates when granules are already juxtaposed to the membrane during active degranulation, not one that drives spontaneous release under resting hypocapnia. [100% CO₂ pretreatment of mast cells suppresses degranulation via intracellular calcium repression](https://pubmed.ncbi.nlm.nih.gov/21284650/), which is the basis for intranasal CO₂ as a clinical treatment for allergic rhinitis — but this mechanism has only been demonstrated at supraphysiological CO₂ concentrations (~20× alveolar) and its operation at physiological CO₂ ranges has not been tested.
>
> > [!warning] Mechanism refined; in vivo magnitude untested
> > An earlier version of this passage attributed granule acidity maintenance to extracellular CO₂ producing carbonic acid. That mechanism is biochemically implausible at physiological pH ranges — blood pH (7.35–7.45) is ~79-fold higher in [H⁺] than granule interior pH (5.3–5.5), a gradient that cannot be maintained by equilibrium chemistry, only by active pumping. The refined ATP/V-ATPase mechanism is mechanistically coherent but loop gain at physiological ATP variations has not been measured. [Isocapnic voluntary hyperventilation does not produce measurable plasma histamine change in humans](https://pubmed.ncbi.nlm.nih.gov/7261540/), ruling out the mechanical hyperventilation arm as a driver. [Voluntary hypocapnic hyperventilation in heated humans reduces forearm cutaneous blood flow](https://pubmed.ncbi.nlm.nih.gov/22972836/) — consistent with sympathetic dominance over any mediator-release mechanism, though mediators were not measured directly. No study has measured plasma histamine or serum tryptase in response to voluntary *hypocapnic* hyperventilation in humans. The clinical observation that hyperventilation syndrome and panic disorder involve cerebrovascular and sympathetic symptoms remains valid, but attributing them specifically to CO₂-granule-pH chemistry was overstated.

**Rationale:** This is the second most substantial edit. It replaces the misleading mechanism statement with the ATP/V-ATPase account, recontextualizes Pollard 1977 honestly (its pH-dependence operates during active exocytosis, not as spontaneous release), adds Strider 2011 with its supraphysiological dose caveat, and removes the Freed 2001 citation (which was about dry-air airway drying in dogs). The warning callout acknowledges the first-principles reasoning, the specific negative in vivo evidence (Barnes 1981, Fujii 2012), and the single empirical gap (no direct in vivo hypocapnic challenge + mediator measurement in humans).

---

### Edit 2.2 — "Self-reinforcing loop" paragraph

**Location:** Same section "CO2 as Active Protector", paragraph following "Hyperventilation as pathological CO2 depletion", currently line 75.

**Current text:**

> The self-reinforcing loop is critical: stress increases breathing rate, CO2 falls, hemoglobin holds oxygen tighter (Bohr effect in reverse), tissues become functionally hypoxic, the organism feels short of breath and breathes faster, CO2 falls further. Serotonin is released from platelets (pH rises when CO2 drops), histamine leaks from mast cells, cerebral vasoconstriction deepens. [Hyperventilation syndrome and panic disorder are clinically intertwined](https://pmc.ncbi.nlm.nih.gov/articles/PMC2937087/). The compensatory response worsens the condition. Meanwhile, the CO2 loss shifts enzyme kinetics toward glycolysis, increasing lactate production -- so hyperventilation simultaneously depletes the protective output and increases the pathological one.

**Proposed replacement:**

> The self-reinforcing loop is critical: stress increases breathing rate, CO2 falls, hemoglobin holds oxygen tighter (Bohr effect in reverse), tissues become functionally hypoxic, the organism feels short of breath and breathes faster, CO2 falls further. Cerebral vasoconstriction deepens as CO2 drops (2% CBF decrease per mmHg), and sympathetic activation produces the classic symptomatology of panic. [Hyperventilation syndrome and panic disorder are clinically intertwined](https://pmc.ncbi.nlm.nih.gov/articles/PMC2937087/). The compensatory response worsens the condition. Meanwhile, the CO2 loss shifts enzyme kinetics toward glycolysis, increasing lactate production — so hyperventilation simultaneously depletes the protective output and increases the pathological one. The coupling to mast cell and platelet mediator release that an earlier version of this passage proposed is now understood to operate via ATP → V-ATPase rather than via direct CO₂-pH chemistry — see "Mediator sequestration is ATP-dependent via V-ATPase" above.

**Rationale:** Removes the specific "serotonin from platelets (pH rises when CO2 drops), histamine leaks from mast cells" claim because it depends on the incorrect direct CO₂-pH-granule mechanism. Replaces with a defensible narrative (cerebrovascular + sympathetic — supported by Fujii 2012 and textbook CO₂ vasoreactivity). Adds an explicit pointer to the refined mechanism in the preceding subsection.

---

## Edits to `Foundation.md`

### Edit 3.1 — "When the fork goes right" paragraph

**Location:** Section "From First Principles", "The metabolic fork" subsection, paragraph starting "When the fork goes right", currently line 69.

**Current text:**

> When the fork goes right — toward CO₂ — the product actively sustains the conditions for more oxidation. CO₂ delivers oxygen to tissues (the Bohr effect shifts the hemoglobin dissociation curve rightward, releasing O₂ where CO₂ is high — which is where metabolism is active and oxygen is needed). CO₂ protects proteins from [cross-linking by reactive aldehydes](https://www.nature.com/articles/s41467-018-05475-z) via carbamino bond formation. CO₂ maintains the slightly acidic pH that keeps inflammatory mediators sequestered in storage granules. The output of successful metabolism creates the conditions for more successful metabolism.

**Proposed replacement:**

> When the fork goes right — toward CO₂ — the product and its co-produced cytosolic ATP together actively sustain the conditions for more oxidation. CO₂ delivers oxygen to tissues (the Bohr effect shifts the hemoglobin dissociation curve rightward, releasing O₂ where CO₂ is high — which is where metabolism is active and oxygen is needed). CO₂ forms carbamates on protein amine groups that [may compete with reactive aldehyde cross-linking](https://www.nature.com/articles/s41467-018-05475-z), though the protective magnitude has not been directly measured. Abundant cytosolic ATP — produced alongside CO₂ by oxidative phosphorylation in fixed stoichiometric coupling — powers V-ATPase-mediated maintenance of acidic granule pH in mast cells and platelets, keeping serotonin and histamine sequestered until stimulated release is needed. The output of successful metabolism creates the conditions for more successful metabolism.

**Rationale:** This is the `Foundation.md` analog of the mechanism refinement. The paragraph keeps its structure and voice but routes the mediator-sequestration claim through ATP/V-ATPase. It also tightens the carbamino claim (to match the existing warning in `The Metabolic Fork.md`) and makes explicit that CO₂ and ATP are co-produced by OXPHOS — which is what justifies using CO₂ as a reliable marker of the metabolic state even though it's not the causal variable in the mediator-sequestration mechanism.

---

## Edits to `Conservation Signaling.md`

### Edit 4.1 — "Shared Triggers" subsection

**Location:** Section "Shared Triggers", subsection currently headed "Alkaline pH from low CO2", lines ~52-58.

**This is a more substantial edit than the others in this proposal.** The Conservation Signaling document has a dedicated subsection built around the incorrect mechanism. It also correctly cites Nunomura 2017 (the V-ATPase paper) for granule pH dependence — meaning this document already has one arm of the refined mechanism, it just hasn't joined the dots to recognize that V-ATPase (not CO₂) is the maintainer. **Minor citation error noted:** the current text refers to Nunomura 2017 as a "Cell Reports study" but the actual paper is in Cell Death & Disease — correct this when applying the edit.

**Current text:**

> **Alkaline pH from low CO2.** This is the most fundamental shared trigger. Both serotonin and histamine are stored in acidic granules — serotonin in platelet dense granules, histamine in mast cell secretory granules. The storage mechanism is identical: at acidic pH, the molecule carries extra positive charges and binds tightly to the granule's proteoglycan matrix. When pH rises, it loses charge, detaches, and leaks out.
>
> For histamine, this has been demonstrated at the molecular level. A [2017 Cell Reports study](https://pmc.ncbi.nlm.nih.gov/articles/PMC5584528/) showed that mast cell granules require acidic pH to store histamine. When granule pH was raised, histamine lost one positive charge, detached from serglycin proteoglycans, and leaked into the extracellular medium — "a profound reduction in the ability of mast cells to store histamine intracellularly." This is not classical IgE-mediated degranulation. It is unregulated leakage from pH-disrupted granules. A person can have chronic histamine symptoms without any allergic trigger — simply from loss of the acidic environment that keeps histamine contained.
>
> For serotonin, platelet release is [dependent on hydroxyl ion transport — suppressed by acidic pH](https://pmc.ncbi.nlm.nih.gov/articles/PMC431691/). The same chemistry applies: acidic environment retains; alkaline environment releases.
>
> CO2 dissolved in body fluids forms carbonic acid, maintaining the acidic intracellular environment that keeps both molecules sequestered. When CO2 falls — from hyperventilation, hypothyroidism, or any shift from glucose oxidation to fat oxidation — pH shifts alkaline, and both serotonin and histamine are released simultaneously. As the chain runs: inadequate oxidative metabolism → less CO2 → alkaline pH → granule destabilization → serotonin and histamine released → both further suppress oxidative metabolism → even less CO2. The conservation program amplifies itself.

**Proposed replacement:**

> **Failing ATP and granule destabilization.** This is the most fundamental shared trigger. Both serotonin and histamine are stored in acidic granules — serotonin in platelet dense granules, histamine in mast cell secretory granules. The storage mechanism is identical: at acidic pH, the molecule carries extra positive charges and binds tightly to the granule's proteoglycan matrix. When granule pH rises, the molecule loses charge, detaches, and leaks out. The granule's acidic interior (pH ~5.3–5.5) is maintained by [V-ATPase](https://pubmed.ncbi.nlm.nih.gov/24165939/) — an ATP-dependent proton pump that holds the ~1.9-unit gradient against cytosol AND simultaneously acts as a pH sensor via V₁-V₀ dissociation. When cellular ATP falls, V-ATPase pumping slows, granule pH rises, and the V₁-V₀ sensor dissociates, coupling granule destabilization to release readiness.
>
> For histamine, this has been demonstrated at the molecular level. A [2017 Cell Death & Disease study](https://www.nature.com/articles/cddis2017206) showed that mast cell granules require acidic pH to store histamine. When granule pH was raised (via V-ATPase inhibition with bafilomycin A1), histamine lost one positive charge, detached from serglycin proteoglycans, and leaked into the extracellular medium — "a profound reduction in the ability of mast cells to store histamine intracellularly." This is not classical IgE-mediated degranulation. It is unregulated leakage from pH-disrupted granules. A person can have chronic histamine symptoms without any allergic trigger — simply from V-ATPase activity becoming inadequate to maintain granule acidity.
>
> For serotonin, platelet release is [pH-dependent during stimulated exocytosis via hydroxyl ion transport](https://pmc.ncbi.nlm.nih.gov/articles/PMC431691/). Pollard et al. 1977 demonstrated in vitro that when granules are juxtaposed to the plasma membrane during thrombin- or ionophore-triggered exocytosis, alkaline extracellular pH accelerates release via anion-transport-mediated osmotic lysis. This is a stimulated-exocytosis mechanism, not a spontaneous-release mechanism.
>
> The coupling from metabolic state to mediator release therefore runs through **ATP availability**, not directly through CO2/pH chemistry. CO2 production is a reliable marker of oxidative metabolism (OXPHOS co-produces CO2 and ATP in fixed stoichiometric coupling), but the causal variable that determines granule stability is cytosolic ATP powering V-ATPase. As the chain runs: inadequate oxidative metabolism → falling cytosolic ATP → V-ATPase pumping slows → granule pH rises → serotonin and histamine leak → both further suppress oxidative metabolism → even less ATP. [Hypoxia (1% O₂) increases mast cell histamine release](https://pubmed.ncbi.nlm.nih.gov/28553287/), consistent with this ATP-mediated mechanism. The conservation program amplifies itself.
>
> > [!warning] Mechanism refined; in vivo magnitude untested
> > An earlier version of this passage attributed granule acidity maintenance directly to "CO2 dissolved in body fluids forms carbonic acid, maintaining the acidic intracellular environment." That framing was mechanistically imprecise: granule interior pH is maintained against a ~1.9-unit gradient by active V-ATPase pumping, not by passive equilibration with extracellular CO₂-pH chemistry. [Isocapnic voluntary hyperventilation does not produce plasma histamine change in humans](https://pubmed.ncbi.nlm.nih.gov/7261540/), ruling out the mechanical hyperventilation arm. No study has measured plasma histamine or serum tryptase in response to voluntary *hypocapnic* hyperventilation in humans, so the in vivo magnitude of the refined ATP/V-ATPase mechanism at physiological metabolic variations remains empirically untested.

**Rationale:** This is the most substantial edit after Loop 7 itself. The subsection heading changes from "Alkaline pH from low CO2" to "Failing ATP and granule destabilization" because the active causal variable is ATP, not alkaline pH. The body of the subsection gains an explicit V-ATPase explanation (which the document didn't have, despite already citing the relevant Nunomura 2017 paper). The Pollard citation is recontextualized as stimulated-exocytosis-only. The causal chain is rewritten to run through ATP instead of CO₂, with CO₂ preserved as a marker. A warning callout makes the refinement explicit and flags the in vivo empirical gap. The small citation correction (Cell Reports → Cell Death & Disease) is folded in. This edit represents the "structural consequence for Layer 2" most visibly: the section that was built around CO₂-as-causal-driver is rebuilt around ATP-as-causal-driver, with CO₂ reframed as a marker.

---

## Edits to `The Preferred Substrate.md`

### Edit 5.1 — "Why Glucose: Maximum CO2 per Oxygen" subsection

**Location:** Section "Why Glucose: Maximum CO2 per Oxygen", paragraph starting "This matters because CO2 is biologically active", currently line 39.

**Current text:**

> This matters because CO2 is biologically active. It shifts the hemoglobin dissociation curve rightward (the Bohr effect), releasing oxygen precisely where metabolism is highest. It forms [carbamino bonds with proteins](https://www.nature.com/articles/s41467-018-05475-z), protecting them from reactive aldehyde damage. It maintains the slightly acidic intracellular pH that keeps inflammatory mediators sequestered in storage granules. Every function documented in [[The System]] that depends on CO2 is maximized when glucose is the primary oxidative substrate and diminished when fat replaces it.

**Proposed replacement:**

> This matters because CO2 is biologically active. It shifts the hemoglobin dissociation curve rightward (the Bohr effect), releasing oxygen precisely where metabolism is highest. It forms [carbamino bonds with proteins](https://www.nature.com/articles/s41467-018-05475-z) that may compete with reactive aldehyde damage (protective magnitude not directly measured). And CO2 production is a reliable marker of cytosolic ATP availability — because OXPHOS produces both CO2 and ATP in fixed stoichiometric coupling, CO2 output tracks with the ATP that powers V-ATPase-mediated maintenance of inflammatory mediator sequestration in mast cell and platelet granules. Every function documented in [[The System]] that depends on CO2 is maximized when glucose is the primary oxidative substrate and diminished when fat replaces it.

**Rationale:** Small edit — a single sentence replacement within a paragraph. Softens the carbamino claim to match the existing warning callout in `The Metabolic Fork.md`, and replaces the "maintains the slightly acidic intracellular pH that keeps inflammatory mediators sequestered" claim with the refined framing that CO₂ is a marker of ATP availability which powers V-ATPase. Preserves the broader argument that glucose oxidation maximizes CO₂/ATP output and that all CO₂-dependent functions benefit from glucose as substrate.

---

## Citation changes summary

**Remove entirely:**
- **Freed et al. 2001** ([AJRCCM 164.5.2003081](https://www.atsjournals.org/doi/full/10.1164/ajrccm.164.5.2003081)) — from `The Metabolic Fork.md` "Inflammatory mediator sequestration" paragraph. Reason: canine dry-air hyperventilation model; mechanism is airway drying/osmolality, not systemic CO₂/pH; measures bronchial reactivity to exogenous histamine, not endogenous release. Clear citation-vs-claim gap.

**Recontextualize (keep but reframe):**
- **Pollard et al. 1977** ([PMC431691](https://pmc.ncbi.nlm.nih.gov/articles/PMC431691/)) — move from "supports the claim that CO₂ maintains granule pH at rest" to "demonstrates pH-dependence during stimulated exocytosis via anion transport + osmotic lysis when granules are juxtaposed to plasma membrane." The paper is technically about pH-dependent release but operates in a specific physiological scenario that doesn't support the vault's original claim.

**Add as primary citations:**
- **Poëa-Guyon et al. 2013** ([PMID 24165939](https://pubmed.ncbi.nlm.nih.gov/24165939/)) — J Cell Biol 203(2):283-98 — V-ATPase V₀ domain as intragranule pH sensor; V₁-V₀ dissociation couples granule pH to exocytosis.
- **Nunomura et al. 2017** ([Cell Death & Disease, cddis2017206](https://www.nature.com/articles/cddis2017206)) — bafilomycin A1 inhibits V-ATPase, elevates mast cell granule pH, reduces intracellular histamine, increases extracellular histamine; acidic granule pH essential for sequestration.
- **Möllerherm et al. 2017** ([PMID 28553287](https://pubmed.ncbi.nlm.nih.gov/28553287/)) — Front Immunol 8:541 — 1% O₂ hypoxia increases mast cell histamine release; consistent with ATP-mediated V-ATPase impairment mechanism.
- **Barnes & Brown 1981** ([PMID 7261540](https://pubmed.ncbi.nlm.nih.gov/7261540/)) — Clin Sci 61(2):159-162 — isocapnic voluntary hyperventilation does NOT produce plasma histamine change in healthy or asthmatic humans; rules out mechanical hyperventilation arm as driver.

**Add with caveat:**
- **Strider et al. 2011** ([PMID 21284650](https://pubmed.ncbi.nlm.nih.gov/21284650/)) — Allergy 66(3):341-350 — 100% CO₂ suppresses mast cell degranulation via intracellular calcium repression. Cite with explicit note that this is supraphysiological (~20× alveolar CO₂) and has not been replicated or extended to physiological ranges in 14+ years.
- **Fujii et al. 2012** ([PMID 22972836](https://pubmed.ncbi.nlm.nih.gov/22972836/)) — voluntary hypocapnic hyperventilation reduces forearm cutaneous blood flow in heated humans; consistent with sympathetic dominance over mediator release but mediators were not measured. Include as indirect evidence against large-magnitude mediator mechanism.

---

## Review checklist for user

Before committing these edits, please verify:

- [ ] **Current text accuracy.** Cross-check each "Current text" block against the live vault files to ensure I've captured the exact current wording (I read them just before writing this proposal but verify).
- [ ] **Voice and tone match.** The proposed replacements should sound like the rest of the vault. Flag anything that reads awkwardly or introduces new jargon.
- [ ] **Warning callout scope.** The two warning callouts (Loop 7, Inflammatory mediator sequestration) are somewhat redundant — they say similar things in similar places. Consider whether both are needed, or whether one should reference the other.
- [ ] **Not over-claiming.** The refined mechanism is still a mechanistic hypothesis — better-supported than the original but not experimentally verified at physiological ATP variations. The proposed text tries to be honest about this; check that it's neither overstated nor understated.
- [ ] **Directional claims preserved.** The edits should preserve all the vault's directional claims (low metabolism → mediator activation → further suppression) while correcting the mechanism. Verify that practical recommendations (ETCO₂/V'CO₂ monitoring, addressing hyperventilation syndromes, etc.) remain intact.
- [ ] **Internal links.** Both warning callouts reference adjacent passages within each document — verify these cross-references are correct after the edits are applied.
- [ ] **The structural consequence for Layer 2's broader "CO₂ is an active product" claim** is acknowledged in the warning callouts but is not given a dedicated reframing paragraph. If you want the broader point made more prominently — e.g., a new subsection in `The Metabolic Fork.md` explaining that CO₂'s active role operates through multiple non-loop mechanisms rather than a formalized positive feedback loop — that would be a separate follow-on edit. I did not include it here because the warning callouts already communicate the key change; but it's a defensible addition if you want the structural retreat made more visible.

---

## What's NOT in this proposal (deferred)

1. **Broader reframing of "CO₂ is an active product" in Foundation.md's thesis statement and The Metabolic Fork.md's "CO₂ as Active Protector" section.** The warning callouts in the edits above communicate the key change, but if you want the structural retreat from "loop-supported active product" to "non-loop active mechanisms" made more explicit at the Layer 2 level, that's a separate edit.
2. **Independent verification of Bolevich & Kogan 2016** (CF-2.A.5). The "Free radical suppression (2-4x)" subsection in `The Metabolic Fork.md` still cites Bolevich & Kogan as the primary support for CO₂'s direct ROS-suppression claim. This subsection is unchanged by the current proposal. Verifying this claim independently is listed as carry-forward CF-2.A.5 and should happen before the vault leans more heavily on Bolevich & Kogan as compensation for Loop 7's structural retreat.
3. **Loop 6 (Thyroid-Everything) CO₂ arm scrutiny** (CF-2.A.1). Loop 6's "low CO₂ independently suppresses thyroid function further" uses a similarly unspecified mechanism. It may need the same refinement (ATP-mediated, CO₂-as-marker) but this has not been directly tested in Sub-test 2.A. Address in Layer 3 or as focused Sub-test 2.C.
4. **Changes to `Practice.md` or other documents.** If any downstream vault documents reference Loop 7 by name or cite the CO₂-pH mediator mechanism specifically, they may need parallel updates. A grep for "CO₂-Serotonin Loop" and related phrases across the vault is recommended before committing.
