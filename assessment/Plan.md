---
title: "Layer 2 Assessment Toolkit — Charter and Build Plan"
aliases:
  - Layer 2 Charter
  - Assessment Toolkit Plan
  - Layer 2 Build Plan
tags:
  - framework/metabolic
  - assessment/charter
  - layer/2
role: charter
scope: layer-2-foundational
last-verified: 2026-05-01
connections:
  - "[[Project Orientation]]"
  - "[[metabolic_framework/Foundation|Foundation]]"
  - "[[metabolic_framework/The System|The System]]"
  - "[[metabolic_framework/Practice|Practice]]"
---

# Layer 2 Assessment Toolkit — Charter and Build Plan

> [!abstract] Purpose
> Derive the universal Layer 2 toolkit — the questions, at-home markers, and lab tests that map any individual onto the bistable metabolic landscape Layer 1 describes — directly from Layer 1, ranked along the cost-utility-practicality frontier. The toolkit is universal across people; only the readings it produces are individual.

---

## The Four Layers — Where This Fits

The metabolic project decomposes into four conceptually distinct but operationally entangled layers:

| Layer | What it is | Universal vs Individual |
|---|---|---|
| **1 — Truth** | What health and disease ARE at the deepest resolution biology allows: mechanisms, attractors, feedback architecture, state-dependent damping, dual lock-in, daily oscillation. Lives in `metabolic_framework/`. | Universal — same for every human |
| **2 — Assessment** | How to map *this* person onto the Layer 1 landscape. The questions, at-home markers, lab tests, and the logic for reading them. **This directory.** | **Toolkit universal; readings individual** |
| **3 — Practice** | How to fit the Layer 1+2-optimal plan into this person's actual life: time, money, family, work, identity, motivation. | Individual |
| **4 — Dynamics** | How all of the above evolve. Layer 1 improves as evidence accumulates. Layer 2 readings shift as state changes. Layer 3 reality changes as life changes. | Process universal; trajectory individual |

Each layer constrains the layer above. Layer 4 determines whether Layer 3 stays calibrated. Layer 3 determines whether Layer 2 measurements ever get acted on. Layer 2 determines whether Layer 1 principles are correctly applied to *this* person. Layer 1 determines what's even worth measuring at Layer 2.

The structural insight that motivates this directory: **the Layer 2 toolkit is itself derivable from Layer 1.** What questions to ask, what physical markers to track, what labs to order are forced by which Layer 1 mechanisms have observable signatures. Different people produce different readings using the same instrument.

---

## What Layer 2 Has To Do

Two distinct jobs, currently conflated in existing materials:

1. **Initial state estimation (mapping).** Determine where this person currently sits on the bistable landscape. Which subsystems are functioning, which are impaired, which attractor are they in, how deep, are slow variables already structurally locked in. Broad, deep, one-time-ish.
2. **Ongoing trajectory tracking.** Detect movement after intervention. Are they shifting toward the healthy attractor? At what rate? Which subsystems are responding? Recurring, narrower, cadence-matched.

These need different toolkit configurations. The first emphasizes coverage and depth; the second emphasizes cadence and signal-to-noise.

---

## How We Got Here

A trace of the reasoning that produced this charter, so future readers understand the *why*:

1. **Foundational reading.** Project Orientation, Essence, the metabolic_framework CLAUDE.md, Foundation, The System, Practice. Established the Layer 1 picture: efficient oxidative metabolism IS health; two attractors when parameters create a disease basin; state-dependent damping unifies feedback failure across systems; dual lock-in; daily oscillation as temporal expression.
2. **Articulated the four-layer model.** Recognized the project decomposes into truth (Layer 1) → state estimation (Layer 2) → fitted practice (Layer 3) → dynamics over time (Layer 4).
3. **Identified the universal/individual split inside Layer 2.** What differs between people is the *readings*, not the *toolkit*. The instrument is universal and derivable from Layer 1. This made Layer 2 a tractable construction problem.
4. **Read Practice.md's monitoring framework** as the closest existing artifact to a Layer 2 toolkit in the vault.
5. **Critically analyzed Practice.md's monitoring section.** Identified what's strong (the bones to keep) and what's missing (the gaps that justify this directory).
6. **Established the build plan below.** Six steps, derived directly from the gaps.

---

## Critical Analysis of the Existing Monitoring Framework

