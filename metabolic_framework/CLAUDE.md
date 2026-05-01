# Metabolic Framework

A first-principles understanding of what health and disease are at the metabolic level, verified against peer-reviewed research, stress-tested for accuracy, organized around biology itself. 14 documents organized in four tiers. This is the unified vault — all stress test refinements are incorporated.

## Read This Vault as an Integration, Not a Database

This vault is a connected system. The meaning of any single statement depends on its connections to other documents through the wikilink network. Surface terms have deep implications: "metabolic rate" is not raw throughput but the rate that emerges from intact hardware; "estrogen amplifies disease" means it amplifies whatever trajectory is in motion, not that it is categorically harmful; "the disease attractor is self-reinforcing" means feedback loops deepen the state when engaged but require specific conditions to engage.

Reading individual statements at face value — without tracing how they connect through the wikilink network — produces shallow conclusions and false contradictions that the vault does not actually contain. Before evaluating evidence against the vault, proposing changes, or answering complex questions about it, trace the reasoning chain through the connections. If you cannot trace it, you do not understand the vault well enough to draw conclusions yet.

The discipline for doing this rigorously is documented in `Verification Methodology.md`. Read it before any work that might modify the vault. The default position: the vault is correct until proven otherwise with verified evidence that survives a deep reading of its logic.

## Before Doing Anything

**If you need to understand the vault:** Follow the Deep Understanding Path below. Do NOT read every file — the vault is designed for layered access. Foundation + System together give the bulk of the conceptual understanding.

**If you need to modify, expand, or evaluate evidence against the vault:** Read `Verification Methodology.md` first. It defines the default position, the three hypotheses for evaluating apparent contradictions, the bar for changing the vault, and the verification sequence. Then read `Methodology.md` for evidence standards, confidence calibration, the document template, and the expansion process.

## Core Principle

Health is efficient oxidative metabolism of Krebs-cycle substrates — primarily glucose, with ketone bodies as a biochemically equivalent alternative — to CO2. Disease is its progressive failure. Every document examines one aspect of that single system. The documents are not independent — they form an interconnected network where every mechanism feeds into and receives from every other.

## Vault Architecture (4 Tiers)

| Tier | Documents | Purpose |
|---|---|---|
| **1. Structural** | `Foundation.md`, `The System.md` | WHAT health/disease are, HOW the system works |
| **2. Mechanisms** | 9 mechanism docs (see below) | The detailed biology of each component |
| **3. Application** | `Practice.md` | What to do: interventions, monitoring, sequence |
| **4. Meta** | `Methodology.md`, `Verification Methodology.md` | How the vault works: standards, navigation, expansion, and how evidence is evaluated and changes are governed |

### Mechanism Documents (Tier 2)

| Document | Components | Role |
|---|---|---|
| `The Master Throttle.md` | Thyroid, T3 | Rate-setter for oxidative metabolism |
| `The Preferred Substrate.md` | Glucose, Ketone Bodies, Randle cycle | Preferred fuels, their biochemistry, and what blocks glucose oxidation |
| `The Metabolic Fork.md` | CO2, Lactate | Two active outputs of the pyruvate decision point |
| `Membrane Damage and Defense.md` | PUFA, Iron, Vitamin E, Ferroptosis | The peroxidation chain: substrate, catalyst, defense |
| `The Hormonal Axis.md` | Estrogen, Progesterone | Single metabolic axis: glycolysis vs oxidation |
| `Conservation Signaling.md` | Serotonin, Histamine, Mast Cells | Parallel conservation/stress mediators |
| `The Gut-Liver Axis.md` | Endotoxin, Liver, LPS, NASH | Gateway stressor + the hub where everything converges |
| `The Cellular Readout.md` | Calcium, PTH, Phosphate | Energy-dependent ion distribution as metabolic readout |
| `The Temporal Dimension.md` | Circadian, Light, Melatonin, PBM | 24-hour oscillation between attractors |

## Navigating This Vault (Context-Efficient Agent Strategy)

### Deep Understanding Path

1. **`Foundation.md`** — The thesis, the first-principles argument, the evidence, the challenges, why the integration doesn't exist in mainstream medicine. **Always start here.**

2. **`The System.md`** — The two attractors (conditional on parameters), 15 components by role, the feedback architecture (10 clean loops + hub + 2 half-closed + forcing function), emergent properties (why disease is progressive, why single interventions fail, context-dependence, threshold dynamics), state-dependent damping, testable predictions, and the temporal oscillation.

These two documents alone provide the complete conceptual architecture.

### Essence-Only Reading Pattern (~3,500 tokens, full framework skeleton)

Every canonical doc (structural, mechanism, application, and meta) opens with an `[!abstract] Essence` callout — a 4-5 sentence prose distillation including load-bearing refinements (mechanism corrections, acute/chronic distinctions, tissue-specific qualifiers) that prevent surface-reading false conclusions.

