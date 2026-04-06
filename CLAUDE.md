# Peat Claims Verification Vault

This is an Obsidian vault containing a systematic verification of Ray Peat's biochemistry claims against modern peer-reviewed research.

## Before Doing Anything

**If you need to understand the vault:** Start with the navigation strategy in [Navigating This Vault](#navigating-this-vault-context-efficient-agent-strategy) below. Do NOT read every file — the vault is designed for layered access.

**If you need to create or modify topic documents:** Read `peat_claims_verified/methodology.md` first. It defines the three-phase process, the document structure, the assessment scale, and the Obsidian conventions that every document follows.

## Core Principle

Health is efficient oxidative metabolism of glucose to CO2. Disease is its progressive failure. Every document in this vault examines one aspect of that single system. The documents are not independent — they form an interconnected network where every topic feeds into and receives from every other topic.

## Vault Architecture

- `peat_claims_verified/System Overview.md` — Entry point. The two metabolic attractors, feedback loops, recurring patterns, and assessment summary across all topics.
- `peat_claims_verified/Practical Convergence.md` — Shared interventions stated once. Topic docs link here instead of restating common recommendations.
- `peat_claims_verified/methodology.md` — The three-phase process, document structure template, Obsidian conventions, and canonical wikilink locations.
- `peat_claims_verified/*.md` — Topic documents (PUFA, thyroid, estrogen, progesterone, serotonin, CO2, lactate, histamine, endotoxin, liver, sugar, iron, vitamin-e, aspirin). All topics are `status/complete` — fully verified under the corrected three-phase methodology with sourced Phase 2 research context.

## Obsidian Conventions

This vault uses Obsidian-flavored markdown. Key rules:

- **Frontmatter** on every file with `title`, `aliases`, `tags`, `role`, `claims`, `assessment-summary`, `connections`, `peat-sources`.
- **Wikilinks over redundancy.** When a mechanism is explained canonically in one doc, others link to it. See the canonical locations table in `methodology.md#Obsidian Conventions`.
- **Callouts for assessments.** `[!success]` = confirmed, `[!tip]` = confirmed with nuance, `[!info]` = partial, `[!warning]` = overstated, `[!question]` = speculative, `[!failure]` = not supported. `[!quote]` for Peat quotes. `[!example]-` for recurring pattern appearances.
- **No cross-document redundancy.** If it's explained fully somewhere, link to it. Don't re-explain.
- **File naming.** Topic documents use lowercase (`pufa.md`, `co2.md`). Structural notes use title case (`System Overview.md`). Wikilinks use the actual filename casing.
- **Tag taxonomy.** Topics: `topic/[name]`, `status/complete`. Structural notes: `structural/moc`, `structural/practical`, `structural/methodology`. All files: `framework/peat`.

## Assessment Honesty

The methodology requires calibrated assessment, not advocacy. Some claims are confirmed. Some are refined. Some are overstated. Some lack evidence. Report all of these accurately. Forcing every claim into "confirmed" is as dishonest as dismissing every claim as "unproven."

## Navigating This Vault (Context-Efficient Agent Strategy)

Do not read full topic files unless you are producing new content. The vault is ~150KB total. The strategies below achieve 85-95% of that understanding for ~15-25KB. The vault was architectured so that structural files capture the system and topic files provide the evidence.

### Deep Understanding Path (~20KB → ~90% comprehension)

When you need to genuinely understand the framework — not just look up a fact, but hold the architecture in working memory — read these three resources in order:

1. **`System Overview.md` (~10KB)** — The two metabolic attractors, 9 interlocking feedback loops, 6 recurring patterns, and the assessment summary table showing what was confirmed/refined/contradicted per topic. This alone is ~75% of the conceptual understanding. **Always start here.**

2. **`Practical Convergence.md` (~3KB)** — The practical synthesis: what the verified claims mean for intervention (the 7 core interventions), and the monitoring framework (temperature + pulse + ETCO2 + lactate). Completes the "so what" that System Overview doesn't cover.

3. **`methodology.md` "Topics Completed" section (~3KB)** — Scroll to the `## Topics Completed` heading (around line 236). Each topic gets 2-3 sentences capturing the key findings, mechanism corrections, AND defining research distortions. This is more informative per token than any other summary in the vault. Do NOT read methodology.md from the top for understanding — the process documentation is only needed when producing new topics.

These three reads give ~90% understanding at ~16KB.

### Going Deeper on Specific Topics

Each topic document contains high-value summary sections that are far cheaper than a full read (~500-800 words per topic vs ~4000-6000 words full):

- **`> [!abstract] Overall Assessment`** — A calibrated ~200-word summary near the bottom of each topic file. Reading all 12 costs ~5KB total and gives the complete verified verdict per topic with specific findings named. Find them with:
  ```
  Grep for "[!abstract]" across peat_claims_verified/*.md
  ```

- **`## What Makes This Topic Different`** — A ~100-word section near the bottom of each topic file identifying its unique contribution to the vault. These explain why estrogen's dominant pattern is context-dependence, why lactate is where the framework is most honestly challenged, why histamine is the most testable integration claim, etc.

- **`## Research Context`** — The industry/incentive analysis near the top of each topic file. These are NOT summarized in any structural file. If you need to understand WHY the research landscape looks the way it does for a topic (the $100B PUFA industry, the $17B antidepressant market, the WHI chemical conflation with 230+ compound horse urine extract), you must read the topic's Research Context section directly. ~800-1200 words each.

### Finding Corrections and Contradictions

To find where Peat was wrong or overstated without reading full files:

```
Grep for "[!warning]" — overstated claims
Grep for "[!failure]" — not supported claims
Grep for "[!question]" — speculative claims
Grep for "NOT confirmed" or "NOT supported" or "CONTRADICTED" — explicit corrections in verification text
```

Key corrections an agent should know exist (details in the topic files):
- **Lactate:** Brain excitotoxicity claim contradicted — acute lactate is neuroprotective. Methylglyoxal direction reversed.
- **Progesterone:** Pregnenolone steal mechanism wrong — HPA axis suppression, not substrate competition. Clinical outcome correct.
- **Serotonin:** SSRI non-selectivity NOT supported. Brain serotonin aging NOT confirmed by imaging.
- **Estrogen:** Glycolytic shift real but mechanism is PI3K/AKT signaling, not direct Complex IV blockade.
- **Thyroid:** Barnes 30-40% prevalence unsupported by modern validation.
- **CO2:** Queen bee longevity supports membrane pacemaker theory, not CO2. Methylation claim speculative.
- **Endotoxin:** PUFA amplifies LPS tissue damage (confirmed) but saturated fat may facilitate LPS *entry* via chylomicrons. Fructose protective at physiological doses but excess fructose damages barrier and liver. Fermentable fiber claim partially supported — modern prebiotic data trends opposite on systemic markers. Carrot fiber lacks formal studies.
- **Liver:** Statin critique confirmed for mitochondrial effects (CoQ10 depletion, liver mitochondrial dysfunction) but statin all-cause mortality data more complex than blanket rejection — meta-analyses show mortality benefit. PUFA required for alcoholic liver injury (confirmed) but NAFLD feeding studies show saturated fat increases steatosis — endpoint distinction (fat accumulation vs inflammatory destruction) resolves the contradiction. Progesterone evidence for liver fibrosis reversal specifically is limited. UGT aging decline more genetically variable than Peat implied.
- **Sugar:** Glucolipotoxicity complicates "sugar protects beta cells" claim — glucose + FFA together MORE toxic than FFA alone. SSB dose-response (20-27% increased diabetes risk per serving) cannot be dismissed. Low-carb diets DO improve HbA1c short-term. GI not "useless" — low-GI diets show modest clinical benefits. Whole grains show 21-25% diabetes protection (complicating blanket anti-starch). Long-term keto adaptation may normalize the cortisol increase seen short-term. PUFA-insulin resistance evidence genuinely mixed.
- **Iron:** Iron hypothesis of CVD sex differences plausible but not proven over hormonal explanation — both likely contribute. Copper-iron age trajectory more complex than simple depletion (compensatory ceruloplasmin increases in neurodegeneration). Iron fortification × PUFA promotion interaction never tested epidemiologically. Blood donation cardiovascular evidence mixed. Ferritin as acute phase reactant confounds iron-mortality studies.
- **Aspirin:** ASPREE trial found aspirin INCREASED cancer mortality (HR 1.14) in healthy elderly without increasing incidence — most dramatic context-dependence in the vault. Neuroprotection mechanistically strong but failed clinically (AD Phase 3, ASPREE dementia). "Shifts toward glucose oxidation" claim contradicted at mitochondrial level — AMPK activation increases fatty acid oxidation. GI bleeding risk real (NNH ~500-816/year), not fabricated. Mead acid surrogate hypothesis untested. Fertility improvement evidence mixed.
- **Vitamin E:** Tocotrienol caution NOT supported — modern data shows GRAS status, safety to 3.2g/day, hepatoprotective in NAFLD. EFA deficiency "intensifying" mitochondrial energy production stronger than evidence warrants — confirmed finding is damage resistance, not enhancement. Anti-estrogenic identity is isoform-dependent: alpha-tocopherol opposes estrogen, but delta-tocopherol can activate estrogen-responsive genes. Desaturase activation by vitamin E deficiency claim unverified in current literature.

### Task-Specific Navigation (The Four Layers)

For answering specific questions or working on targeted sections:

**Layer 1 (~10KB):** Read `System Overview.md`. Always start here.

**Layer 2 (~2KB total):** Scan frontmatter for any doc's metadata without reading body text.
```bash
obsidian properties file="thyroid" format=json
```
Returns title, claims list, connections, assessment-summary as structured JSON. Or Grep for `assessment-summary` across all files for the vault-wide index in one call.

**Layer 3 (~0.5KB per doc):** Get a document's heading tree before reading content.
```bash
obsidian outline file="estrogen"
```
Returns the full heading structure. Navigate to the specific section needed.

**Layer 4 (targeted):** Read only the specific section you need. Follow wikilinks to specific headings. Use native Read with offset/limit.

**Example:** "How does estrogen relate to serotonin?" costs ~6KB (System Overview → wikilink to `serotonin.md#Claim 5` → read that section), not ~150KB (reading all files).

### Obsidian CLI Commands (Requires Obsidian Running)

Use these for graph navigation — they query Obsidian's index, not the files directly:

| Command | What it returns |
|---|---|
| `obsidian outline file="X"` | Heading tree without reading content |
| `obsidian backlinks file="X" counts` | Every file linking to X, with counts |
| `obsidian links file="X"` | Every file X links out to |
| `obsidian properties file="X" format=json` | Full frontmatter as structured JSON |
| `obsidian search query="term" limit=N` | Which files contain the term |
| `obsidian tag name="topic/X"` | Files with a specific tag |
| `obsidian tags sort=count counts` | Full tag taxonomy |
| `obsidian unresolved` | Vault-wide broken link check |

**Known bug (Windows/Git Bash):** Colon subcommands with key=value parameters fail with exit 127. Affects `property:read`, `search:context`, `property:set`. Workarounds:
- Use `properties file="X" format=json` instead of `property:read`
- Use `search` for file list + native Read for content instead of `search:context`

### When to Use CLI vs Native Tools

- **CLI** for graph navigation: outline, backlinks, links, search, tags, unresolved
- **Native Read** for actual content retrieval (with offset/limit for specific sections)
- **Native Grep** for pattern matching with line numbers (finding callout types, specific text patterns)

### Canonical Wikilink Locations

When you need a specific mechanism, go directly to its canonical treatment instead of searching:

| Mechanism | Canonical Location |
|---|---|
| System architecture | `System Overview.md` |
| Shared interventions | `Practical Convergence.md` |
| Topic summaries (2-3 lines each) | `methodology.md#Topics Completed` |
| PUFA-serotonin loop | `pufa.md#PUFA and Serotonin Promotion` |
| PUFA-estrogen loop | `pufa.md#PUFA-Estrogen Mutual Amplification` |
| PUFA immunosuppression | `pufa.md#PUFA and Immunosuppression` |
| CO2-serotonin axis | `serotonin.md#Claim 4` |
| Estrogen-MAO-serotonin | `serotonin.md#Claim 5` |
| SSRI critique + allopregnanolone | `serotonin.md#Claim 7` |
| Thyroid downstream cascade | `thyroid.md#Claim 1` |
| TSH diagnostic critique | `thyroid.md#Claim 2` |
| T3 vs T4 therapy / DIO2 | `thyroid.md#Claim 5` |
| Pregnenolone steal (corrected) | `progesterone.md#Why Progesterone Depletes` |
| Estrogen-histamine loop | `histamine.md#Claim 2` |
| pH-dependent mast cell storage | `histamine.md#Claim 3` |
| MCAS as metabolic failure | `histamine.md#Claim 8` |
| Lactate shuttle (honest integration) | `lactate.md#The Lactate Shuttle Question` |
| Warburg effect (bidirectional) | `lactate.md#Claim 3` |
| Carbamino protection hypothesis | `co2.md#Claim 3` |
| Estrogen tissue accumulation | `estrogen.md#Claim 3` |
| Endotoxin barrier vicious circle | `endotoxin.md#Claim 2` |
| Endotoxin-estrogen-liver circuit | `endotoxin.md#Claim 3` |
| Gut-thyroid-motility circuit | `endotoxin.md#Claim 4` |
| PUFA-endotoxin synergy | `endotoxin.md#Claim 5` |
| Endotoxin practical reduction | `endotoxin.md#Claim 8` |
| Liver energy-dependent hub | `liver.md#Claim 1` |
| Glycogen-glucuronidation connection | `liver.md#Claim 2` |
| Glucuronidation master pathway | `liver.md#Claim 3` |
| Cholesterol as substrate (statin critique) | `liver.md#Claim 4` |
| Liver portal gatekeeper | `liver.md#Claim 5` |
| PUFA-liver toxicity | `liver.md#Claim 6` |
| Albumin as protective output | `liver.md#Claim 7` |
| Liver regeneration / fibrosis reversal | `liver.md#Claim 8` |
| Glucose as preferred substrate | `sugar.md#Claim 1` |
| Randle cycle mechanism | `sugar.md#Claim 2` |
| Diabetes as metabolic failure | `sugar.md#Claim 3` |
| Fructose dual nature (canonical) | `sugar.md#Claim 4` |
| Sugar-stress hormone cascade | `sugar.md#Claim 5` |
| Starch vs sugar distinction | `sugar.md#Claim 6` |
| Glycemic index critique | `sugar.md#Claim 7` |
| Iron-PUFA Fenton catalyst | `iron.md#Claim 1` |
| Iron accumulation with aging | `iron.md#Claim 2` |
| Menstruation as iron regulation | `iron.md#Claim 3` |
| Iron fortification concerns | `iron.md#Claim 4` |
| Iron and infection/immunity | `iron.md#Claim 5` |
| Iron liver/brain damage | `iron.md#Claim 6` |
| Copper-iron antagonism | `iron.md#Claim 7` |
| Iron practical reduction | `iron.md#Claim 8` |
| Antioxidant misdefinition and suppression | `vitamin-e.md#Claim 1` |
| Vitamin E as estrogen antagonist | `vitamin-e.md#Claim 2` |
| PUFA-iron-vitamin E triad | `vitamin-e.md#Claim 3` |
| Vitamin E mitochondrial energy protection | `vitamin-e.md#Claim 4` |
| Vitamin E anti-inflammatory/anti-fibrotic | `vitamin-e.md#Claim 5` |
| Vitamin E and lipofuscin/aging | `vitamin-e.md#Claim 6` |
| Forms of vitamin E | `vitamin-e.md#Claim 7` |
| Aspirin beyond COX — metabolic regulator | `aspirin.md#Claim 1` |
| Aspirin as estrogen antagonist | `aspirin.md#Claim 2` |
| Aspirin and cancer | `aspirin.md#Claim 3` |
| Aspirin neuroprotection | `aspirin.md#Claim 4` |
| Aspirin inverted safety narrative | `aspirin.md#Claim 5` |
| Regulatory triad (aspirin + vitamin E + progesterone) | `aspirin.md#Claim 6` |

Full canonical locations table: `methodology.md#Obsidian Conventions`.

## Adding New Topics

The methodology documents the full process. The short version:

1. Phase 1: Extract Peat's actual position from raypeat.com primary sources. Reconstruct reasoning chains, not just conclusions. Stop and get review before proceeding.
2. Phase 2: Identify the research context (funding, comparisons, timescales, endpoints, disciplinary fragmentation) **from real-time research, not training data**. Every factual claim about the research landscape must have a fetched source. See the critical rule in `methodology.md#Phase 2`.
3. Phase 3: Verify against research with full context. Use the assessment scale honestly. Connect to existing topics via wikilinks.

Follow the document structure template and Obsidian conventions in `methodology.md`. Link new topics into the existing network — update `System Overview.md` and `Practical Convergence.md` as needed.

**Finding existing references to a new topic:** Before writing, search for how existing docs already mention the topic:
```bash
obsidian search query="cholesterol" limit=10
```
Or use `Grep` across the vault. This reveals which existing docs need wikilinks to the new topic and which mechanisms are already partially documented elsewhere.
