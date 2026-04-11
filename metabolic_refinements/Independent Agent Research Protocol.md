# Independent Agent Research Protocol

## Purpose of This Document

This document specifies how to use independent agent research as a **triangulation tool** for complex questions in this workspace. It is a methodology, not a briefing — the briefing docs themselves are one-shot artifacts tailored to specific questions, while this protocol describes the reusable pattern for how to construct them, how to run the consultation, and how to critically assess the outputs.

**The core insight:** when a question is complex enough that single-pass reasoning loops or risks missing blind spots, independent agent perspectives can catch errors, surface alternative angles, and stress-test conclusions. But agents are not oracles — their value comes entirely from being **critically assessed** against first principles and against what we already understand. The triangulation only works if the assessment is done honestly: updating when the evidence is sound, holding when it isn't.

This protocol is written for future Claude sessions (or other agents) working in this vault who want to run this kind of triangulation properly. Read it in full before using it.

---

## When to Use This Approach

Use independent agent research when:

- A claim is **load-bearing enough** that getting it wrong would degrade the integration substantially
- The **evidence is genuinely complex** — multiple conflicting findings, nuanced mechanisms, contested interpretations
- Your own reasoning is **looping or circling** without clear resolution
- The question has **enough nuance** that a single reasoning pass might miss important angles
- You want to **catch blind spots** in your own analysis
- You've already done substantial work on the question and want **independent stress-testing** rather than fresh primary research

**Do NOT use this approach for:**

- **Simple factual lookups.** Direct search is faster and more reliable.
- **Claims already well-understood.** Confirmation wastes effort.
- **Questions where the primary literature is sparse.** Agents can't conjure data that doesn't exist.
- **Problems you haven't yet reasoned through yourself.** Your own first-pass reasoning is cheaper and better-grounded before you add external perspectives — you also can't critically assess agent output on a topic you haven't thought through.

The protocol is valuable when you've **earned the right to consult**: you've done your own work, identified the real tension, and need independent eyes to test whether your reasoning is sound.

---

## Core Principles

**Agents are independent perspectives, not oracles.** Their output is an input to your own critical thinking, not a replacement for it. Treat agent reports the way you treat primary literature: evaluate the evidence and reasoning, don't defer to authority.

**Convergence across agents is stronger evidence than a single agent.** When multiple independent agents reach the same conclusion via matching reasoning, that's meaningful signal. When they diverge, the divergence is diagnostic — it usually reveals where the question is genuinely uncertain.

**First principles is the reference standard, not agent consensus.** If all agents converge on a conclusion but it contradicts first-principles biochemistry, physics, or logic, the agents are wrong. Never surrender first-principles reasoning to consensus.

**Self-contained context is non-negotiable.** If the briefing doc isn't comprehensive enough for an agent with zero prior context, the agent will fill gaps with assumptions and the entire triangulation becomes worthless. Over-include context rather than under-include.

**The briefing is a research document, not a letter to an agent.** Write it to stand alone as a research brief that any researcher or LLM could read cold and understand what to analyze. Do NOT write sections addressed to "the agent" with phrases like "you are being asked" or "we want you to" — that meta-framing confuses agents who don't have context that they are part of a multi-agent consultation process. The substance should be identical, but phrased as research objectives and tasks rather than as instructions to a consultant. If the brief reads naturally when you imagine handing it to a stranger who asks "what is this?", it's framed correctly.

**Don't bias the framing.** Present findings as facts, not as interpretations. Share open questions honestly. Include an explicit statement in the brief that if the evidence leads to a different conclusion than the current position, that conclusion should be stated — but frame it as an epistemic principle for the analysis, not as a "we welcome your disagreement" meta-statement addressed to a consultant.

**Critical assessment is where the value lives.** Writing the briefing and receiving reports is the cheap part. The expensive, load-bearing work is evaluating what the agents said against first principles and against your own understanding. Skipping this phase defeats the entire purpose.

---

## Phase 1: Constructing the Briefing Document

The briefing must be **self-contained** — an agent reading it cold, with no other access to the vault or our conversation, should have everything needed to reason about the question independently. Over-include rather than under-include.

Required sections, in this order:

### 1. Research Objective

State the substantive question the brief is asking to analyze and why it matters. Frame it as a research goal, not as an address to an agent. The section should read as "we need first-principles analysis of X because Y" — not "you are being asked to analyze X." Explicitly state, as an epistemic principle, that if the evidence leads to a conclusion contradicting the framing in the brief, that is the correct answer and should be stated with reasoning. Keep it neutral: the brief should work as a self-contained research document handed to any researcher or LLM cold, not as a letter addressed to a consultant.

### 2. Project Context