For framework-level orientation without deep reading, read just the essence callouts across all canonical docs. This gives the full skeleton at ~2% of the vault's token weight. Drill into doc bodies when specifics are needed — the essence is orientation, not replacement.

```
Grep for "^> \[!abstract\] Essence" across metabolic_framework/*.md to locate all 14 essences (Foundation + The System + 9 mechanism docs + Practice + Methodology + Verification Methodology). Essence.md at `essence/Essence.md` and CLAUDE.md itself do not carry the callout.
```

The essences are derived from the canonical doc bodies; if conflict, the body wins. See `Methodology.md#On the Essence Callouts` for the subordination clause and audit discipline.

**Principles-level complement — `essence/Essence.md`** (at `..\essence\Essence.md`, one directory up from this vault). The per-doc essences in this vault distill *mechanisms*; `Essence.md` distills the framework's 13 first principles across 6 layers (what life is → what health and disease ARE → how the system behaves architecturally → temporal dynamics → scope → interpretive discipline). The two layers answer different questions and complement rather than duplicate each other. Read `Essence.md` (~2,500 tokens) to hold the first-principles skeleton; read the 14 per-doc essences (~4,500 tokens) to hold the mechanism skeleton. Together (~7k tokens, ~5% of the vault's weight) they give orientation at both the conceptual and mechanistic layers.

### Going Deeper

Each mechanism doc has high-value sections cheaper than a full read:

- **Opening paragraphs** (no heading, first 2-3 paragraphs) — The mechanism's role in the system.
- **`## System Connections`** — Table of connections to every other mechanism doc.
- **`## Where the Evidence Is Complex`** — Honest calibration: what's textbook vs uncertain. Marked with `[!warning]` callouts.
- **`## Research Context`** — Funding distortions, chemical conflation, why the picture is fragmented.

To get the key insight from each mechanism doc without reading in full:
```
Read the opening paragraphs + System Connections table
```

### Targeted Lookup

For a specific section or mechanism, go directly to its canonical location below. **If you just need the 4-5 sentence distillation of a whole doc** (not a specific sub-section), read the `[!abstract] Essence` callout at the top of the doc — see the Essence-Only Reading Pattern subsection above. Use this table for the deeper section-level drill-downs the essence doesn't cover.

