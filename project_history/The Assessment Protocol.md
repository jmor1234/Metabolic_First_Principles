# The Assessment Protocol

**What this document is:** The bridge from "what is true about biology" (`The Integrated Framework.md`) to "what does THIS specific person do" (`metabolic_foundations/Practice.md`). It maps a person's observable data onto the framework's 6 state variables, estimates which metabolic regime they occupy, and outputs a targeted intervention priority.

**What this document is not:** A medical diagnosis. A replacement for clinical evaluation. A numerical scoring system. The data does not support that precision, and the protocol does not pretend otherwise.

**Traceability:** This protocol is built on the verified framework — the stress-tested architecture documented across `metabolic_foundations/` and `metabolic_refinements/`. Where specific findings inform the design, the source document is cited. The key findings that shape this protocol:

- Conditional bistability: the system can exhibit two stable states, but only when parameter conditions create a disease basin (`metabolic_refinements/Conditional Bistability and Attractor Dynamics.md`)
- State-dependent damping: every self-correcting mechanism requires ATP, so restoring mitochondrial function re-enables ALL damping systems (`metabolic_refinements/Stress Test Summary.md`)
- Slow/fast variable separation: M and P operate on weeks-months timescales and determine the landscape the fast variables operate on
- CO2 is a readout to monitor, not a mechanism to target (`metabolic_refinements/Loop 7 — Metabolism-Mediator Coupling.md`)

---

## The Assessment Principle

The same intervention produces different results depending on where the person is in the system. A monostable person (healthy attractor only — perturbations return to health) may need only 2-3 targeted interventions. A bistable person (trapped in a disease basin where feedback loops maintain the disease state) needs multiple simultaneous interventions to cross the threshold back to health. An assessment that does not determine which regime the person occupies cannot tell them what to do.

### The fundamental constraint

The framework's 6 state variables are:

| Variable | What it is | Timescale | Measurability |
|---|---|---|---|
| **M** (mitochondrial function) | Oxidative capacity — the fundamental state | Days-weeks | No direct clinical test. Inferred from functional markers. |
| **T** (active T3) | Master throttle — sets the rate of everything | Hours | Partially measurable (free T3), partially functional |
| **E** (free estrogen) | Glycolytic shift driver | Hours-days | Blood levels unreliable for tissue (5-50x accumulation) |
| **P** (PUFA tissue content) | Hardware damage substrate | Weeks-months | No clinical test. Estimated from dietary history only. |
| **L** (endotoxin load) | Gateway stressor | Hours | Not routinely measured. Inferred from symptoms. |
| **Lambda** (chronic lactate) | Epigenetic reprogramming driver | Hours-days | Blood lactate measurable; tissue lactylation is not. |

The two most important variables — M (determines whether damping systems work) and P (determines whether a disease basin exists) — are the least measurable. This is not fixable. The protocol works within it honestly.

### Three principles

**1. Iterative, not linear.** The assessment is not a single pass that produces a final answer. It produces a working estimate, predicts a response pattern, and refines the estimate based on what actually happens. Three passes: history and slow-variable estimation, then measurement and mismatch analysis, then dynamic assessment. Each pass constrains the next.

**2. Honestly retrospective on regime.** You cannot determine from a snapshot whether someone is monostable or bistable. Regime is revealed by how the system responds to intervention. The protocol produces a working regime estimate and checks it against reality over weeks. When the estimate is wrong, the response pattern tells you.

**3. Default conservative.** When uncertain about regime, assume bistable. Over-treating (addressing multiple variables when only one is needed) is harmless — it means doing more beneficial things. Under-treating (addressing one variable when multiple are needed) wastes months before reassessment catches it.

### The timescale-separation diagnostic

The slow variables (P, M) set the landscape. The fast variables (T, E, L, Lambda) snap to equilibria determined by that landscape. This separation is a diagnostic tool: if you estimate the slow variables from history, you can *predict* what the fast-variable equilibrium should look like. Then measure the fast variables and compare.

- **Match:** The slow-variable estimate is probably right. The person's current state reflects their chronic trajectory.
- **Fast variables worse than predicted:** Something acute is layered on top — a recent stressor, infection, medication, or life event. The chronic landscape may be better than current markers suggest. This is good news for prognosis.
- **Fast variables better than predicted:** Compensatory effort is masking a deeper problem. The person feels adequate while the slow variables degrade underneath. This is the most dangerous case. The meal test and morning recovery assessment are designed to unmask it.

---

## Pass 1: History and Slow-Variable Estimation

History is not background. It is the primary evidence for the variables that cannot be directly measured.

### Dietary history (estimates P)

