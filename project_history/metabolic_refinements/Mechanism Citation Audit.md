---
title: "Mechanism Citation Audit"
aliases:
  - Citation Deployment Audit Results
  - Pass 1 Mechanism Audit
last-updated: 2026-04-12
source: "Post-stress-test citation deployment audit across all 9 mechanism documents"
scope: audit
---

A systematic citation deployment audit of all 9 mechanism documents in `metabolic_foundations/`, applying the CF-2.A.4 four-dimension check (species / scenario / endpoint / proposed-mechanism match) to every load-bearing citation. This audit brings the mechanism documents to stress-test-level verification on citation accuracy — complementing the structural verification performed in Layers 1-3.

## Summary

| Document | Load-bearing citations | CLEAN | FLAGGED | UNCERTAIN | Uncited claims |
|---|---|---|---|---|---|
| The Master Throttle | 15 | 8 (53%) | 4 (27%) | 3 (20%) | 4 |
| Membrane Damage and Defense | 21 | 20 (95%) | 1 (5%) | 0 | 5 |
| The Hormonal Axis | 36 | 30 (83%) | 3 (8%) | 2 (6%) | 7 |
| Conservation Signaling | 40 | 31 (78%) | 5 (13%) | 3 (8%) | 4 |
| The Gut-Liver Axis | 16 | 5 (31%) | 3 (19%) | 4 (25%) | 6 |
| The Preferred Substrate | 23 | 21 (91%) | 1 (4%) | 0 | 7 |
| The Metabolic Fork | 24 | 13 (54%) | 3 (13%) | 8 (33%) | 3 |
| The Cellular Readout | 18 | 12 (67%) | 2 (11%) | 4 (22%) | 5 |
| The Temporal Dimension | 28 | 22 (79%) | 2 (7%) | 4 (14%) | 7 |
| **TOTAL** | **221** | **162 (73%)** | **24 (11%)** | **28 (13%)** | **48** |

Note: The Metabolic Fork's high UNCERTAIN rate (33%) is mostly from inaccessible URLs (403/303 errors), not substantive concerns.

## Confirmed errors (Pass 2 primary-source verified)

### Error 1 — Ca + Vit D fracture reduction claim contradicted by its own citation

**Document:** The Cellular Readout
**Claim:** Ca + Vit D supplementation produces 15% total fracture reduction and 30% hip fracture reduction.
**Citation:** PMC12506016
**What the paper actually says:** The paper's OWN meta-analysis of 11 RCTs (43,869 postmenopausal women with osteoporosis) found NO significant fracture reduction (RR 0.95, CI 0.85-1.07, p=0.28). The 15%/30% figures come from an older NOF meta-analysis (PMC4715837, Weaver et al. 2016) that the paper merely references — and the paper's primary finding disagrees with those numbers.
**Severity:** HIGH — the cited paper contradicts the claim. This affects a practical recommendation about supplementation.
**Fix needed:** Replace citation with the NOF meta-analysis (PMC4715837) that actually supports the numbers, AND note the PMC12506016 contradicting finding. Or revise the claim to reflect the mixed evidence.

### Error 2 — Ringer's lactate: wrong paper cited

