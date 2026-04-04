---
title: "Audit: Phase 2 Integrity Gap"
tags:
  - structural/audit
  - framework/peat
role: structural-note
---

# Audit: Phase 2 Integrity Gap

## What We Found

During production of the histamine topic document (April 2026), we discovered that Phase 2 (Research Context) had been written entirely from the agent's training knowledge rather than from real-time research of primary sources. The Phase 2 section contained confident, well-structured, plausible-sounding claims about the research landscape — market sizes, diagnostic timelines, prevalence rates, what clinical workups include or exclude — that were presented as factual but had not been verified against any source.

When we actually researched the Phase 2 claims against current literature, several were wrong or misleading:

- **MCAS diagnostic timeline** was stated as "formally proposed in 2007, criteria published 2012-2016." The actual timeline: Akin et al. 2010 initial proposal, Valent et al. 2012 first criteria, Vienna Consensus Group refinement 2019-2021 (Valent et al. 2019, Gulen et al. 2021).
- **Dietary vs. endogenous histamine proportions** were stated as "dietary is a minor contributor" — presented as fact. The actual literature does not quantify the relative proportions. This unsourced claim would have led Phase 3 to dismiss dietary restriction research as addressing a "minor variable."
- **The PUFA-mast cell relationship** was presented as straightforward destabilization. Actual research shows intact n-3 PUFAs can reduce IgE-mediated degranulation through lipid raft disruption (opposite direction), while PUFA peroxidation products trigger degranulation through a different mechanism. The complexity would have been missed.
- **Specific claims about what standard clinical workups include or exclude** were stated without checking actual diagnostic guidelines.

The corrected Phase 2, built from fetched sources with linked citations, produced a materially different interpretive framework that changed how Phase 3 evidence was read and assessed.

## Why This Matters

Phase 2 is not supplementary context. It is the interpretive lens through which all Phase 3 evidence is read. It determines:

1. **Which studies are considered relevant** — a wrong claim about what comparison the research makes leads the agent to search for the wrong studies or dismiss the right ones.
2. **How contradictory evidence is weighted** — a wrong claim about funding incentives leads the agent to over- or under-discount specific findings.
3. **Whether a finding is assessed as confirmed vs. nuanced vs. overstated** — a wrong claim about timescale or endpoint issues leads to miscalibrated assessment.
4. **Which disciplinary silos are searched** — a wrong claim about fragmentation patterns leads to missed evidence in fields not identified.
5. **What the reader takes away** — research context framing shapes how every verification section is understood, even by human readers who trust the methodology.

A slightly wrong Phase 2 does not produce obviously wrong Phase 3 conclusions. It produces subtly tilted conclusions that cannot be distinguished from sound ones without re-examining the evidence through a corrected lens. This is worse than an obviously wrong analysis because it passes inspection.

## The Scope of the Problem

