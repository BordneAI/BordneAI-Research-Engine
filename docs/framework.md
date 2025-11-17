# Framework: How to Apply BordneAI to Any Domain

## Universal Methodology for Evidence-Based Analysis

The BordneAI Research Engine applies to **any contested domain**. This document shows how.

---

## Five-Step Workflow

### Step 1: Clarify the Question

**Objective:** Define what you're asking and establish boundaries.

#### 1a. State the Question Clearly
- Write the question in one sentence
- Avoid vagueness ("What happened?" is not specific enough)
- Be concrete and falsifiable

**Examples (Generic):**
- "What was the institutional position on [topic] during [date range]?"
- "What evidence supports [claim] based on T1 and T2 sources?"
- "How do competing hypotheses weight given available evidence?"

#### 1b. Establish Temporal Boundaries
- What time period is relevant?
- Does the question span decades? Months?
- Note: Historical change is real; be precise about timing

**Examples:**
- "During 1995-2000, what was institutional policy on X?"
- "Between event A and event B, what evidence emerged?"

#### 1c. Identify Domain & Scope
- What domain is this question in? (historical, scientific, institutional, policy, etc.)
- Is this a question about facts, motivations, intentions, or institutional behavior?
- What is *out of scope*? (Don't analyze everything; bound your analysis)

**Examples:**
- Domain: "Institutional decision-making"
- Scope: "Public institutional records only; no analysis of private communications"
- Domain: "Historical research"
- Scope: "Evidence available by 2025; does not include future declassification"

#### 1d. Identify Decision-Makers or Affected Parties
- Who cares about this question?
- Whose interests are at stake?
- Who would have relevant knowledge?

This helps identify relevant sources (T1 from authorities, T4 from insiders, etc.).

---

### Step 2: Gather and Classify Evidence

**Objective:** Collect evidence and assign source tiers systematically.

#### 2a. Identify Evidence Sources
Search for evidence across all tiers:
- **T1**: Official sources, declassified records, primary documents
- **T2**: Peer-reviewed research, preprints, technical reports
- **T3**: Reputable secondary sources, established analysis
- **T4**: Testimony, interviews, insider accounts

#### 2b. Classify Each Source
For each piece of evidence, determine:
- What tier is this source? (T1, T2a, T2b, T3, or T4_named/anon)
- When was it created? (Creation date)
- When was it accessed? (Access date for this analysis)
- What is the confidence level? (Based on source authenticity and methodology)

Use SOURCING_PROFILE_V2.1.md for detailed tier definitions.

#### 2c. Flag Contradictions
- Do sources conflict?
- Which tier do they represent?
- Use default hierarchy (T1 > T2 > T3 > T4) unless context suggests otherwise

#### 2d. Assess Source Gaps
- Is evidence available for all parts of the question?
- What evidence is *sealed* (classified, protected)?
- What evidence is *unknown* (not yet discovered)?
- Is there evidence of *suppression*? (Distinguish from sealed or unknown)

**Output: Source Summary**
```
Total sources identified: X
Tier breakdown:
- T1: X sources
- T2: X sources
- T3: X sources
- T4: X sources
Major gaps: [What evidence is missing?]
Contradictions: [Which sources conflict?]
Sealed records: [What's classified?]
```

---

### Step 3: Identify Competing Hypotheses

**Objective:** List all credible interpretations of the evidence.

#### 3a. Brainstorm Hypotheses
For your question, what are the *credible* interpretations consistent with available evidence?

**Criteria for Credibility:** A hypothesis is credible if:
- It is consistent with T1 or T2 evidence
- It is not contradicted by T1 evidence
- It is logically coherent (doesn't violate basic logic)

Do not dismiss hypotheses just because you think one is more likely.

#### 3b. Eliminate Clearly Refuted Hypotheses
If a hypothesis is *explicitly contradicted* by strong T1 evidence, flag it as refuted.

**Example:** "Hypothesis X is explicitly contradicted by [T1 source Y]; confidence: <1%"

#### 3c. Weight Remaining Hypotheses
For each remaining hypothesis, assign preliminary weights based on:
- How much T1/T2 evidence supports this hypothesis?
- How much evidence contradicts it (but doesn't refute)?
- What is the logical coherence?

**Output: Hypothesis List**
```
Hypothesis A: [Description], preliminary confidence: ~60% [evidence base]
Hypothesis B: [Description], preliminary confidence: ~30% [evidence base]
Hypothesis C: [Description], preliminary confidence: ~10% [evidence base]
Refuted: [Hypothesis X] because [T1 contradiction]
```

---

### Step 4: Apply Guardrails & Refine Analysis

**Objective:** Check for reasoning errors and refine hypothesis weights.

#### 4a. Temporal Anchoring Check
- Does every major claim specify *when* it applies?
- Are historical transitions marked with dates?
- Are time periods clearly bounded?

**Correction:** Add specific dates to atemporal claims.

#### 4b. Suppression Claims Check
- Do any claims assert that information is being suppressed?
- If yes: Is there explicit *evidence* of suppression?
- Or is it just sealed/unknown?

**Correction:** Replace unsupported suppression claims with "sealed" or "unknown" classifications.

#### 4c. Competing Hypotheses Check
- Are all credible hypotheses presented?
- Are alternatives dismissed without evidence?

**Correction:** Add missing hypotheses; show evidence for dismissing alternatives.

#### 4d. Language Precision Check
- Scan for hedge words: "may," "might," "could," "possibly," "probably"
- Replace with explicit confidence percentages

**Correction:** Replace hedging with explicit confidence.

#### 4e. Institutional Reasoning Check
- Does analysis explain institutional behavior through incentives?
- Or does it assume conspiracy without evidence?

**Correction:** Replace conspiracy language with institutional incentive reasoning.

#### 4f. Physics/Logic Check
- Do any hypotheses violate basic physics or logic?
- If yes: Is the violation noted explicitly?
- Does the violation eliminate the hypothesis, or just lower its confidence?

**Correction:** Make physics/logic violations explicit; don't use them to dismiss hypotheses without noting.

#### 4g. Sealed/Unknown/Conspiracy Check
- Are these three categories distinguished?
- Is sealed information treated as analyzable (using structural secrecy framework)?
- Is unknown information treated as innocent gap, not conspiracy?

**Correction:** Reclassify information; use appropriate reasoning for each category.

#### 4h. Refine Hypothesis Weights
Based on guardrail corrections, update confidence weights for hypotheses:
- If new evidence emerged during guardrail check: Recalculate weights
- If suppression claims were removed: May need to lower confidence in certain hypotheses
- If institutional incentives were better analyzed: May shift weights toward institutional explanations

**Output: Updated Hypothesis Distribution**
```
Hypothesis A: XX% confidence [guardrail-verified basis]
Hypothesis B: XX% confidence [guardrail-verified basis]
Hypothesis C: XX% confidence [guardrail-verified basis]
Confidence distribution: [A: XX%, B: XX%, C: XX%]
```

---

### Step 5: Structure Final Analysis

**Objective:** Format analysis according to mandatory structure.

#### 5a. Header
```
Question: [Your question]
Domain: [Historical / Scientific / Institutional / Policy / Other]
Entropy Level: [L1-L5]
Source Tier Mix: T1: X%, T2: Y%, T3: Z%, T4: W%
Analysis Date: YYYY-MM-DD
```

#### 5b. Verified Facts (T1/T2 Only)
List facts directly supported by T1 or T2 sources:
```
- [Fact A]: [T1 source, confidence: X%]
- [Fact B]: [T2 source, confidence: X%]
```

#### 5c. Analysis & Interpretation
Separate facts from inference. Show reasoning:
```
Based on verified facts [A] and [B], the evidence supports Hypothesis [X] with [Y%] confidence because [reasoning].

Alternative Hypothesis [W] is also consistent with evidence because [reasoning], receiving [Z%] confidence.
```

#### 5d. Testimony Attribution (if T4 used)
```
T4_named: [Name, credentials, as_of date]: [testimony], confidence: X%

T4_anon: [contextual markers]: [testimony], confidence: X%
```

#### 5e. Structural Secrecy Context
```
Sealed records: [What information is classified/protected?]
Institutional incentive: [Why is it sealed?]
Reasoning about sealed information: [Using institutional incentives, what can we infer?]
Impact on analysis: [How does sealing affect confidence?]
```

#### 5f. Competing Hypotheses (Final)
```
Hypothesis A: [Description], XX% confidence
  Supporting evidence: [T1/T2 sources]
  Contradicting evidence: [sources that challenge this]

Hypothesis B: [Description], XX% confidence
  Supporting evidence: [T1/T2 sources]
  Contradicting evidence: [sources that challenge this]
```

#### 5g. Guardrail Verification
Quick checklist:
```
✓ Temporal Anchoring: Key dates specified
✓ No Unanchored Suppression: Suppression claims have evidence
✓ Competing Hypotheses: All credible alternatives presented
✓ Language Precision: No hedging; explicit confidence
✓ Institutional Context: Incentives explained; no conspiracy
✓ Physics/Logic: Constraints noted where relevant
✓ Sealed ≠ Unknown ≠ Conspiracy: Categories distinguished
```

#### 5h. Next Steps
```
Evidence that would increase confidence in Hypothesis A: [Specific evidence type]
Evidence that would increase confidence in Hypothesis B: [Specific evidence type]
Evidence that would refute Hypothesis C: [Specific evidence type]
```

---

## When the Framework Works Best

The BordneAI framework is most effective for:

### 1. Institutional Decision-Making Questions
**Example Domains:** "What was the institutional position on X?" "Why did institution Y choose policy Z?"

**Why it works:** Institutional behavior is analyzable through incentives; T1 sources (official statements, declassified records) are available; institutional archives provide documentary evidence.

### 2. Historical Research Questions
**Example Domains:** "What evidence exists about historical event X?" "How do historians interpret competing accounts of Y?"

**Why it works:** T1 sources (primary documents) are available; competing historical narratives are well-established; declassification provides new evidence over time.

### 3. Scientific Anomaly Questions
**Example Domains:** "What does research show about phenomenon X?" "How do competing scientific hypotheses weight?"

**Why it works:** T2 sources (peer-reviewed research) are comprehensive; methodology is transparent; hypothesis competition is standard scientific practice.

### 4. Policy Analysis Questions
**Example Domains:** "What are the institutional incentives behind policy X?" "Why did institution Y change policy Z?"

**Why it works:** Institutional records exist; policy rationales are documentable; incentive analysis is rigorous; alternatives can be identified.

### 5. Contested Domain Questions (Generally)
**Characteristics:** Evidence is incomplete, contested, or sealed; multiple credible interpretations exist; stakes are institutional or historical.

**Why it works:** Framework is designed precisely for contested domains where uncertainty is genuine.

---

## When the Framework Doesn't Work (or Requires Modification)

### 1. Questions Requiring Prediction
**Problem:** The framework is designed for *analyzing existing evidence*, not predicting futures.

**Limitation:** Cannot forecast what will happen if evidence about future incentives, decisions, or events is unavailable.

**Modification:** Can analyze *institutional scenarios* ("If X happens, institution will likely Y") using institutional incentive reasoning, but not genuine prediction.

### 2. Questions About Unknowable Subjective States
**Problem:** Can only analyze objective evidence; cannot know internal thoughts without evidence.

**Limitation:** Questions like "What was person X really thinking?" cannot be answered without testimony or documentary evidence.

**Modification:** Can analyze *revealed preferences* (what behavior shows about incentives) or *institutional positions* (what organizations stated), not private thoughts.

### 3. Questions Lacking Evidence Anchoring
**Problem:** Framework requires T1/T2 evidence baseline; pure speculation is refused.

**Limitation:** Questions with zero T1/T2 evidence (Entropy Level L5) must be refused.

**Modification:** Can reframe to analyzable question ("Given X is sealed, what institutional incentives suggest about likely content?") but cannot analyze pure speculation.

### 4. Questions Outside Knowledge Cutoff
**Problem:** Framework requires documented evidence; future events are not yet documented.

**Limitation:** Cannot analyze events post-dating available evidence base.

**Modification:** Can analyze *precursors* and *institutional incentives* suggesting what future events might occur, but not the events themselves.

---

## Practical Checklist: Is My Question Analyzable?

Before starting analysis, check:

- [ ] Question is **specific and falsifiable** (not vague)
- [ ] **Temporal boundaries** are clear (what time period?)
- [ ] **Domain** is identified (historical, scientific, institutional, etc.)
- [ ] **Some T1 or T2 evidence** exists (otherwise Entropy L5; will be refused)
- [ ] **Reasonable person could disagree** on answer (contested, not settled)
- [ ] Question **does not require prediction** of genuinely unknown future
- [ ] Question **does not require access to sealed records directly** (but reasoning about them is OK)
- [ ] **Multiple hypotheses are credible** (if only one possible answer exists, framework is overkill)

If all boxes check, proceed with five-step workflow above.

---

## Example Applications (Generic Scenarios)

### Scenario 1: Institutional History
**Question:** "What was institution X's stated position on policy Y between 1990-2000, and did it change?"

**Applicable because:**
- Clear temporal boundaries (1990-2000)
- T1 sources exist (official statements, policy documents)
- Multiple credible positions possible
- Institutional records analyzable through incentives

### Scenario 2: Scientific Controversy
**Question:** "How do competing hypotheses about phenomenon X weight based on available research?"

**Applicable because:**
- T2 sources exist (peer-reviewed research)
- Multiple credible interpretations exist
- Methodology is transparent
- Bayesian weighting is standard

### Scenario 3: Historical Interpretation
**Question:** "What does evidence show about historical event Y, and what are competing interpretations?"

**Applicable because:**
- Primary sources available (T1)
- Competing historical narratives exist
- Declassification reveals new evidence over time
- Temporal anchoring is clear

### Scenario 4: Intelligence Analysis
**Question:** "Given institutional behavior pattern Z, what incentives explain it, and what does it suggest about institutional intentions?"

**Applicable because:**
- Institutional behavior is observable
- Incentives framework applies
- Multiple plausible explanations exist
- Sealed records can be reasoned about using incentives

---

## Version & References

**Version**: 1.0
**Last Updated**: 2025-11-17

For detailed sourcing rules, see SOURCING_PROFILE_V2.1.md
For guardrails and error detection, see GOVERNANCE.md
For system instructions, see SYSTEM_PROMPT-v3.0.md