**Document:** The Metabolic Fork
**Claim:** "Ringer's lactate potentiates neutrophil activation and pulmonary inflammation in severe hemorrhagic shock resuscitation."
**Citation:** PMID 17414340
**What the paper actually says:** Todd et al. 2007 compared NS vs LR in swine hemorrhagic shock and found LR was SUPERIOR to NS (less volume, less coagulopathy, less acidosis). The paper does NOT discuss neutrophil activation or pulmonary inflammation.
**Correct citations:** PMID 17215740 (Alam et al. — hypertonic saline + pentoxifylline reduces RL-associated neutrophil activation and pulmonary inflammation) or PMID 16456435 (HSPTX as alternative to RL, discussing RL's inflammatory effects).
**Severity:** MEDIUM — the claim itself is likely correct (supported by other papers), but the cited paper is simply wrong.
**Fix needed:** Replace PMID 17414340 with the correct paper(s).

### Error 3 — Reverse T3 receptor binding: non-peer-reviewed claim

**Document:** The Master Throttle
**Claim:** Reverse T3 "binds to T3 receptors without producing metabolic effects," competing with active T3.
**Citation:** Restorative Medicine journal (non-peer-reviewed integrative medicine publication)
**What peer-reviewed literature says:** Halsall & Oddy 2021 (Annals of Clinical Biochemistry) explicitly states: "It is frequently claimed in articles published on the internet, but not in peer-reviewed papers, that reverse T3 blocks or 'gets in the way of' the nuclear thyroid receptors." rT3 binding affinity at nuclear receptors is at least 200-fold weaker than T3, making competitive inhibition at physiological concentrations implausible. The REAL mechanism: rT3 competitively inhibits DIO1 (type 1 deiodinase), impairing T4→T3 conversion. This is a different and peer-reviewed mechanism.
**Severity:** HIGH — the claim as stated is not supported by peer-reviewed research. The document builds a causal chain (high rT3 → blocks T3 at receptors → functional hypothyroidism) that peer-reviewed literature does not support. The correct mechanism (rT3 inhibits DIO1) produces the same clinical picture (impaired T3 production) but via a different pathway.
**Fix needed:** Replace the nuclear-receptor-binding claim with the DIO1-competitive-inhibition mechanism. Replace the citation with Halsall & Oddy 2021 or the primary DIO1 kinetics literature.

### Error 4 — PTH mast cell activation: supraphysiological dose

**Document:** The Cellular Readout
**Claim:** PTH triggers mast cell degranulation, releasing serotonin and histamine. Deployed in a causal chain: dietary Ca deficiency → moderate PTH elevation → mast cell activation → mediator release.
**Citation:** PubMed 6191761
**What the paper says:** PTH induces serotonin and histamine release from RAT peritoneal mast cells at 25 units/ml — explicitly described as "within the higher limits of the elevated PTH levels found in advanced uremia." The effect is dose-dependent: lower concentrations produce less or no release.
**The gap:** The framework's causal chain (dietary deficiency → moderate PTH → mast cells) requires the effect at MUCH lower PTH concentrations than the paper tested. The paper tested pathological levels (advanced uremia range), not moderate dietary-deficiency levels. Also: rat species, not human.
**Severity:** MEDIUM — the mechanism is real at high concentrations but the causal chain as deployed may overclaim the relevance to dietary-level PTH elevations.
**Fix needed:** Add dose qualifier ("at pathological concentrations") and species qualifier ("in rat mast cells"). Note that the relevance to moderate dietary PTH elevation is undemonstrated.

## Reclassified (not errors — text should add nuance)

### LPS and deiodinase direction (The Master Throttle)

**Claim:** LPS suppresses T3 / alters deiodinase activity.
**Citation:** PMC12171323 + related literature
**What the literature shows:** LPS activates D2 (type 2 deiodinase) in hypothalamic tanycytes, increasing LOCAL T4→T3 conversion in the mediobasal hypothalamus. This increased hypothalamic T3 drives TRH suppression → TSH suppression → central hypothyroidism. At the whole-organism level, LPS DOES suppress thyroid function — but via the paradoxical route of activating local D2, not via simple direct suppression. The document's claim "LPS suppresses T3" is correct at the organism level; the mechanism is more nuanced than implied.
**Fix needed:** Add the D2 activation mechanism explicitly. Note that LPS-driven T3 suppression operates via increased hypothalamic D2 → local T3 → TRH suppression, not via direct D1 inhibition alone.

## Error pattern

The confirmed errors cluster into the same categories the structural stress test predicted:

| Error type | Count | Examples |
|---|---|---|
| Citation contradicts claim | 1 | Ca+VitD fracture |
| Wrong paper cited | 1 | Ringer's lactate |
| Non-peer-reviewed source for mechanistic claim | 1 | rT3 receptor binding |
| Dose/scenario mismatch (supraphysiological → physiological) | 1 | PTH mast cell |
| Species extrapolation (rat → human without qualifier) | ~12 | Across multiple documents |
| Causal attribution beyond citation scope | ~6 | Across multiple documents |
| Direction reversal | 1 | PMC6624793 serotonin-lipolysis (known from stress test) |

**The stress test's CF-2.A.4 prediction holds at the mechanism level:** citation deployment errors cluster at bulk-effect mechanisms with non-molecular citations. The 4 confirmed errors all involve claims where the mechanism is stated at a level of generality that doesn't match the citation's specific context.

## Uncited framework-specific claims (48 total)

These fall into two categories:

**Integrative interpretations (~30):** Claims like "these loads are not additive, they are multiplicative," "the nightly conservation program," "MCAS as metabolic failure." These synthesize across multiple individually-cited facts and don't have individual citations because they ARE the integration. Not errors — they are the framework's intellectual contribution. Should be labeled as framework interpretation where they aren't already.

**Specific quantitative or mechanistic claims without citation (~18):** Examples include "fructose accelerates ethanol oxidation by ~80%," "T3 supports dopamine synthesis," "PUFA more potent inhibitors of glucose oxidation than saturated fats," "estrogen increases intestinal permeability." These need either citations or "framework interpretation" qualification.

## Impact on the structural architecture

**None.** The 4 confirmed errors, the ~12 species-extrapolation issues, the ~6 causal-attribution stretches, and the 48 uncited claims are all mechanism-level precision issues. None affect:
- The ontological claim (health IS oxidative metabolism)
- The 10-loop architecture or the causal-independence classifications
- The conditional bistability finding
- The state-dependent damping insight
- The six testable predictions

The structural stress test (Layers 1-3) and this citation audit test different things: the stress test tested whether the architecture's LOGIC is sound; the citation audit tested whether the mechanism documents' EVIDENCE DEPLOYMENT is accurate. The architecture is sound. The evidence deployment is 73% clean, 11% flagged, with 4 confirmed errors needing correction.

## Documents ranked by citation quality

| Rank | Document | Clean rate | Action needed |
|---|---|---|---|
| 1 | Membrane Damage and Defense | 95% | Fix known PMC6624793 error only |
| 2 | The Preferred Substrate | 91% | Fix carbamino/aldehyde extrapolation; add ketone body coverage |
| 3 | The Hormonal Axis | 83% | Add species qualifiers to 3 citations |
| 4 | The Temporal Dimension | 79% | Note melatonin dual identity; qualify PUFA-light extrapolation |
| 5 | Conservation Signaling | 78% | Replace 2 non-peer-reviewed sources; add species qualifiers |
| 6 | The Cellular Readout | 67% | Fix Ca+VitD contradiction; qualify PTH dose; add 5 citations |
| 7 | The Metabolic Fork | 54% | Fix Ringer's wrong paper; verify inaccessible citations |
| 8 | The Master Throttle | 53% | Fix rT3 claim; add LPS/D2 nuance; add species qualifiers |
| 9 | The Gut-Liver Axis | 31% | Add glucuronidation species qualifier; cite antibiotic hormonal claim; replace blog source |