| Mechanism | Canonical Location |
|---|---|
| **System architecture** | `The System.md` |
| **Two attractors** | `The System.md#The Two Attractors` |
| **Feedback architecture** | `The System.md#The Feedback Loops` |
| **State-dependent damping** | `The System.md#State-dependent negative feedback` |
| **Testable predictions** | `The System.md#Testable predictions` |
| **Emergent properties** | `The System.md#Emergent Properties` |
| **Temporal oscillation** | `The System.md#The Temporal Architecture` |
| **Interventions** | `Practice.md#The Core Interventions` |
| **Aspirin deep-dive** | `Practice.md#Aspirin: The Upstream Regulator` |
| **Monitoring framework** | `Practice.md#Monitoring: How to Know If It's Working` |
| **Implementation sequence** | `Practice.md#Sequence: What to Address First` |
| **Dual genome regulation (T3)** | `The Master Throttle.md#Dual Genome Regulation` |
| **Downstream cascade (T3)** | `The Master Throttle.md#The Downstream Cascade` |
| **TSH diagnostic problem** | `The Master Throttle.md#The Diagnostic Problem` |
| **DIO2 polymorphism** | `The Master Throttle.md#The Conversion Problem` |
| **Ketone bodies biochemistry** | `The Preferred Substrate.md#Ketone Bodies: The Third Fuel Category` |
| **Randle cycle mechanism** | `The Preferred Substrate.md#The Randle Cycle: The Fork Blockade` |
| **PDH cofactors (B1, Mg, NAD+)** | `The Preferred Substrate.md#The PDH Checkpoint` |
| **Fructose dual nature** | `The Preferred Substrate.md#Fructose: The Randle Bypass` |
| **Sugar consumption paradox** | `The Preferred Substrate.md#The Sugar Consumption Paradox` |
| **CO2 as active protector** | `The Metabolic Fork.md#CO2 as Active Protector` |
| **Lactate as disease driver** | `The Metabolic Fork.md#Lactate as Active Disease Driver` |
| **Lactate shuttle (honest)** | `The Metabolic Fork.md#The Honest Integration` |
| **ETCO2 + lactate measurement** | `The Metabolic Fork.md#Measurement` |
| **Peroxidation chain** | `Membrane Damage and Defense.md#The Peroxidation Chain` |
| **PUFA in membranes** | `Membrane Damage and Defense.md#PUFA` |
| **Iron / Fenton / ferroptosis** | `Membrane Damage and Defense.md#Iron` |
| **Vitamin E regulatory identity** | `Membrane Damage and Defense.md#Vitamin E` |
| **Estrogen glycolytic shift** | `The Hormonal Axis.md#Estrogen` |
| **Progesterone opposition** | `The Hormonal Axis.md#Progesterone` |
| **What tips the E/P balance** | `The Hormonal Axis.md#What Tips the Balance` |
| **Pregnenolone steal (corrected)** | `The Hormonal Axis.md#What Tips the Balance` |
| **Serotonin conservation role** | `Conservation Signaling.md#Serotonin` |
| **Serotonin hypothesis collapse** | `Conservation Signaling.md#Serotonin` |
| **SSRI / allopregnanolone** | `Conservation Signaling.md#Serotonin` |
| **Histamine / mast cells** | `Conservation Signaling.md#Histamine` |
| **MCAS as metabolic failure** | `Conservation Signaling.md#MCAS as Metabolic Failure` |
| **Shared triggers (ATP/V-ATPase, estrogen)** | `Conservation Signaling.md#Shared Triggers` |
| **Gut barrier energy-dependence** | `The Gut-Liver Axis.md#The Gut Barrier` |
| **Endotoxin gateway stressor** | `The Gut-Liver Axis.md#Endotoxin as the Gateway Stressor` |
| **Liver as metabolic hub** | `The Gut-Liver Axis.md#The Liver as Metabolic Hub` |
| **Three interface loops** | `The Gut-Liver Axis.md#The Three Interface Loops` |
| **Glucuronidation + glycogen** | `The Gut-Liver Axis.md#The Liver as Metabolic Hub` |
| **Resmetirom + Wegovy dual validation** | `The Gut-Liver Axis.md#Fibrosis and Recovery` |
| **Calcium energy-dependent exclusion** | `The Cellular Readout.md#Energy-Dependent Calcium Exclusion` |
| **The calcium paradox** | `The Cellular Readout.md#The Calcium Paradox` |
| **PTH as disease mediator** | `The Cellular Readout.md#PTH as Systemic Disease Mediator` |
| **Phosphate-aging (Klotho)** | `The Cellular Readout.md#Phosphate as Aging Accelerator` |
| **Nocturnal conservation program** | `The Temporal Dimension.md#The Nightly Conservation Program` |
| **Morning reversal (two pathways)** | `The Temporal Dimension.md#The Morning Reversal` |
| **Photobiomodulation (670nm)** | `The Temporal Dimension.md#Photobiomodulation` |
| **PUFA-light photosensitization** | `The Temporal Dimension.md#PUFA-Light Photosensitization` |
| **Melatonin corrections** | `The Temporal Dimension.md#Where the Evidence Is Complex` |
| **Evidence standards** | `Methodology.md#Evidence Standards` |
| **Confidence calibration** | `Methodology.md#Confidence Calibration` |
| **Document template** | `Methodology.md#The Document Template` |
| **Expansion process** | `Methodology.md#How to Expand the Vault` |
| **Default position (vault correct until proven)** | `Verification Methodology.md#The Default Position` |
| **Three hypotheses for contradictions** | `Verification Methodology.md#The Three Hypotheses In Order` |
| **Bar for changing the vault** | `Verification Methodology.md#The Bar for Changing the Vault` |
| **Verification sequence (6 steps)** | `Verification Methodology.md#The Verification Sequence` |
| **Three rules (acute/chronic, context, pass/fail)** | `Verification Methodology.md#The Three Rules` |
| **Research standards** | `Verification Methodology.md#Research Standards` |

### Honest Calibration and Challenges

All honest calibration uses `[!warning]` callouts throughout the vault:
```
Grep for "[!warning]" across metabolic_framework/*.md
```

Key things an agent should know about what this vault contains:

**Stress test refinements (now integrated into the text):**
- **CO2 is a parallel marker, not a causal driver** in any feedback loop. ATP/V-ATPase is the actual mechanism for mediator sequestration. CO2's non-loop roles (Bohr effect, carbamino bonds, calcium/pH buffering) are real and preserved. See The System.md (Loop 7), The Metabolic Fork.md, Conservation Signaling.md.
- **Bistability is conditional** on parameter values (PUFA burden, iron load, chronic stress, endotoxin). Some organisms are monostable. See The System.md, Foundation.md.
- **State-dependent damping** — every negative feedback mechanism depends on mitochondrial respiratory capacity for the machinery that performs it (synthesis, folding, trafficking, cofactor regeneration), even when the regulatory act itself is thermodynamically free. This unifies feedback failure across otherwise independent systems (HPT, HPA, antioxidants, biogenesis, autophagy, hepatic regeneration, lactate clearance) through multiple coupled downstream currencies: ATP (for protein synthesis and autophagy mechanics), NADPH (for antioxidant cofactor regeneration, produced ATP-independently via the pentose phosphate pathway), membrane potential Δψ_m (for substrate import), and NAD+ (for sirtuin-mediated regulation — tissue-specific and not reliably human-translatable via NR/NMN supplementation, per Chubanava 2025 and Dollerup 2020). All share the mitochondrial OXPHOS origin and fall together when M fails. One of several mechanisms generating bistability here — alongside ultrasensitivity, mutual inhibition, and saturation of positive feedback — and distinctive for the cross-system unification. See The System.md.
- **Ketone bodies** are a biochemically distinct third fuel category (CO2/ATP matching glucose, not equivalent to raw fatty acid β-oxidation). Randle pathology ≠ adapted ketosis. See The Preferred Substrate.md.
- **Loop architecture** is 10 clean closed loops + 1 multi-armed hub + 2 half-closed + 1 periodic forcing function (not 13 loops). See The System.md.
- **Six testable predictions** from the formal bistability analysis, two already observed. See The System.md.

