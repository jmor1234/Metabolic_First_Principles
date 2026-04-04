# Peat Claims Verification Vault

This is an Obsidian vault containing a systematic verification of Ray Peat's biochemistry claims against modern peer-reviewed research.

## Before Doing Anything

Read `peat_claims_verified/methodology.md` first. It defines the three-phase process, the document structure, the assessment scale, and the Obsidian conventions that every document follows. Do not create or modify topic documents without understanding the methodology.

## Core Principle

Health is efficient oxidative metabolism of glucose to CO2. Disease is its progressive failure. Every document in this vault examines one aspect of that single system. The documents are not independent — they form an interconnected network where every topic feeds into and receives from every other topic.

## Vault Architecture

- `peat_claims_verified/System Overview.md` — Entry point. The two metabolic attractors, feedback loops, recurring patterns, and assessment summary across all topics.
- `peat_claims_verified/Practical Convergence.md` — Shared interventions stated once. Topic docs link here instead of restating common recommendations.
- `peat_claims_verified/methodology.md` — The three-phase process, document structure template, Obsidian conventions, and canonical wikilink locations.
- `peat_claims_verified/AUDIT - Phase 2 Integrity Gap.md` — Documents an integrity issue discovered during production and the ongoing remediation. Read this if any topic document has `status/phase1` in its frontmatter.
- `peat_claims_verified/*.md` — Topic documents (PUFA, thyroid, estrogen, progesterone, serotonin, CO2, lactate, histamine). Check each document's frontmatter `status` tag — `status/complete` means fully verified, `status/phase1` means Phase 1 retained but Phases 2 and 3 are awaiting redo.

## Obsidian Conventions

This vault uses Obsidian-flavored markdown. Key rules:

- **Frontmatter** on every file with `title`, `aliases`, `tags`, `role`, `claims`, `assessment-summary`, `connections`, `peat-sources`.
- **Wikilinks over redundancy.** When a mechanism is explained canonically in one doc, others link to it. See the canonical locations table in `methodology.md#Obsidian Conventions`.
- **Callouts for assessments.** `[!success]` = confirmed, `[!tip]` = confirmed with nuance, `[!info]` = partial, `[!warning]` = overstated, `[!question]` = speculative, `[!failure]` = not supported. `[!quote]` for Peat quotes. `[!example]-` for recurring pattern appearances.
- **No cross-document redundancy.** If it's explained fully somewhere, link to it. Don't re-explain.
- **File naming.** Topic documents use lowercase (`pufa.md`, `co2.md`). Structural notes use title case (`System Overview.md`). Wikilinks use the actual filename casing.
- **Tag taxonomy.** Topics: `topic/[name]`, `status/complete` or `status/phase1` (see audit doc). Structural notes: `structural/moc`, `structural/practical`, `structural/methodology`, `structural/audit`. All files: `framework/peat`.

## Assessment Honesty

The methodology requires calibrated assessment, not advocacy. Some claims are confirmed. Some are refined. Some are overstated. Some lack evidence. Report all of these accurately. Forcing every claim into "confirmed" is as dishonest as dismissing every claim as "unproven."

## Navigating This Vault (Context-Efficient Agent Strategy)

Do not read full topic files. The Obsidian structure enables layered navigation — get maximum understanding for minimum context consumed.

### The Four Layers

**Layer 1 (~10KB — start here always):** Read `peat_claims_verified/System Overview.md`. Gets the full architecture (two attractors, 9 feedback loops, 6 recurring patterns, assessment summary table) for ~3% of total vault context.

**Layer 2 (~2KB total):** Scan frontmatter for any doc's metadata without reading body text.
```bash
obsidian properties file="thyroid" format=json
```
Returns title, claims list, connections, assessment-summary as structured JSON. Or use `Grep for assessment-summary` across all files for the vault-wide index in one call.

**Layer 3 (~0.5KB per doc):** Get a document's heading tree before reading content.
```bash
obsidian outline file="estrogen"
```
Returns the full heading structure. Navigate to the specific section needed.

**Layer 4 (targeted):** Read only the specific section you need. Follow wikilinks to specific headings. Use native Read with offset/limit.

**Example:** "How does estrogen relate to serotonin?" costs ~6KB through this vault (System Overview → wikilink to `serotonin.md#Claim 5` → read that section), not ~300KB (reading all files).

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
| PUFA-serotonin loop | `pufa.md#PUFA and Serotonin Promotion` |
| PUFA-estrogen loop | `pufa.md#PUFA-Estrogen Mutual Amplification` |
| CO2-serotonin axis | `serotonin.md#Claim 4` |
| Estrogen-MAO-serotonin | `serotonin.md#Claim 5` |
| Thyroid downstream cascade | `thyroid.md#Claim 1` |
| Pregnenolone steal | `progesterone.md#Why Progesterone Depletes` |

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