### What's strong (the bones to keep)

- **Fork-position anchor.** CO₂ vs. lactate is the right master readout because they *are* the two products of the metabolic fork, not proxies.
- **Temperature + pulse as a 2D diagnostic.** The 3-state grid (warm+moderate / warm+fast / cold+slow) catches adrenaline compensation — the most common false positive in metabolic assessment.
- **The meal test.** Highest signal-per-cost item available. Free, 5 minutes; reveals whether the organism can mount thermogenesis or is running on stress hormones.
- **Honest calibration of standard workups.** TSH ≠ tissue thyroid; blood estrogen ≠ tissue estrogen; LFTs measure damage not function. Correctly named.
- **RQ = 0.75–0.8 in adequate-carb state = Randle blockade.** Sharp Layer 1→2 mapping; "metabolic inflexibility" *is* a chronically low RQ.

### What's missing or underdeveloped

1. **List, not system.** Markers presented individually; no combinatorial logic for which markers triangulate which subsystem, no signature-recognition rule, no disambiguation matrix.
2. **Questions tier essentially absent.** Jumps from free physical measures to clinical labs, skipping the entire history/symptom layer that is *cheaper than free* and often the most pattern-revealing: cold extremities, morning energy onset latency, postprandial fog, sleep-onset and 3 AM awakening pattern, cold/heat tolerance, stool form/transit, tongue coating, hair/nail/skin quality, cycle regularity, PMS severity, libido, recovery from exercise, afternoon crash timing, cognitive sharpness curve.
3. **Sensitive labs missing or underspecified.** Free T3 / Reverse T3 / Free T4 (the doc says "TSH bad" but doesn't specify what to actually measure); fasting insulin / HOMA-IR; GGT (most metabolically informative liver enzyme); ferritin (iron load = peroxidation catalyst); hs-CRP; triglyceride:HDL ratio; RBC magnesium (serum useless); 4-point cortisol curve; full sex hormone panel with SHBG; homocysteine; uric acid; 25-OH vitamin D.
4. **No cost-utility ranking.** Free vs. clinical is binary; no information-per-dollar continuum.
5. **No cadence specification.** Daily / weekly / monthly / quarterly capture rhythms not specified per marker.
6. **No state-dependent interpretation rule.** Cortisol high in early stress, blunted in late burnout — same biology, opposite reading. Practice.md interprets at face value, reproducing the false-contradiction risk the vault warns against.
7. **Wearables / continuous data not addressed.** HRV, CGM, sleep staging — increasingly cheap, often near-zero marginal cost, currently absent.
8. **Monitoring vs. mapping conflation.** Framed as "How to Know If It's Working" — verification of intervention, not initial state estimation. Two distinct toolkit configurations needed.
9. **Time-of-day / posture / conditions unspecified.** Pulse on waking ≠ pulse mid-afternoon. Targets given without protocols that make targets reliable.

---

## The Build Plan

Six steps, in order. Each step's output feeds the next.

### Step 1 — Subsystem Inventory from Layer 1

List every Layer 1 mechanism that has any observable signature. Approximate row vector to refine: thyroid sufficiency, oxidative throughput, glycolytic shift, PUFA tissue burden, iron status, gut barrier integrity, liver clearance capacity, calcium handling, circadian phase / morning-reversal capacity, mediator load (serotonin/histamine), HPA axis dynamics, sex hormone ratio (E/P), mitochondrial respiratory capacity directly, structural lock-in indicators (dynamical-vs-irreversible distinction).

**Deliverable:** `assessment/Subsystems.md` — the canonical row vector Layer 2 must estimate, each subsystem cross-referenced to its Layer 1 mechanism document.

### Step 2 — Marker Derivation per Subsystem

For each subsystem, exhaustively list every marker that legitimately informs it across four tiers:
1. Questions / history / symptom inventory
2. At-home physical / wearable
3. Cheap labs (sub-$200 panels)
4. Specialized labs (sub-specialty panels, advanced imaging, functional testing)

Each marker traced to the specific Layer 1 mechanism it reflects.

**Deliverable:** `assessment/Markers.md` — exhaustive marker list per subsystem with mechanism trace.

### Step 3 — Marker Properties Matrix

For each marker, specify:
- Subsystem(s) informed (primary vs. secondary)
- Cost (dollars)
- Cadence (daily / weekly / monthly / quarterly / one-time)
- Signal-to-noise (high / moderate / low)
- Capture protocol (time of day, posture, conditions, fasting state)
- State-dependent interpretation rule (does it behave differently in early vs. late disease?)
- Use case (mapping / tracking / both)
- Reporter reliability tier (objective instrument / objective at-home / reported / interpreted)

**Deliverable:** `assessment/Marker Properties.md` — the canonical matrix.

### Step 4 — Triangulation Logic

Disambiguation: which combinations of markers identify which specific subsystem failures, and which patterns are diagnostic of which attractor states.

Example: *low temp + fast pulse + low ETCO₂ + 3 AM awakening + cold extremities + GGT > X → high probability of [specific subsystem failure pattern].*

**Deliverable:** `assessment/Triangulation.md` — pattern recognition rules.

### Step 5 — Cost-Utility Frontier Ordering

A canonical assessment sequence: what to capture first (free, high-signal questions + T/pulse/meal test), what to add next (cheap labs that resolve ambiguity from tier 1), what to reach for only when cheaper layers can't disambiguate. Optimized for information-per-dollar, not absolute coverage.

**Deliverable:** `assessment/Sequence.md` — the canonical capture order.

### Step 6 — Mapping vs. Tracking Split

Two configurations of the toolkit:
- **Initial mapping pass:** broader, deeper, one-time-ish; emphasizes coverage and depth.
- **Ongoing tracking pass:** narrower, repeated, cadence-matched; emphasizes signal-to-noise on variables responding to intervention.

**Deliverable:** `assessment/Configurations.md` — the two-mode toolkit specification.

---

## Design Principles That Govern This Toolkit

These inherit from Layer 1's discipline and constrain every step above:

1. **Mechanistic specificity.** Every marker traces to a specific Layer 1 mechanism. No marker included because it's "metabolic-feeling"; each must have a named pathway it reflects.
2. **Direct over proxy.** ETCO₂ measures oxidative output directly; TSH measures pituitary response. Privilege direct; name when proxy is unavoidable.
3. **Disambiguation by combination.** Single markers are noise; signatures are signal. The toolkit's power is combinatorial logic, not any individual reading.
4. **Cost-utility, not cost alone.** A free question that captures something a $400 panel doesn't sometimes outranks the panel.
5. **Cadence-matched capture.** Capture frequency must match the variable's natural timescale or the data is noise.
6. **State-dependent interpretation.** The same marker can have opposite meanings in different attractor states. Interpretation rules must encode this.
7. **Honest reporter reliability.** Objective instruments, objective at-home measurements, self-reported observations, and clinician-interpreted findings have different reliability tiers; weight accordingly.
8. **Mapping vs. tracking are different jobs.** The toolkit must be configurable for both.
9. **Asymmetry principle inherits from Layer 1.** Once derived, the toolkit is correct until proven otherwise with verified evidence. Bar for change is high; corrigibility is preserved.

---

## Open Questions / Where This Could Be Wrong

- **Subsystem completeness.** Step 1's row vector may miss subsystems Layer 1 implicitly tracks. Cross-check against every mechanism doc before declaring complete.
- **Markers with empirical signal but partial mechanism trace.** Tongue coating, foamy urine, certain TCM-tradition markers correlate with specific states but their mechanism is partially understood. How to weight markers where empirical signal exists but the Layer 1 trace is incomplete?
- **Phenotype universality.** Toolkit assumes the same instrument works across people. Some markers may be more or less informative across age, sex, pregnancy, ethnicity-mediated genetic variation (e.g., DIO2 polymorphism). Flag where universality is assumed and where it must be qualified.
- **Wearable validity.** HRV, CGM, sleep-staging from consumer devices have varying validation rigor. Specify which signals are trustworthy and which are noise.

---

## What Lives Where (Once Built)

```
assessment/
├── Plan.md                  ← this document
├── Subsystems.md            ← Step 1 output
├── Markers.md               ← Step 2 output
├── Marker Properties.md     ← Step 3 output
├── Triangulation.md         ← Step 4 output
├── Sequence.md              ← Step 5 output
└── Configurations.md        ← Step 6 output
```

Future Layer 3 (`practice_personalization/`) and Layer 4 (`dynamics/`) directories will follow the same charter-first pattern.