**Years of PUFA exposure:**
- How many years/decades eating seed oils (soybean, corn, canola, sunflower, safflower, cottonseed)?
- How much processed food, restaurant food, fried food?
- What cooking fats were used at home growing up?

**Current dietary fat profile:**
- Primary cooking fats now?
- How much processed food currently?
- Awareness of seed oil content in foods?

**Time since dietary change:**
- If the person has changed their fat intake, how long ago?
- Tissue PUFA turnover: adipose tissue takes 2-4+ years to substantially turn over. Red blood cell membranes turn over in ~120 days. Mitochondrial cardiolipin composition changes over months.
- A person who ate high-PUFA for 30 years and switched 6 months ago still has very high tissue P.

**Body composition:**
- More adipose tissue = more stored PUFA = larger reservoir to turn over.

**P estimation:**

| Category | Profile | Implication |
|---|---|---|
| **High P** | Decades of standard diet, limited time since change (<1-2 years), or no change | Disease basin may exist. Loop 1 (PUFA-peroxidation) is fueled. Hardware damage ongoing. |
| **Moderate P** | Changed diet 2-4 years ago, or moderate historical exposure | Tissue burden declining but not cleared. Transitional period. |
| **Low P** | Never had high PUFA exposure, OR changed 4+ years ago with low adiposity | Disease basin from P is unlikely. Loop 1 has limited substrate. |

Confidence: medium at best. This is an estimate from intake, not a tissue measurement. State this honestly.

### Medical and symptom history (estimates M trajectory)

**Duration and trajectory:**
- How long have symptoms been present? Months → possible monostable perturbation. Years-decades → likely bistable.
- Is the trajectory worsening, stable, or improving? Progressive worsening despite removing known causes is the hysteresis signature — the strongest single signal for bistability.

**Recovery patterns:**
- Does the person bounce back from illness, stress, or sleep disruption? Quick recovery → damping systems intact → likely closer to monostable. Prolonged recovery or permanent post-event decline → damping systems weakened → likely closer to bistable.
- Has there been a discrete event (surgery, pregnancy, prolonged stress period, menopause, infection) after which health never fully recovered? This is a common pattern for crossing the bistability threshold.

**Previous interventions and responses:**
- Has the person tried single interventions (thyroid medication, dietary changes, supplements, stress reduction)? Did they help? For how long? Did improvement plateau?
- "I've tried everything and nothing works" or "things help for a while then stop" are strong bistability signals — the system compensates around single-loop interventions.

