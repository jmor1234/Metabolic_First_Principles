# Metabolic Framework

A multi-phase, multi-agent research project I designed and orchestrated to answer one question from first principles: *what IS health, and what IS disease, at the deepest resolution biology currently allows?* The output is a 14-document knowledge vault. **This README is about the work, not the biology** — the strategy, the design decisions, the discipline I built into the system, and what I learned about doing rigorous research with agents.

## What I Built and Why

I wanted to see what's possible when AI agents are used as the execution layer of a deliberately designed research system, rather than as a single model responding to a prompt. The domain — metabolic biology — was chosen for three reasons: it offered substantive first-principles questions; a coherent existing framework (Ray Peat's body of work) was broad, mechanistic, and accessible for systematic extraction; and the field is fragmented enough across specialties that integrating across them was itself useful work.

**All research, claim verification, source-level citation work, and adversarial stress testing was executed by AI agents. I designed the workflows, directed the campaigns, held the framework context throughout, and made every load-bearing synthesis decision.** The vault is the output of an agentic system I built and ran across multiple phases and stress-testing campaigns — not a single model run on a prompt.

## Core Strategic Decisions

Key design choices that shaped the project:

**1. Use a coherent starting framework as a vehicle, not a destination.** I needed something to test against rather than fragments to assemble from scratch across dozens of specialties. Peat's work was the most coherent first-principles integration of metabolic biochemistry publicly available. The project was designed to verify, refine, and where necessary correct his positions — not confirm them. The final vault contains structural insights Peat never articulated and removes claims that did not survive verification.

**2. Sequence the work in phases, never overwrite a prior phase.** Four sequential phases (verify → extract → stress test → unify), each leaving the prior phase intact and traceable. Original verification work, the pre-stress-test snapshot, the stress test logs, the refinement diffs — all preserved in `project_history/`. Any current claim can be traced back through its full evidence chain. If a refinement turns out wrong, the prior position is recoverable.

**3. Hold refinements as a separate layer before merging.** When stress testing produced corrections, I did not silently overwrite the foundations. I built `metabolic_refinements/` as a parallel epistemic layer with its own audit trail, and only merged into the unified vault once each refinement passed classification. This separated the work of *finding* corrections from the work of *accepting* them, because agents can produce coherent-sounding revisions that should not flow directly into the canonical artifact.

**4. Default to the asymmetry principle.** The cost of wrongly changing a hard-built integration is higher than the cost of wrongly leaving it unchanged. Integrations are expensive to build and cheap to degrade; a wrong non-change can be revisited later when evidence is clear. So the default is: the vault is correct until proven otherwise with verified evidence that survives deep reading. The bar for change is high, deliberately.

## How I Designed the Discipline

Two opposing failure modes had to be guarded against simultaneously:

- **Defending the framework unfairly.** Built-in explanatory resources (acute/chronic distinctions, context-dependence) can absorb any counterexample if allowed to flex after the fact, making the framework unfalsifiable.
- **Changing the framework on shallow understanding.** Apparent contradictions frequently dissolve under deep reading. In stress testing this turned out to be the more common failure — agents produced confident-sounding "corrections" that were actually misreadings of what the framework already said.

Guardrails against both:

- **Three interpretive rules** constraining when the framework's explanatory resources can be invoked — for example, requiring that any acute/chronic distinction be grounded in observable control architecture (programmatic entry, intact termination, repair-bounded damage, baseline return) rather than in the outcome it's trying to explain. Classifying by outcome is circular; the rules forbid it.
- **Three hypotheses checked in order** whenever research appears to contradict the vault: (1) you are misunderstanding the vault, (2) the research measures something different, (3) the vault is wrong. Agents kept skipping to #3. The sequence is formalized in the methodology.
- **A six-step verification sequence** for any proposed change, with two audits at its core: a *causal-independence audit* (Pearl's screening-off test plus Metabolic Control Analysis conservation relations) for distinguishing genuinely independent causal variables from parallel markers, and a *citation-deployment audit* (species / scenario / endpoint / proposed-mechanism match) that checks whether a paper actually supports the specific claim it's being deployed for.

Each guardrail was added in response to a specific failure mode observed in the work itself.

## How I Designed the Agentic System

Division of labor between me and the agents:

**My work:**
- Designed the workflows — the three-phase per-topic verification process, the multi-campaign stress testing structure, the refinement-document templates, the verification sequence, the classification rules, the audits
- Directed the campaigns — what to test, which load-bearing claims to stress, when a refinement was ready to merge, when an apparent contradiction needed deeper investigation versus accommodation
- Held the synthesis — integration across campaigns and topics required someone holding the full framework picture

**The agents' work, under the discipline:**
- Primary-source extraction of original positions
- Real-time literature verification (PubMed / DOI / institutional sources — never training data)
- Independent triangulation on load-bearing claims (multiple agents on the same question separately, then convergence comparison)
- Stress testing campaigns with structured outputs (live investigation logs, refinement diff catalogs, classified outcome documents)
- Citation-deployment audits

**What I learned, codified into the methodology:** delegation works for narrow retrieval (specific lookups, replication checks, factual values, "has X been confirmed?"). It fails for evaluation that requires framework context — agents produce coherent-sounding narratives that have to be un-accepted before they corrupt the synthesis. The verification methodology document (`metabolic_framework/Verification Methodology.md`) codifies the operational distinction between what to delegate and what to keep.

## What This Project Demonstrates

Beyond the metabolic content, three things:

**Rigor.** A framework explicitly designed to be corrected, with the bar for correction set high deliberately. Every specific claim has a verifiable PubMed/DOI source — training data and general knowledge do not count. Every refinement traceable to its evidence chain. Confidence calibrated at two levels (document and individual claim). Honest about what's textbook versus probable versus speculative — every document has a "Where the Evidence Is Complex" section.

**System design.** A multi-phase, multi-campaign agentic research workflow that produced traceable, auditable outputs at every stage. The methodology was developed by doing the work and refined as I learned what agents could and could not be trusted with. The artifacts — methodology documents, verification sequences, audit templates, the refinement layer architecture — generalize beyond this domain.

**Integration across disciplines.** The vault connects findings from endocrinology, hepatology, oncology, neurology, cell biology, and immunology into one coherent picture. Mechanism-level confirmations from independent fields not citing each other (ferroptosis 2012, histone lactylation 2019, NASH drug approval 2024, bariatric remission hysteresis, Tabak 2009 critical slowing down, 670nm Complex IV activation 2024) all support pieces of the same architecture.

## Where to Look

- **5-minute orientation** — `essence/Essence.md` (13 first principles)
- **30-minute conceptual picture** — `metabolic_framework/Foundation.md` then `metabolic_framework/The System.md`
- **The discipline** — `metabolic_framework/Verification Methodology.md`
- **How the project moved through its phases** — `project_history/Overview.md`
- **Honest accounting of the starting framework** — `Ray Peat — Historical Assessment.md`

---

The framework is designed to be corrected. Corrections are features, not failures. The bar is high because integrations are expensive to build and cheap to degrade.