The seven topic documents completed before histamine — PUFA, thyroid, estrogen, progesterone, serotonin, CO2, and lactate — were all produced before the Phase 2 research requirement was established. Their Phase 1 content (extraction from Peat's primary articles on raypeat.com) is sound — it was built from fetched primary sources. Their Phase 3 verification sections contain linked citations to peer-reviewed papers, so the individual study references are real.

But the interpretive framework through which those studies were selected, read, and assessed was built from agent training knowledge, not from verified research of the actual research landscape. This means:

- **Research context framing** (who funds the research, what comparisons are made, what timescales are studied, what endpoints are measured, what disciplinary fragmentation exists) was likely generated from training data in all seven documents.
- **Contextual commentary within verification sections** — the paragraphs that explain *why* a study's framing matters, *why* a comparison is misleading, *why* an endpoint is the wrong one — was shaped by the unverified Phase 2 lens.
- **"What Makes This Topic Different" sections** contain meta-observations about the research landscape that may rest on unsourced claims.
- **Assessment calibration** — whether a claim was rated "confirmed," "confirmed with nuance," "partially supported," or "overstated" — was determined by reading evidence through a lens that may have been tilted.

### Highest-Risk Areas by Document

| Document | Highest-Risk Phase 2 Content |
|---|---|
| **Serotonin** | Pharmaceutical incentive narrative (SSRI revenue claims, German FDA Prozac rejection, suppressed alternatives framing). Some is sourced (Moncrieff review), some is likely training-data framing. |
| **Progesterone** | Bioidentical vs. synthetic progestin callout (WHI claims, MPA vs progesterone, patent economics). Directionally likely correct but specific claims may be unsourced. |
| **Thyroid** | "Anti-thyroid environment" framing, Synthroid market dominance, TSH testing infrastructure narrative. |
| **PUFA** | Historical consumption shift specific numbers, Burr experiment critique details, seed oil industry claims. |
| **Lactate** | "Lactate shuttle rehabilitation" framing, sports performance industry influence claims. |
| **CO2** | Mainstream framing of CO2 as waste product, claims about how permissive hypercapnia is viewed. |
| **Estrogen** | HRT industry framing, claims about how tissue-bound estrogen is measured or not measured in clinical practice. |

## What We Have to Do

### The Principle

Phase 1 (extraction from Peat's primary sources) is retained. It does not depend on an interpretive framework — it is reconstruction of stated positions from fetched primary articles.

Phases 2 and 3 must be redone for all seven existing documents. Phase 3 cannot be selectively retained because its conclusions were reached through an unverified Phase 2 lens. The only way to restore epistemic integrity is to rebuild from Phase 2 up:

1. **Retain Phase 1** for each document (Peat's Position sections, direct quotes, reasoning chains, first-principles logic).
2. **Delete Phase 2 content** (research context framing, contextual commentary, "What Makes This Topic Different" in its current form).
3. **Delete Phase 3 content** (Verification sections, assessment callouts, research citations, Sources sections).
4. **Redo Phase 2** with real-time research — every factual claim about the research landscape verified against fetched primary sources, per the updated methodology.
5. **Redo Phase 3** through the corrected Phase 2 lens — re-search, re-read, re-assess with the verified interpretive framework.
6. **Update structural documents** (System Overview assessment table, Practical Convergence if needed) to reflect any changed assessments.

### Execution Order

The documents should be redone in the original production order (PUFA, estrogen, progesterone, thyroid, serotonin, CO2, lactate) because later documents reference earlier ones. If an earlier document's assessment changes, downstream references need updating.

### What This Does NOT Mean

- It does not mean the existing conclusions are wrong. Many or most are likely correct.
- It does not mean the cited studies are invalid. The individual paper references are real and linked.
- It means we cannot distinguish which conclusions are sound from which were shaped by a tilted framing, and a knowledge base that cannot make that distinction does not meet its own stated standard of fidelity.

## Methodology Update

The methodology document (`methodology.md`) has already been updated with:

1. A new critical rule at the top of Phase 2: "Phase 2 must be researched, not inferred."
2. An expanded principle: "Context before content — but context must be researched, not assumed."
3. A new item (#6) in the Phase 2 checklist: verify what the modern literature actually says about mechanisms the framework identifies before assuming they are unstudied.

These changes prevent the same error in future topic production. This audit document records the discovery and the remediation plan for the existing documents.

## Status

- [x] Gap identified (during histamine document production, April 2026)
- [x] Methodology updated to prevent recurrence
- [x] Histamine document produced under corrected methodology
- [x] PUFA — Phases 2 and 3 redone. Key changes: MDA-Complex IV evidence now noted as mixed across tissues. Thyroid displacement nuanced (attenuated in vivo by albumin). Fish oil metastasis reclassified as cancer-type-specific (colon promotes, breast inhibits). SHBG displacement classified as debated rather than confirmed. Membrane pacemaker bird data acknowledged. Research context sourced with $100B+ market data, AHA-P&G history, 2025 JMA meta-analysis, DGAC conflicts.
- [ ] Estrogen — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] Progesterone — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] Thyroid — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] Serotonin — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] CO2 — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] Lactate — Phase 3 stripped, Phase 1 retained. Phases 2 and 3 to be redone.
- [ ] System Overview — Update assessment table after all redos complete
- [ ] Practical Convergence — Review for any changes after all redos complete