Brief, focused context:
- What the vault is and what it's trying to do (find what's most true, not defend a framework)
- The project's explicit goal of correction over defense
- **Prior self-corrections** as concrete examples so the agent knows this framework is willing to update
- The user's values: first-principles reasoning, interconnection awareness, honest calibration, critical thinking

Keep this section tight — enough that the agent understands the stakes and the epistemic posture, no more.

### 3. The Specific Claim Being Tested

The claim stated **verbatim** from the vault, followed by **unpacking of its sub-commitments**. If the claim is ontological ("X IS Y"), spell out what specific positions the identification commits the framework to. Name the load-bearing words (IS, efficient, specifically, etc.).

This section must be precise because imprecision here corrupts everything downstream.

### 4. The Vault's Own Reasoning Chain

Represent the vault's argument **accurately and completely**, not charitably or uncharitably. Include:
- The reasoning steps in order, link by link
- The empirical and textbook foundations the argument rests on
- The vault's own caveats and acknowledged uncertainties (agents should know where the framework has been honest about its limits)
- Any relevant self-corrections the vault has already made on related claims

Fair representation matters because an agent attacking a straw-man version of the claim produces useless analysis.

### 5. First-Principles Verification Material

Anything the agent should be able to verify independently from textbook sources:
- Stoichiometry (balanced equations, ATP yields, substrate ratios)
- Physics/chemistry fundamentals
- Textbook biochemistry/physiology that's not in dispute
- Calculations that can be redone from scratch

Include actual numbers. Agents should verify these, not just accept them. **Explicitly invite them to catch errors in your own calculations.**

### 6. Factual Findings From Research So Far

Everything substantive you've found, presented as **factual data with sources, not as interpretations**. This section is the biggest bias risk — write it carefully.

- Each finding as a data point, not a conclusion
- Source citations inline
- Populations, durations, methods where relevant
- Contradictions or apparent inconsistencies flagged as such
- Nothing framed as "this proves X" or "this suggests the vault is wrong"

The agent should be able to reach a different conclusion from the same data if the evidence warrants it. If the briefing's framing guides them toward your current view, you've wasted the consultation.

### 7. The Research Question and Sub-Questions

State the central question precisely, followed by 3–6 specific sub-questions that decompose it. The sub-questions structure the agent's analysis without prescribing the conclusion.

### 8. Open Questions We Haven't Resolved

What you know you don't know. Being honest about your own uncertainty is important — it prevents the agent from reverse-engineering your position from what you left out, and it signals that you're genuinely asking rather than confirming.

### 9. Research Tasks

List the specific analytical tasks the brief requires, framed as research objectives rather than as instructions to a consultant. Standard tasks include:

1. Independent verification of facts (including the brief's own calculations)
2. First-principles reasoning, not summary of literature
3. Steelman both sides — actually make the strongest version of each, not pro forma
4. Classification using the framework's criteria (typically Pass / Refinement / Fail)
5. Additional literature not already covered
6. Factual errors in the brief itself
7. Epistemic calibration — explicit about what is confident vs uncertain
8. Prioritization: the single most important finding, the biggest remaining uncertainty, the most valuable next test

State in the brief that if the evidence leads to a conclusion different from the framing, that conclusion should be stated with reasoning. Frame this as an epistemic research principle ("factual accuracy and mechanistic correctness are what we need"), not as a meta-statement addressed to a consultant ("we welcome your disagreement"). The former is a research principle that stands on its own; the latter implies a consultation context the reader may not have.

### 10. Methodology Notes

The methodological principles the agent should apply. These may vary by question, but common ones include:

- **Rate vs efficiency distinction.** Same output at different metabolic cost.
- **Acute vs chronic distinction.** Same signal, opposite effects at different timescales.
- **Context-dependence must be falsifiable.** If invoked, the context variable must be specified in advance, independently measurable, and generate directional predictions.
- **Tissue-level vs whole-body level.** Claims that hold at one level don't automatically generalize.
- **Integration principle.** Vault claims are interconnected; evaluating one requires attention to its connections.
- **Evidence must measure the right variable.** A study measuring proxy X cannot confirm or deny a claim about mechanism Y.

This lets the agent apply the same rigor you would.

### 11. Response Format

Specify the desired response structure so results are actionable:
- Classification with specific reasoning
- Strongest single finding (the one piece of evidence that most informs the classification)
- Biggest remaining uncertainty (what would need to be measured to resolve it)
- Specific edits recommended (if Refinement) — concrete text, not vague directions
- Factual errors in the brief itself
- Additional literature not covered
- Most valuable next test

Specify that the response should be detailed enough to show reasoning, concise enough to be actionable. Frame this as format guidance for the analysis, not as instructions addressed to a consultant.

### 12. Sources Already Used

Full URL list. Lets the agent verify primary sources and avoid duplicating searches already performed.

### 13. Note on Epistemic Stance (Optional)

Optionally include a brief closing note stating that the framework is willing to be corrected, that prior self-corrections are concrete evidence of this, and that a classification of Fail (if the evidence warrants) is as useful as Refinement. Frame this as epistemic context for the analysis, not as a consultation preamble. Keep it short — two or three sentences. Skip this section entirely if the Research Objective (Section 1) already conveys the epistemic stance clearly — duplication reads as meta-framing.

---

## Phase 2: Running the Consultation

Two workflows are valid for dispatching agents. The protocol works agnostically for both — the difference is only in who spawns the agents and how the responses arrive.

**Workflow A — Main assistant dispatches directly.** The main assistant spawns multiple independent sub-agents in parallel via its Agent tool, each given the same briefing file and running with no knowledge of the others. Responses come back through the tool and are saved to temporary files for critical assessment. Use this when the main assistant has agent-dispatching tools and the user is comfortable delegating the running.

**Workflow B — User runs external agents and pastes responses back.** The user takes the briefing document and feeds it to external agents (separate Claude sessions, other models, or a mix). Agents analyze independently. Their responses are pasted back into the conversation with the main assistant, who then performs the critical assessment phase. Use this when the user wants direct control over which agents are consulted, wants to use models the main assistant cannot dispatch, or wants to verify each agent's thinking before it enters the synthesis step.

In either workflow, the core principles are identical:

- **Multiple agents in parallel where possible.** Two independent perspectives are meaningfully stronger than one; three is the practical upper bound before diminishing returns. Each agent gets the same briefing with **no knowledge of the others**.
- **No interaction during reasoning.** Don't feed agents intermediate results or each other's outputs. The independence is the whole point.
- **Don't read any agent output while your own analysis is in flight.** Hold your own position first, so the agents' reports don't anchor you before you've finished your own work.
- **Preserve agent responses as temporary files** during the critical assessment phase so they can be re-read as needed. In Workflow A the main assistant writes them after dispatch; in Workflow B the main assistant may write them to disk for record-keeping after the user pastes them. Delete after synthesis — don't leave them as permanent workspace clutter.

---

## Phase 3: Critical Assessment of Agent Output

This is the most important phase. The briefing was cheap; the critical assessment is where the value lives. **Do not skip this phase, even when the agents' conclusions match yours — especially then.**

For each agent report, evaluate:

### Factual Accuracy
- Do their claims match the primary literature they cite?
- Do they match the biochemistry / physics / textbook foundations you've verified independently?
- If they cite specific numbers, are the numbers right? (Check at least the most load-bearing ones.)
- If you can't immediately verify, note it and check later.

### Depth of Reasoning
- Did they actually reason from first principles, or just summarize literature?
- Did they trace the prediction chain link by link?
- Did they distinguish what's textbook from what's contested?
- Shallow summary without reasoning is low-value even if the classification happens to be correct.

### Honest Steelmanning
- Did they make the strongest possible case for both sides, or did they half-heartedly do one side?
- Pro forma steelmanning is a tell of weak analysis.
- A good report makes the opposing case well enough that you could mistake it for the agent's actual position.

### Classification Logic
- Does their classification actually follow from the evidence they present?
- Or did they leap to a conclusion the evidence doesn't support?
- Watch for confident-sounding conclusions without matching evidentiary weight.

### What They Caught That You Missed
- New angles you hadn't considered
- Overlooked literature
- Biochemical or mechanistic subtleties
- Factual errors in your own prior analysis
- **Take these seriously and update your position where warranted.** This is the primary value of the consultation.

### What They Missed That You Caught
- Gaps in their analysis
- Findings from your own research they didn't address
- Angles they didn't engage with
- Don't just assume they saw everything — spot-check what they left out. An agent's silence on a key finding is not endorsement.

### Convergence vs Divergence Across Agents
- Where multiple agents reach the same conclusion via the same reasoning, convergence is meaningful signal
- Where they diverge, the divergence is diagnostic — it usually reveals where the question is genuinely uncertain or where one agent missed something specific
- **If their convergent conclusion contradicts first principles or bedrock facts, first principles wins.**

---

## Phase 4: Synthesis

Integrate the agents' findings with your own analysis:

1. **Accept factual corrections** where the agents caught errors in your biochemistry, citations, or claims. Write down explicitly what changed and why. Verify the correction against a primary source before accepting it — don't just take the agent's word.
2. **Update reasoning** where the agents' logic is sound and adds something you missed. Don't resist updating just because it changes your prior position — that's the whole point of the exercise.
3. **Hold your ground** where the agents' reasoning is flawed or where first principles override their conclusions. Don't cave to consensus when your reasoning is better grounded.
4. **Identify the convergent core** — the claims that survived triangulation — and treat those as well-tested.
5. **Identify residual uncertainty** — claims where agents diverged or where the evidence is genuinely incomplete — and flag them as carry-forward items.
6. **Document the synthesis in the working log**: what the agents added, what you corrected, what you held, what remains open. The synthesis is the permanent record; the individual agent reports are ephemeral.
7. **Commit the updated state** so the triangulation outcome is durable.

---

## Phase 5: Housekeeping

- **Briefing docs are one-shot artifacts.** They're tailored to a specific question and lose their value once that question is answered. Delete them after the work is complete unless the structure is worth preserving as a reusable template. Git history retains them if future reference is needed.
- **Agent response files are temporary.** Transcribe the key findings into the permanent record (the tracking doc, the vault corrections, the working log), then delete the response files. They're conversation artifacts, not canonical records.
- **Update the carry-forward items section** (or equivalent running log of open questions) with any new uncertainties that surfaced during triangulation.
- **Commit with a clear message** describing the triangulation outcome so the git history is meaningful and the work can be picked up by a future session cold.

---

## Anti-Patterns to Avoid

**Using agents as a shortcut instead of as stress-testing.** If you haven't done your own reasoning first, agent consultation wastes effort. You can't critically assess what you haven't already thought through.

**Taking agent output at face value.** Agents can be confidently wrong, confidently vague, or confidently shallow. Always critically assess, even when the conclusion matches yours.

**Deferring to consensus against first principles.** If all agents agree on a conclusion that contradicts bedrock biochemistry or the vault's own logic, trust first principles, not consensus.

**Writing briefings that bias toward your current view.** If the briefing's framing guides the agent toward your conclusion, you've wasted the consultation. Present findings neutrally.

**Under-including context to save tokens.** A briefing that leaves the agent guessing at context produces worthless analysis. Over-include.

**Accepting corrections without verifying.** Just because an agent flags a factual error doesn't mean they're right. Check the primary source before updating the record.

**Rubber-stamping when the work feels done.** If you're tempted to skip the critical assessment phase because the agent's conclusion matches yours, that's exactly when critical assessment matters most. Do it anyway.

**Piling agents on every question.** Triangulation is expensive in attention. Reserve it for questions where the added rigor is justified.

**Leaving agent response files around.** They're conversation artifacts, not canonical records. Transcribe what matters and delete the originals.

---

## Summary Checklist

**Before using this protocol:**
- [ ] Have I done my own first-pass reasoning on this question?
- [ ] Is the question load-bearing enough to justify the effort?
- [ ] Are there identifiable open angles I can't resolve alone?

**Constructing the briefing:**
- [ ] Is it self-contained for a reader with no prior context?
- [ ] Does it read as a research document, not a letter addressed to an agent? ("We need analysis of X" not "You are being asked to analyze X.")
- [ ] Are findings presented as data, not interpretations?
- [ ] Have I included first-principles verification material with actual numbers?
- [ ] Have I represented the framework's reasoning fairly (not as a straw man)?
- [ ] Have I stated that different conclusions are valid, framed as an epistemic principle (not as a "we welcome your disagreement" meta-statement)?
- [ ] Have I included methodology principles for the analysis to apply?
- [ ] Have I specified the response format expected?

**Running the consultation:**
- [ ] Am I holding my own position before reading any agent output?
- [ ] Are the agents working independently with no knowledge of each other?

**Critical assessment:**
- [ ] Did I verify load-bearing factual claims in each report?
- [ ] Did I check whether their reasoning actually supports their classification?
- [ ] Did I spot-check what they left out?
- [ ] Did I check convergence and divergence across agents honestly?
- [ ] Did I apply first-principles reasoning to their conclusions, not just accept them?

**Synthesis:**
- [ ] Have I accepted corrections where warranted (and verified them against primary sources)?
- [ ] Have I held ground where first principles override their reasoning?
- [ ] Have I documented what changed, what held, and what remains open?
- [ ] Have I updated carry-forward items with new uncertainties?
- [ ] Have I cleaned up the one-shot artifacts (briefing, agent responses)?
- [ ] Have I committed the updated state with a clear message?

---

## Final Note

The failure mode to guard against most carefully is **deference**. Agent output can feel authoritative because it's comprehensive, cited, and structured — but it's just another perspective, subject to the same error modes as any other analysis. The triangulation protocol is only valuable if you remain willing to say "the agents all agree on this and they're all wrong, because [first-principles reason]."

The point of consulting independent agents is not to outsource the thinking. It's to expose your own reasoning to perspectives that don't share your assumptions, catch what you missed, and stress-test what you concluded. The thinking — the critical, first-principles, interconnection-aware thinking — stays with you.

Use this protocol when it helps. Don't use it when it doesn't. And never let it replace your own judgment.