**Medical history:**
- Thyroid diagnosis (hypothyroid, Hashimoto's, subclinical hypothyroid)?
- Hormonal history (menstrual patterns, hormonal contraceptives, HRT, pregnancies)?
- Chronic conditions (PCOS, endometriosis, NASH, IBS/SIBO, autoimmune, metabolic syndrome)?
- Medications (statins affect CoQ10 and vitamin E recycling; PPIs affect mineral absorption; SSRIs affect serotonin dynamics)?

### Predicted fast-variable equilibrium

Based on the P and M estimates, predict what the fast variables SHOULD look like if the person is at their chronic equilibrium (not acutely perturbed):

| Slow-variable estimate | Predicted fast-variable equilibrium |
|---|---|
| High P, long duration, degraded M | Low T, elevated E (especially with adiposity), elevated L (gut-thyroid coupling), elevated Lambda |
| Low P, short duration, adequate M | Fast variables near normal — any abnormality is likely a correctable perturbation |
| Mixed (e.g., high P but recent change, moderate M) | Intermediate — fast variables improving but not yet normalized |

Write this prediction down before measuring. The mismatch between prediction and measurement is itself diagnostic.

---

## Pass 2: Measurement and Mismatch

### Self-assessment tier

This tier estimates M, T, and P (roughly). It cannot meaningfully estimate L or Lambda without clinical data. Three of six variables is enough to start — it is an M-first triage tool, not a full 6-variable assessment. Be honest about this.

**Temperature** (M and T indicator):

Oral temperature, first thing on waking, before getting up. Use a reliable thermometer. Record daily for at least 5 consecutive days to establish pattern.

| Waking temperature | Interpretation |
|---|---|
| < 97.4 F | Impaired — consistently below population baseline. Suggests low M, low T, or both. |
| 97.4 - 97.8 F | Borderline — metabolic rate may be adequate or may be supported by compensation. Meal test clarifies. |
| > 97.8 F | Adequate range. Approaching 98.6 F is optimal. |

Confounders: electric blankets, ambient temperature, menstrual cycle phase (progesterone raises temperature in luteal phase), adrenaline compensation (a warm waking temperature can be cortisol-driven). Temperature alone is insufficient — interpret with pulse and meal test.

**Pulse** (M and T indicator):

Seated, resting, after 5 minutes of sitting quietly. Not immediately after waking (autonomic transition), not after caffeine, not after exertion. Record alongside temperature.

| Resting pulse | Interpretation |
|---|---|
| < 65 bpm | Likely suppressed — insufficient thyroid drive. Exception: trained endurance athletes (which itself may reflect adaptation to conservation-mode metabolism). |
| 65-75 bpm | Borderline — may be adequate or mildly suppressed. Context from temperature and meal test. |
| 75-85 bpm | Adequate — metabolic rate is generating this cardiac output. |
| > 95 bpm | Likely compensatory — adrenaline driving heart rate because thyroid is not driving metabolic rate. Especially suspect if accompanied by anxiety, tremor, or cold extremities. |

**The combination tells more than either alone:**

| Temperature | Pulse | Most likely interpretation |
|---|---|---|
| Warm (>97.8) | Moderate (75-85) | Genuine metabolic adequacy — M and T likely adequate |
| Warm (>97.8) | Fast (>95) | Stress compensation — adrenaline generating both warmth and heart rate. T likely low, cortisol high. Meal test will likely unmask. |
| Cold (<97.4) | Slow (<65) | Decompensated hypothyroidism — neither thyroid nor stress hormones maintaining metabolic rate. Low M, low T. |
| Cold (<97.4) | Fast (>95) | Mixed compensation — heart rate driven by adrenaline but not enough to maintain temperature. Significant T deficit with partial stress compensation. |

**Symptom inventory** (estimates T, E, L):

Thyroid-suggestive (low T): constipation, hair loss or thinning, dry skin, cold intolerance, morning difficulty, brain fog, unexplained elevated cholesterol, slow Achilles reflex relaxation, outer eyebrow thinning.

Estrogen-dominance-suggestive (high E): water retention/bloating, breast tenderness, heavy or irregular periods, mood swings, fibroids or endometriosis history, difficulty losing weight (especially hips/thighs). In men: gynecomastia, abdominal fat distribution, emotional lability. Post-menopausal: symptoms may intensify even as serum estrogen falls — tissue estrogen accumulates via local aromatase independent of ovarian production.

Endotoxin-suggestive (high L): bloating, gas, irregular transit, food intolerances, alcohol sensitivity, history of SIBO, IBS, or antibiotic-responsive gut symptoms. Coupling note: if T appears low, expect L is elevated — Loop 12 (gut-thyroid-motility) links them.

**Dietary and lifestyle context:**
- Current carbohydrate intake relative to energy needs (chronic under-eating drives cortisol)
- Current fat sources (still consuming seed oils? how much?)
- Light exposure (morning sunlight? indoor work? screen exposure after dark?)
- Sleep quality and duration
- Stress load (physiological and psychological)
- Exercise pattern (none vs moderate vs overtraining — all three are informative)

### Clinical tier (adds resolution)

These tests resolve specific ambiguities in the self-assessment. They are not required to start — the self-assessment tier is sufficient for initial triage and intervention. They are most valuable when the self-assessment produces ambiguous or contradictory signals.

**Free T3** — the actual active hormone. Not part of standard panels — must be specifically requested. Most informative thyroid test.
- Low free T3 with normal TSH = the TSH trap. The pituitary responds to its own T4-to-T3 conversion, which may be intact while peripheral conversion (where 70-90% of T3 is produced) is impaired.
- High free T4 / free T3 ratio = conversion problem. Potentially DIO2 polymorphism (12-30% of population).
- Elevated rT3 = T4 being diverted to inactive reverse T3 by stress, illness, or inflammation.

**Blood lactate** (fasting) — the most direct single clinical measure of the metabolic fork.
- < 2 mmol/L: normal — the fork is going toward CO2
- 2-4 mmol/L: mild elevation — some metabolic compromise, PDH may be partially blocked
- \> 4 mmol/L: significant — substantial metabolic failure, oxidative capacity impaired

**SHBG** — low SHBG = more free estrogen (and more free testosterone). Both PUFA and insulin resistance lower SHBG. Useful for estimating E when serum estradiol is unreliable.

**Progesterone** — for E/P ratio. The ratio matters more than absolute levels of either. Low progesterone with any estrogen = estrogen dominance regardless of estrogen's absolute level.

**RQ** (respiratory quotient, via indirect calorimetry) — 1.0 = pure glucose oxidation, 0.7 = pure fat oxidation. An RQ of 0.75-0.80 in someone eating adequate carbohydrate means pyruvate is being diverted to lactate or fat storage — the metabolic fork is blocked. Resolves the ambiguity of "is carbohydrate intake adequate or is the fork blocked?"

**ETCO2** (end-tidal CO2) — useful as an individual trend marker. Falling ETCO2 over time within a person reflects their own metabolic trajectory. Cross-population interpretation is complicated by ventilation pattern variability. Not available outside clinical settings.

### Mismatch analysis

Compare observed fast variables (from the measurements above) against the prediction from Pass 1.

**Match (observed matches predicted):** The slow-variable estimate is probably right. The person is at their chronic equilibrium. Intervention targets the slow variables for durable change.

**Observed worse than predicted:** Something acute is layered on top of the chronic state. Look for: recent illness, new medication, life event, seasonal shift, dietary lapse. The chronic landscape may be better than current markers suggest — addressing the acute perturbation may produce faster improvement than the slow-variable estimate would predict.

**Observed better than predicted (the dangerous mismatch):** The person's markers look better than their history suggests they should. This signals compensatory effort — cortisol and adrenaline maintaining function while slow variables degrade underneath. The key unmasking tests:

- The meal test (Pass 3) — compensation collapses when blood sugar normalizes from food
- Morning recovery dynamics (Pass 3) — the nightly conservation dip reveals what daytime compensation hides
- The specific pattern "warm temperature + fast pulse" or "good daytime energy + terrible mornings" = compensation signature

This mismatch is the most important finding the assessment can produce. It identifies people who feel adequate but are on a trajectory toward threshold crossing.

---

## Pass 3: Dynamic Assessment

Static measures capture where the system is. Dynamic measures capture how the system *responds to perturbation* — which reveals how close it is to the threshold and how strong the damping systems are.

### Morning recovery

The organism enters the nightly conservation dip every night (melatonin, cortisol, free fatty acid mobilization, metabolic rate suppression) and must reverse it each morning. The speed and completeness of this reversal is a critical slowing down measurement that occurs naturally every day.

**Protocol:**

Record within 15 minutes of waking:
- Oral temperature
- Subjective energy (1-5 scale: 1 = cannot function, 5 = fully alert and energetic)
- Time of waking

Record again 2 hours after waking (after light exposure and breakfast):
- Oral temperature
- Subjective energy

Do this for at least 5 consecutive days.

**Interpretation:**

| Pattern | What it means |
|---|---|
| Rapid recovery — warm and energetic within 30-60 min, temperature rises >0.5 F by 2 hours | Strong reversal capacity. System exits conservation dip completely. Damping systems intact. |
| Moderate recovery — takes 1-2 hours to feel functional, temperature rises modestly | Incomplete reversal. The nightly dip goes deeper or the morning reversal is slower than optimal. |
| Slow or absent recovery — cold and sluggish for 2+ hours, temperature barely rises | Impaired reversal. The conservation program is not being fully reversed. Strong signal for low M and/or low T. |
| Never reaches full daytime energy — persistent low-grade fatigue all day | Deep nightly dip exceeding recovery capacity. Each cycle may leave a residual deficit. Strongest self-assessment signal for disease-attractor predominance. |

### The meal test

The single most informative free test. It probes M directly by removing adrenaline compensation — when blood sugar normalizes from food, the stress hormones that were maintaining metabolic rate withdraw, revealing the underlying metabolic capacity.

**Protocol:**

Perform fasted in the morning. No coffee or food before the test.

1. Sit quietly for 5 minutes.
2. Record oral temperature and seated resting pulse. (Baseline.)
3. Eat a mixed meal — protein, carbohydrate, and fat. Examples: eggs with toast and butter; yogurt with fruit and honey; milk with a meal. Not just coffee. Not just fruit. A real meal.
4. Record temperature and pulse at 30 minutes and 60 minutes after eating.

Repeat on at least 3 separate mornings to establish pattern. Day-to-day variability (from sleep quality, stress, menstrual cycle, ambient temperature) means a single test is insufficient.

**Interpretation:**

| Response | What it means |
|---|---|
| Temperature rises >= 0.3 F, pulse rises 5-10 bpm | **Adequate M.** Genuine thermic effect — the body is metabolizing the substrate and producing heat. This is what metabolic adequacy looks like. |
| Temperature falls, pulse drops or stays flat | **Impaired M unmasked.** Adrenaline compensation was maintaining temperature; food normalized blood sugar and the stress hormones withdrew, revealing the deficit. This is the most diagnostically valuable result. |
| Temperature flat, pulse spikes > 15 bpm | **Stress response to food.** Possible gut involvement (L), possible blood sugar dysregulation. Not a clear M signal — investigate gut and glucose dynamics. |
| Temperature rises, pulse drops substantially (> 10 bpm) | **Transition from compensation to genuine metabolism.** Adrenaline pulse was high; food allowed the system to switch from stress-driven to substrate-driven metabolism. Usually a positive sign — the underlying capacity is present but was masked. |

**Pattern across multiple days:**

Consistent adequate response across 3+ mornings = high confidence that M is adequate.
Mixed results (adequate some days, impaired others) = borderline M, influenced by day-to-day variables. Investigate what differs on good vs. bad days (sleep, stress, food timing).
Consistently impaired across 3+ mornings = high confidence that M is impaired. Intervention priority: restore M.

---

## Regime Estimation

This section integrates Pass 1-3 into a working regime estimate. It is a probability-weighted judgment, not a binary classification. The estimate will be confirmed or revised by the response to intervention.

### Factors favoring monostable (healthy attractor only)

- Short symptom duration (months, not years)
- Clear precipitating event (recent stress, dietary change, medication, illness, life transition)
- Recovery between episodes — perturbations have historically returned to baseline
- Low estimated P (short PUFA history or long time since change)
- M markers adequate or only mildly borderline
- Fast variables worse than predicted from slow variables (acute perturbation on an intact landscape)
- Young age (less slow-variable accumulation)

### Factors favoring bistable (disease basin exists, system is in it)

- Long symptom duration (years-decades)
- Progressive worsening despite removing known causes — the hysteresis signature
- Multiple systems engaged simultaneously (thyroid + gut + hormonal + inflammatory)
- Failed single interventions — "things help for a while then stop"
- High estimated P with limited time since change
- Multiple M markers converging on impaired (temp, pulse, meal test, morning recovery all pointing the same direction)
- Fast variables matching or better than predicted (the system is at its disease equilibrium, not acutely perturbed — or worse, compensating)
- Slow morning recovery across multiple days
- Discrete historical event after which health never fully recovered (threshold-crossing event)

### When uncertain: default bistable

The asymmetry: a false-positive bistable classification means the person addresses multiple variables when only one was needed — they do more beneficial things than strictly necessary. A false-negative bistable classification means the person addresses one variable when multiple are needed — they spend months on insufficient intervention before the reassessment catches the error.

Default conservative. Expand the intervention set if any 3+ state variables appear impaired.

### Predicted response patterns

The regime estimate produces a predicted response pattern. Write this down. The prediction is checked against reality at 4-8 weeks (fast variables) and 3-6 months (slow variables).

**Monostable prediction:** Clear, progressive improvement within 4-8 weeks of starting the highest-priority interventions. Temperature trend upward, energy improving, symptoms resolving. The improvement continues without plateau because the system is returning to its only attractor.

**Bistable with partially intact slow variables:** Initial improvement (fast variables respond in weeks) followed by plateau (slow variables have not yet shifted). This is NOT treatment failure — it is the expected dynamics. The plateau signals that fast-variable interventions are working but slow-variable resets (PUFA tissue turnover, mitochondrial hardware rebuilding) need time. Continue the intervention set and reassess at 3-6 months for slow-variable movement.

**Bistable with substantially degraded slow variables:** Very slow trajectory. Fast variables may show modest improvement in weeks but the overall picture changes slowly — over months, not weeks. If no improvement at all after 8 weeks of multi-variable intervention, reassess the fundamentals: is the person actually implementing the changes? Is there an unidentified factor (medication, environmental exposure, undiagnosed condition)?

**What confirms the regime estimate:**
- Monostable: progressive improvement without plateau confirms monostable.
- Bistable: initial improvement → plateau → continued improvement after expanding intervention set confirms bistable.

**What revises the regime estimate:**
- Estimated monostable but improvement plateaus at 6-8 weeks → revise to bistable, expand intervention set.
- Estimated bistable but rapid full resolution with minimal intervention → was monostable. Continue simpler approach.
- Improvement followed by regression despite continued intervention → identify what changed (new stressor? dietary lapse? seasonal shift?) or reassess whether an unidentified variable is active.

---

## The Targeted Intervention Map

State-dependent damping is the deepest finding of the stress test: every self-correcting mechanism the body has — antioxidant defense, immune resolution, mitophagy, hormonal homeostasis, lactate clearance — requires ATP to function. When M is low, ALL damping fails. When M is restored, ALL damping re-engages.

This means restoring M is not one priority among six. It is the priority that enables every other. The body does not need the assessment to manually identify and oppose every engaged feedback loop. It needs enough metabolic capacity to run its own correction systems. The intervention map is organized around this principle.

### The universal priority: restore M

Regardless of regime, regardless of which other variables are impaired, these interventions restore oxidative capacity and re-enable damping:

**PDH cofactors** — unlock the metabolic fork. Without these, increased carbohydrate intake produces more pyruvate that cannot be oxidized, paradoxically increasing lactate.
- Thiamine (B1): pyruvate dehydrogenase cofactor — the gatekeeper of the fork
- Magnesium: PDH phosphatase activation (~50% of Americans consume below the EAR)
- Niacinamide: NAD+ precursor — the electron carrier feeding Complex I

**Morning light** — cytochrome c oxidase activation. 670nm light is absorbed directly by Complex IV, improving mitochondrial respiration. Natural sunlight provides this plus circadian entrainment simultaneously. 30-60 minutes within the first hour of waking.

**Adequate substrate** — glucose for oxidation. Fruit, milk, honey. Not on a chronically restricted diet — caloric restriction drives cortisol, which suppresses T4-to-T3 conversion and mobilizes PUFA from storage.

**Thyroid cofactors** — T3 drives respiratory enzyme expression at both genomes. Without adequate T3, the ceiling on oxidative capacity is fixed. Cofactors must be present simultaneously: selenium (deiodinase enzymes AND GPX4 ferroptosis defense), zinc (TPO expression), iodine (substrate).

These four clusters are the "restore M" intervention. They are the starting point for every person assessed by this protocol, regardless of regime or specific variable profile.

### Variable-specific interventions

Beyond the universal M restoration, additional interventions target specific impaired variables:

**P high → PUFA reduction** (`Practice.md` #1)
- Eliminate seed oils. Favor saturated fats (butter, coconut oil, tallow, dairy fat).
- This is the longest game — tissue turnover takes months to years. Start immediately, expect gradual improvement.
- Vitamin E (mixed tocopherols) as a bridge: terminates peroxidation chains while tissue PUFA declines.
- Reduce iron if stores are elevated (iron catalyzes PUFA peroxidation — Loop 1). Donate blood, limit iron-fortified foods.

**T low → thyroid support** (`Practice.md` #2)
- Cofactors first (selenium, zinc, iodine — in the universal M restoration above).
- Remove thyroid suppressors: PUFA (already addressed), chronic stress (#7 below), endotoxin (#5 below).
- If functional markers remain impaired after 4-8 weeks of cofactors + suppressor removal → clinical thyroid assessment. Free T3, free T4/T3 ratio, rT3. Consider DIO2 polymorphism (12-30% of population — T4-only therapy is insufficient for these individuals).
- Coupling note: T and L are linked (Loop 12). Restoring T improves gut motility, which reduces L. Restoring T also improves hepatic estrogen clearance, which reduces E.

**E high → estrogen opposition** (`Practice.md` #6)
- Address upstream conditions first: support thyroid (drives progesterone synthesis and estrogen clearance), reduce PUFA (reduces estrogen amplification via SHBG displacement), reduce stress (restores gonadal progesterone production).
- Progesterone supplementation, if appropriate, directly restores the protective signal — but without upstream corrections, the conditions depleting progesterone remain active.
- Liver support for estrogen clearance: maintain liver glycogen (glucuronidation drops ~80% without it), raw carrot salad (non-fermentable fiber that binds estrogen for excretion).

**L high → gut integrity** (`Practice.md` #5)
- The highest-leverage gut intervention is motility through thyroid support — not probiotics or fiber supplements. Coupling: T → motility → reduced bacterial overgrowth → reduced endotoxin → improved liver → improved T3 conversion → more T. Breaking in from the T side is most effective.
- Adjuncts: raw carrot salad, activated charcoal (intermittent), cascara sagrada (barrier integrity via mitochondrial respiration), glycine/gelatin (TLR4 downregulation).
- Avoid excessive fermentable fibers in a metabolically compromised state — they can increase bacterial toxin production.

**Lambda high → restore M** (Lambda is downstream)
- Chronic lactate clears when oxidative capacity returns. Lactate clearance IS oxidative capacity — when mitochondria can oxidize pyruvate, lactate falls.
- PDH cofactors are the most direct intervention (they unlock the fork that is producing lactate instead of CO2).
- If fasting blood lactate remains elevated despite M restoration interventions → investigate whether the epigenetic lock-in (histone lactylation) is established. This would present as persistently elevated lactate with otherwise improving markers — the metabolic fork is partially unlocked but the gene expression program hasn't fully reversed. Time and continued M support are the primary tools.

### Monostable strategy

2-3 interventions addressing the primary impaired variables, starting with the universal M restoration. The system will return to its only attractor once the perturbation is resolved.

Monitor closely at 4-8 weeks. Progressive improvement confirms the estimate. If improvement plateaus → reassess as bistable and expand.

### Bistable strategy

Address all impaired variables simultaneously. The multi-input threshold nonlinearity predicts that addressing 3+ variables simultaneously produces disproportionately large improvement — the system crosses the separatrix between attractors. This is a structural requirement of the architecture, not a philosophical preference for comprehensiveness.

Priority order within the simultaneous set:
1. Restore M (universal — re-enables all damping)
2. Reduce P (the slow-variable reset that determines whether the disease basin persists)
3. Support T (the rate-setter for M)
4. Reduce L (the gateway stressor that activates everything simultaneously)
5. Oppose E (the glycolytic shift driver — but only after upstream corrections are in place)
6. Address stress and amino acid balance (contextual — metabolic improvements from 1-5 reduce stress load automatically)

The first 4 are the critical simultaneous set for most bistable presentations. Numbers 5-6 add leverage but depend on 1-4 being in place first.

Bedtime nutrition (milk with honey and salt) deserves specific mention for bistable regime: it suppresses the nocturnal hypoglycemia → cortisol → free fatty acid cascade that deepens the nightly conservation dip. In a bistable person, each nightly cycle that goes too deep leaves a residual deficit. Suppressing the cascade reduces this ratchet effect.

---

## Monitoring and Reassessment

### Daily self-monitoring

**Waking temperature and pulse** — record daily. The trend over weeks matters more than any single reading. Look for the temperature trend to move upward as M improves.

**Morning recovery** — note daily: how long after waking until feeling fully functional? Shortening morning recovery time is one of the earliest signs that the organism is exiting the nightly dip more completely.

**Meal test** — perform 1-2x per week initially to establish baseline, then weekly to track trajectory. The response should improve over time: if the meal test showed temperature dropping initially (impaired M) and shifts to temperature rising (adequate M), this is direct evidence of M restoration.

**Energy stability through the day** — fewer afternoon crashes, more consistent energy, less reliance on caffeine or sugar for rescue = less dependence on stress-hormone compensation.

### Clinical monitoring (periodic, if available)

**Blood lactate** (fasting) — the most direct single clinical measure. Falling lactate over months is the clearest objective confirmation that the metabolic fork is shifting toward oxidation.

**Free T3** — if thyroid intervention is active. Tracks the rate-setter.

**ETCO2** — individual trend marker. Rising ETCO2 over time within a person reflects improving oxidative metabolism. Not useful as a one-time snapshot or for cross-population comparison.

**RQ** (via indirect calorimetry) — if accessible. Rising toward 1.0 means glucose oxidation is increasing. The most direct measure of whether the Randle cycle block is resolving.

### Reassessment timeline

**Fast variables (T, L, Lambda): reassess at 4-8 weeks.** These respond on this timescale. Temperature, pulse, meal test response, gut symptoms, and blood lactate (if measured) should show directional change if the interventions are working.

**Regime estimate: reassess at 8-12 weeks based on response pattern.** By this point, the predicted response pattern should be distinguishable from the alternatives. Progressive improvement = monostable confirmed. Improvement → plateau = bistable, expand intervention set. No improvement = reassess fundamentals.

**Slow variables (P, M): reassess at 3-6 months.** Tissue PUFA turnover and mitochondrial hardware rebuilding operate on this timescale. Do not expect or look for slow-variable changes before this. Premature reassessment produces false negatives ("PUFA reduction isn't working" after 6 weeks is not meaningful — the tissue hasn't turned over yet).

### Reassessment triggers

**Improvement stalls after initial progress:** Which slow variable is the bottleneck? Has P had enough time to turn over? Is M hardware rebuilding or just being driven harder by T3? Is there an unaddressed loop (gut integrity, estrogen, chronic stress) that is holding the system in the disease basin?

**New symptoms appear:** May indicate that as one compensatory mechanism is withdrawn, an underlying deficit becomes visible. A person who starts thyroid support and develops new gut symptoms may be experiencing the thyroid-gut coupling in reverse — increased motility revealing bacterial overgrowth that was previously quiescent. This is progress, not regression.

**Improvement followed by regression:** What changed? New stressor? Dietary lapse? Seasonal shift (winter reduces light input)? Medication change? Illness? Identify the perturbation. If nothing identifiable changed, reassess whether the improvement was compensation-driven rather than genuine M restoration.

---

## Signal Conflicts

When markers disagree, the conflict itself is diagnostic. These are the most common patterns and how to interpret them.

### Warm temperature + slow pulse

Most likely: adrenaline-driven warmth with thyroid suppression. The warmth is cortisol/adrenaline compensation; the slow pulse reflects true T3 deficit (T3 drives both metabolic heat AND cardiac chronotropy through different pathways — adrenaline can substitute for the heat but not the chronotropic effect as directly).

What to do: the meal test will usually resolve this. If temperature drops after eating, the warmth was compensatory. Prioritize thyroid support.

### Normal meal test + severe gut symptoms

Most likely: L is the primary driver, independent of current M status. The gut can be the entry point (Loops 10/12) even when systemic M is adequate — endotoxin damages the barrier locally via iNOS → ATP depletion in enterocytes. The rest of the system may still be functioning, but the gateway is open.

What to do: prioritize gut interventions (motility via thyroid support, carrot salad, activated charcoal, cascara) and reassess. If M markers are genuinely adequate, the gut may be the single-variable perturbation in a monostable person.

### Good daytime energy + terrible mornings

Most likely: compensatory effort maintaining daytime function while the nightly conservation dip goes too deep. The person has enough cortisol/adrenaline reserve to power through the day, but the depth of the nightly dip and the slowness of morning recovery reveal the underlying M deficit.

What to do: this is the "fast better than predicted" mismatch — compensation masking degradation. Address the nightly dip directly (bedtime nutrition, evening light management) AND the underlying M deficit. Don't be reassured by the good daytime function.

### Low temperature + fast pulse

Classic adrenaline compensation for hypothyroidism. The body is driving heart rate with stress hormones because thyroid is not providing metabolic drive. Often accompanied by anxiety, tremor, sleep difficulty, or reactive hypoglycemia.

What to do: strongly suggestive of T as primary deficit. Thyroid cofactors + suppressor removal first. The meal test will likely show temperature dropping (stress hormones withdraw as blood sugar normalizes from food, revealing the deficit they were masking).

### Improvement in some markers, worsening in others

Most likely: the intervention is addressing one variable while revealing the deficit in another that was previously masked by compensation. Common example: thyroid support improves energy and temperature but gut symptoms worsen (increased motility revealing bacterial overgrowth). Another: PUFA reduction improves skin and joint symptoms but fatigue temporarily worsens (the system was using PUFA-derived prostaglandins for certain compensatory functions that are now unmasked).

What to do: this is progress, not regression. The newly revealed deficit was always present — the intervention unmasked it. Identify the newly revealed variable and add the corresponding intervention. The trajectory should continue improving as both variables are addressed.

---

## What This Assessment Cannot Determine

**Precise tissue PUFA content.** No accessible measurement exists. The dietary history estimate is the best available proxy, but it cannot account for individual variation in adipose tissue mass, metabolic rate during accumulation, or tissue-specific PUFA incorporation rates. Confidence is medium at best.

**Precise mitochondrial function.** No routine clinical test directly measures mitochondrial oxidative capacity. M is inferred from functional markers, all of which have confounders. The meal test is the best single probe because it unmasks compensation, but even it is an indirect measure. Research-grade tools (Seahorse Bioanalyzer, muscle biopsy for Complex IV activity) exist but are not clinically accessible.

**Tissue estrogen levels.** Blood estrogen levels do not reflect tissue estrogen after menopause (local aromatase produces 5-50x serum concentrations in target tissues). The assessment relies on symptoms and ratio markers, which are informative but imprecise.

**Whether the person is monostable or bistable with certainty.** Regime is estimated from history, trajectory, and marker profile — then confirmed or revised by response to intervention. The parameter-region boundaries (what specific values of P, iron, stress, L place an organism in the bistable region) are currently unknown. The regime estimate is a working hypothesis, not a diagnosis.

**Loop gain.** The assessment identifies which variables are impaired, which points to which feedback loops are engaged. But it cannot determine how strongly engaged each loop is — whether it is weakly active (easily broken by a single intervention) or strongly active (requiring intensive sustained intervention). This distinction matters for prognosis but is invisible to the available measurements.

**The precise threshold location.** The framework predicts that a threshold exists between the monostable and bistable regions, and between the healthy and disease attractors within the bistable region. The assessment cannot determine how close a person is to that threshold. Critical slowing down metrics (morning recovery dynamics, meal test response time) provide indirect evidence of threshold proximity, but the quantitative relationship between these metrics and actual distance-from-threshold has not been established.

---

**This assessment is a starting point.** It produces a working estimate and a predicted response pattern. The response refines the estimate. Each iteration — assess, intervene, monitor, reassess — makes the picture more accurate for this specific person. The protocol is designed to self-correct, but the self-correction requires time (weeks for fast variables, months for slow variables) and honest observation.

It is not a replacement for clinical evaluation. Any person with significant health concerns should work with qualified healthcare providers. The assessment provides a framework for understanding metabolic health that can inform — but not substitute for — clinical care.