**Mechanism corrections (integrated into the text with `[!warning]` callouts):**
- Estrogen glycolytic shift via PI3K/AKT, not direct Complex IV blockade (The Hormonal Axis)
- Pregnenolone steal wrong — HPA axis suppression, not substrate competition (The Hormonal Axis)
- Acute lactate is neuroprotective; chronic lactate drives epigenetic reprogramming (The Metabolic Fork)
- ASPREE showed aspirin increasing cancer mortality in elderly (Practice)
- ETCO2 is distinct from V'CO2 — reflects production AND ventilation (The Metabolic Fork, Foundation)
- Melatonin has genuine anti-estrogenic and thymus-rejuvenating effects (The Temporal Dimension)
- M1/M2 macrophage glycolytic burst is controlled deployment, not pathology (Foundation)

**Critical instruction for agents:** Before proposing any change to the vault, read `Verification Methodology.md`. The vault is an integration — apparent contradictions frequently dissolve when the vault is deeply understood rather than read at face value. The default position is that the vault is correct until proven otherwise with verified, replicated evidence that directly measures the variables the vault's claims operate on. See the Three Hypotheses and the Bar for Changing the Vault.

## Obsidian Conventions

### Wikilink Aliases
Grouped mechanism docs have aliases. These all resolve correctly:
- `[[PUFA]]`, `[[Iron]]`, `[[Vitamin E]]`, `[[Ferroptosis]]` → `Membrane Damage and Defense.md`
- `[[Estrogen]]`, `[[Progesterone]]` → `The Hormonal Axis.md`
- `[[Serotonin]]`, `[[Histamine]]`, `[[MCAS]]` → `Conservation Signaling.md`
- `[[CO2]]`, `[[Lactate]]` → `The Metabolic Fork.md`
- `[[Endotoxin]]`, `[[Liver]]`, `[[LPS]]`, `[[NASH]]` → `The Gut-Liver Axis.md`
- `[[Calcium]]`, `[[PTH]]` → `The Cellular Readout.md`
- `[[Thyroid]]`, `[[T3]]` → `The Master Throttle.md`
- `[[Glucose]]`, `[[Sugar]]` → `The Preferred Substrate.md`
- `[[Circadian]]`, `[[Light]]`, `[[Melatonin]]`, `[[PBM]]` → `The Temporal Dimension.md`

### Callout Types (only these four)
- `[!abstract]` — Section summaries, key takeaways. **When placed at the top of a file (above the opening paragraphs) and titled "Essence," this callout carries the specific distillation role defined in `Methodology.md#On the Essence Callouts` — 4-5 sentence prose, derived from the body, body wins if conflict.**
- `[!example]` — Concrete evidence with citation
- `[!warning]` — Honest calibration: challenges, limitations, uncertainty
- `[!tip]` — Practical implications, navigation

### Tag Taxonomy
- `structural/entry`, `structural/system`, `structural/practice`, `structural/meta`
- `mechanism/[name]` for mechanism docs
- `framework/metabolic` on all files

### Frontmatter Fields
`title`, `aliases`, `tags`, `role`, `confidence`, `last-verified`, `scope`, `connections`

## When to Use CLI vs Native Tools

- **Native Read** with offset/limit for targeted section access
- **Native Grep** for pattern matching (finding callout types, specific text patterns, citations)
- **Native Glob** for file listing
- **Obsidian CLI** (if running) for graph navigation: `obsidian outline`, `obsidian backlinks`, `obsidian links`, `obsidian search`

## Relationship to Peat Verification Vault

This vault was produced from a verification project archived at `project_history/peat_claims_verified/`. That vault verified claims against research. This vault extracts the verified findings as standalone knowledge, with stress test refinements incorporated. The two are independent — this vault contains no references to the verification project, no claim numbers, and no person-specific framing.
