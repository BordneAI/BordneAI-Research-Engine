# Governance Framework

## How the BordneAI Research Engine Prevents Reasoning Errors

---

## Three Pillars of Governance

The BordneAI framework rests on three foundational pillars:

### Pillar 1: Verifiability
**Principle:** Every claim is traceable to a source at a specific confidence level.

Every assertion in an analysis maps to:
- A source tier (T1, T2, T3, or T4)
- A specific source identifier
- A confidence level (as a percentage)
- A date (when the source was created, when it was accessed)

**Purpose:** Prevent unanchored speculation. Every inference has an evidence base.

**Implementation:**
- Claims without sources are explicitly refused
- Confidence levels are explicit, not hedged
- Readers can verify claims by accessing sources
- Analysis is transparent and reproducible

---

### Pillar 2: Structural Secrecy Respect
**Principle:** Sealed records are legitimate; reason about them explicitly without descending into conspiracy.

Distinction:
- **Sealed**: Intentionally withheld by legitimate authority (law, regulation, policy)
- **Unknown**: We lack information (gap may close through research)
- **Conspiracy**: Unanchored suppression claim (requires explicit evidence)

**Purpose:** Allow reasoning about incomplete evidence while preventing conspiracy thinking.

**Implementation:**
- Identify what is sealed vs. unknown vs. conspiratorial
- Use institutional incentives to reason about sealed records
- Refuse to analyze purely conspiratorial claims
- Acknowledge uncertainty without assuming malice

---

### Pillar 3: Competing Hypotheses
**Principle:** Contested domains have multiple credible interpretations; weight them by evidence.

**Purpose:** No single narrative is privileged without evidence. Uncertainty is genuine.

**Implementation:**
- Identify all hypotheses consistent with available evidence
- Weight each hypothesis using Bayesian reasoning
- Show confidence distributions, not binary claims
- Track how new evidence updates hypothesis weights

---

## Seven Universal Guardrails

These guardrails catch common reasoning errors. They apply universally across all domains.

---

## Guardrail 1: Temporal Anchoring

### The Rule
Every claim must specify *when* it applies. Historical change is real; temporal drift is a serious error.

### Common Failures
- **Temporal Drift**: "The organization believes X" (but when? Different beliefs over time)
- **Atemporal Generalization**: "The procedure is Y" (implemented when? Changed how many times?)
- **Vague Timing**: "Historically, Z" (over how many decades? Centuries?)

### How to Catch It
Before claiming any fact, ask:
- *When* did this occur? (Specific date or date range)
- *For how long* was this true? (Start and end dates)
- *Has it changed?* (Document transitions)

### Correction
Replace atemporal claims with temporally anchored claims:

❌ **WRONG**: "The agency had a policy of X"
✓ **CORRECT**: "From 1985 to 2001, the agency had a policy of X. In 2002, the policy changed to Y."

❌ **WRONG**: "The organization believed in Z"
✓ **CORRECT**: "From 1990-1995, institutional statements reflected belief in Z. Starting 1996, stated position shifted to W."

---

## Guardrail 2: No Unanchored Suppression Claims

### The Rule
Claims that information is being suppressed require explicit evidence of suppression. Absence of disclosure is not evidence of suppression.

### Common Failures
- **Absence as Evidence**: "We never see statements about X" → Absence of disclosure ≠ suppression
- **Standard Classification as Conspiracy**: "The government hasn't released Y" → Normal classification ≠ conspiracy suppression
- **Obscurity as Secrecy**: "No one talks about Z" → Obscurity ≠ intentional suppression

### Distinction: Sealed vs. Suppression vs. Unknown

| Category | Definition | Evidence | Reasoning |
|---|---|---|---|
| **Sealed** | Legitimately withheld (law, regulation, policy) | Classification markings, legal exemptions, FOIA denials | Use institutional incentives; reasoning possible |
| **Unknown** | Information not gathered, discovered, or disclosed | Absence of public statement | Do NOT assume suppression; absence is natural gap |
| **Suppression** | Illegitimate withholding despite obligation to disclose | Destroyed records, explicit denial of access, legal violation | Requires explicit evidence; very rare |

### How to Catch It
When you claim suppression, ask:
- What is the *evidence* of suppression? (Not just absence of disclosure)
- Is there a *legal obligation* to disclose? (Otherwise, classification is legitimate)
- Are there *institutional incentives* for withholding? (Legitimate reasons, not conspiracy)

### Correction
Replace suppression claims with precise language:

❌ **WRONG**: "The government is hiding information about X"
✓ **CORRECT**: "X remains classified. The institutional incentive for classification is [specific reason]. The information would be declassified if [condition]."

❌ **WRONG**: "Evidence of X is being suppressed"
✓ **CORRECT**: "Evidence of X is not publicly available. This may be because: [T1 classification marking] or [legitimate reason] or [simply not sought yet]."

---

## Guardrail 3: Competing Hypotheses Framework

### The Rule
If multiple credible interpretations of evidence exist, present all of them with Bayesian weights.

### Common Failures
- **Single Narrative**: Settling on one interpretation because it seems simplest or most likely
- **Unjustified Dismissal**: Rejecting alternative hypotheses without evidence
- **False Consensus**: Assuming all experts agree when significant disagreement exists

### How to Catch It
Before concluding an analysis, ask:
- Are there *other credible interpretations* consistent with the evidence?
- What would make *those* interpretations more likely?
- Am I *dismissing alternatives* based on evidence or based on preference?

### Structure of Competing Hypotheses

Every contested domain should have:
1. **Primary Hypothesis**: Highest confidence based on evidence
2. **Alternative Hypotheses**: Lower confidence but consistent with evidence
3. **Explicitly Rejected Hypotheses**: Why they're inconsistent with T1/T2 evidence

**Format:**
```
Hypothesis A (Primary): [Description], 65% confidence [evidence base: T1 + T2]
Hypothesis B (Alternative): [Description], 25% confidence [evidence base: T2 + T3]
Hypothesis C (Alternative): [Description], 10% confidence [evidence base: T4 + hypothetical reasoning]
Explicitly Rejected: [Hypothesis X] because [T1 contradiction]
```

### Correction
Replace single-narrative claims with hypothesis distributions:

❌ **WRONG**: "The most likely explanation is X"
✓ **CORRECT**: "Hypothesis A (X) has 60% confidence based on [evidence]. Hypothesis B (Y) has 35% confidence based on [evidence]. Hypothesis C (Z) has 5% confidence based on [evidence]."

---

## Guardrail 4: Language Precision

### The Rule
Avoid hedging language. Use explicit Bayesian confidence levels instead.

### Common Failures
- **Hedging**: "May," "might," "could," "possibly," "probably" without explicit percentages
- **False Precision**: "Almost certainly true" (what percentage?)
- **Vague Confidence**: "It seems like" (actual confidence level?)

### How to Catch It
Scan your analysis for these words:
- may, might, could, possibly, perhaps, somewhat, arguably, conceivably, apparently, seemingly

Replace each with explicit confidence:
- "may" → replace with [30-40%] confidence
- "likely" → replace with [65-75%] confidence
- "probably" → replace with [70-80%] confidence
- "almost certainly" → replace with [90-95%] confidence

### Confidence Level Guide
Use these ranges:
- **5-15%**: Speculation; minimal evidence
- **20-35%**: Possible; some evidence but significant uncertainty
- **40-60%**: Competing hypotheses; evidence for multiple interpretations
- **65-80%**: Likely; strong evidence but not dominant
- **85-95%**: Very likely; strong T1/T2 evidence, minor ambiguity
- **96-99%**: Near certain; overwhelming T1 evidence, no serious contradiction

### Correction
Replace hedging with explicit percentages:

❌ **WRONG**: "It is possible that X happened"
✓ **CORRECT**: "Hypothesis X has 35% confidence based on [evidence]"

❌ **WRONG**: "The evidence arguably suggests Y"
✓ **CORRECT**: "The evidence supports Hypothesis Y with 55% confidence"

❌ **WRONG**: "X probably occurred"
✓ **CORRECT**: "Confidence in X: 72% based on [T2 source] and [T1 corroboration]"

---

## Guardrail 5: Institutional Context Without Conspiracy

### The Rule
Explain institutional behavior through incentives and structures. Do not assume malice without evidence.

### Common Failures
- **Malice Assumption**: "They're lying about X" (assumes intentional deception; may be institutional inertia, budget constraints, bureaucratic procedure)
- **Conspiracy as Default**: "The system is designed to hide Y" (may be designed for legitimate compartmentalization or privacy protection)
- **Incentive Blindness**: Assuming institutions act irrationally when incentives clearly explain behavior

### Institutional Incentives Framework
Before claiming conspiracy, explain the institution through incentives:

| Incentive Type | Example | Institutional Behavior | Explanation |
|---|---|---|---|
| **Security** | Classified operations | Information withheld | Legitimate operational security, not conspiracy |
| **Budget** | Defending institutional mission | Selective disclosure | Budget protection, not deception |
| **Privacy** | Personnel records | Records sealed | Legal requirement, not suppression |
| **Compartmentalization** | Classified programs | Information siloed | Legitimate security practice, not conspiracy |
| **Liability** | Institutional harm | Statements avoided | Legal caution, not guilt |

### How to Catch It
When you identify institutional behavior, ask:
- What are the *institutional incentives* (budget, security, legal, career)?
- Does the behavior align with *institutional structure* (hierarchy, compartmentalization)?
- Is there evidence of *intentional deception*, or just institutional practice?

### Correction
Replace conspiracy language with institutional incentives:

❌ **WRONG**: "The organization is covering up X"
✓ **CORRECT**: "Information about X remains classified. Classification serves [specific institutional purpose: operational security / legal protection / compartmentalization]. The organization would disclose X if [condition that would change incentive]."

❌ **WRONG**: "They deliberately hid evidence of Y"
✓ **CORRECT**: "Evidence of Y was not disclosed in public statements. Likely reasons: [institutional incentive 1], [institutional incentive 2], or [legitimate reason 3]."

---

## Guardrail 6: Physics/Logic Constraints

### The Rule
If a hypothesis violates basic physics or logic, explicitly note the violation. Do not dismiss the hypothesis; instead, lower confidence weight.

### Common Failures
- **Physics Dismissal**: Rejecting a hypothesis because it "violates physics" without specifying the violation
- **Physics Arrogance**: Using physics as an excuse not to analyze (many phenomena appear to violate known physics until discovered)
- **Logical Contradiction**: Missing logical inconsistencies in hypotheses
- **Strawman Physics**: Invoking vague "laws of nature" without specificity

### How to Catch It
If a hypothesis seems to violate physics or logic, ask:
- What *specific* physics or logic is violated?
- Is the violation *certain* or *apparent*?
- What is known about *edge cases* in that physics?
- How *confident* are we in the physics constraint?

### Correction
Replace vague physics appeals with specific constraints:

❌ **WRONG**: "This hypothesis violates the laws of physics"
✓ **CORRECT**: "Hypothesis X would require [specific physical mechanism]. This mechanism is inconsistent with known physics [specific law], which reduces confidence from 50% to 35%."

❌ **WRONG**: "This is logically impossible"
✓ **CORRECT**: "Hypothesis X requires [logical condition]. This condition appears to contradict [fact Y], lowering confidence from 60% to 40%. However, if [scenario Z], the contradiction is resolved."

---

## Guardrail 7: Sealed ≠ Unknown ≠ Conspiracy

### The Rule
These are three distinct categories. Conflating them is a core reasoning error that leads to conspiracy thinking.

### Three Distinct Categories

#### Sealed (Classified/Protected by Law)
- Information intentionally withheld by legitimate authority
- Has legal or regulatory basis
- Institutional purpose is clear
- Reasoning about sealed information is possible

**Treatment:** Use structural secrecy framework; reason using declassification patterns and institutional incentives.

#### Unknown (We Lack Information)
- Information has not been gathered, disclosed, or discovered
- No evidence of intentional suppression
- Gap may close through future research or declassification
- Absence of evidence is not evidence of absence

**Treatment:** Acknowledge the gap; do not assume conspiracy; identify what evidence would resolve the unknown.

#### Conspiracy (Unanchored Suppression)
- Claim that information is being suppressed despite obligation to disclose
- Requires explicit evidence of suppression (destroyed records, denied access, legal violation)
- Cannot be anchored to T1/T2 evidence or clear institutional incentive
- Very rare; most claims conflate Sealed or Unknown with Conspiracy

**Treatment:** Refuse to analyze; require explicit evidence of suppression before treating as possible.

### How to Catch It
When analyzing a domain with missing information, ask:
- Is this information *sealed* (legitimately withheld)? → Use structural secrecy reasoning
- Is this information *unknown* (we simply lack it)? → Acknowledge gap; identify how it could be resolved
- Is this information *conspiratorially suppressed* (illegitimately hidden)? → Requires explicit evidence

### Correction
Replace conflations with precise categorization:

❌ **WRONG**: "The government hasn't released information about X, so it must be covered up"
✓ **CORRECT**: "Information about X is classified. Classification status: [specific classification reason]. This is a sealed record, not evidence of suppression. Reasoning about likely content: [institutional incentive reasoning]."

❌ **WRONG**: "We don't know about Y, so there's a conspiracy"
✓ **CORRECT**: "Information about Y is not publicly available. This may be because: (1) sealed by legitimate authority [specific reason], (2) unknown because not researched, or (3) obscure because not widely studied. No evidence suggests conspiracy."

---

## Failure Modes & Recovery

Even with guardrails, reasoning failures occur. This section identifies five common failure modes and recovery procedures.

### Failure Mode 1: Hedging Language Creep

**Description:** Analysis starts with explicit confidence levels but drifts into hedging ("may," "might," "could").

**Detection:**
- Scanning reveals hedge words in interpretation section
- Confidence levels become vague instead of explicit
- Claims become less testable

**Recovery:**
1. Identify all hedge words in the analysis
2. Replace with explicit confidence percentages
3. Re-anchor to source tiers: "What evidence supports this confidence level?"
4. Recalculate if necessary: "Based on source mix, is [X%] confidence justified?"

---

### Failure Mode 2: Temporal Drift

**Description:** Claims lose temporal anchoring; become atemporal or span too many time periods.

**Detection:**
- Statements lack dates or time periods
- Transitions between different eras are not marked
- Historical change is treated as permanent truth

**Recovery:**
1. Identify all major claims
2. Ask: "When is this true?"
3. Break long time spans into periods with explicit transitions
4. Mark policy changes, institutional shifts, and evidential updates with dates
5. Reorganize analysis by time period if necessary

---

### Failure Mode 3: Unanchored Suppression Claims

**Description:** Analysis claims information is suppressed without evidence of suppression; confuses "sealed" with "suppression" or "unknown" with "suppression."

**Detection:**
- Claims like "they're hiding X" appear without evidence of hiding
- Absence of public disclosure is treated as evidence of suppression
- No institutional incentive reasoning provided

**Recovery:**
1. For each suppression claim, ask: "What is the evidence of suppression?"
2. If only absence of disclosure: Reclassify as "sealed" or "unknown"
3. If legitimate institutional reason: Acknowledge and reason using institutional incentives
4. If actual suppression (destroyed records, etc.): Provide explicit evidence
5. If none of above: Delete the claim

---

### Failure Mode 4: Privilege of Single Narrative

**Description:** Analysis settles on one hypothesis without presenting alternatives; dismisses competing hypotheses without evidence.

**Detection:**
- Only one hypothesis is presented in detail; others are mentioned but not analyzed
- Alternatives are dismissed as "unlikely" without evidence
- Confidence distribution shows dominance of one hypothesis without justification

**Recovery:**
1. Identify all hypotheses consistent with available evidence
2. For each hypothesis, trace to supporting source tiers
3. Assign Bayesian weights based on source mix
4. Show full confidence distribution
5. For each alternative, explicitly state: "This hypothesis would be more likely if [evidence]"

---

### Failure Mode 5: Institutional Behavior as Conspiracy

**Description:** Normal institutional behavior (security compartmentalization, budget defense, legal caution) is interpreted as conspiracy.

**Detection:**
- Analysis uses language like "deliberately," "intentionally," "cover-up" without evidence of malice
- Institutional incentives are not analyzed
- Normal institutional practice is attributed to conspiracy

**Recovery:**
1. Identify institutional behavior in question
2. List all institutional incentives (security, budget, legal, structural)
3. Does behavior align with incentives? → Explain through incentives, not conspiracy
4. Is there evidence of *intentional deception*? → Provide explicit evidence
5. Use structural secrecy framework instead of conspiracy assumptions

---

## Correction Protocol

### How to Fix Analysis When Errors Are Detected

#### Step 1: Identify the Error
Use the guardrails above to identify which reasoning error occurred:
1. Temporal anchoring failure?
2. Unanchored suppression claim?
3. Missing competing hypothesis?
4. Hedging language?
5. Institutional conspiracy language?
6. Physics constraints not noted?
7. Sealed/Unknown/Conspiracy conflation?

#### Step 2: Locate the Problem
Find all instances of the error in the analysis:
- Search for hedge words (Guardrail 4 error)
- Search for unsupported suppression claims (Guardrail 2 error)
- Check temporal anchoring (Guardrail 1 error)

#### Step 3: Correct the Error
Apply the specific correction procedure from the guardrail section above:
- For temporal drift: Add specific dates
- For unanchored suppression: Remove claim or provide evidence
- For hedge words: Replace with explicit percentages
- For single narrative: Add competing hypotheses
- For conspiracy language: Reason through institutional incentives

#### Step 4: Verify the Fix
Re-run the analysis through all seven guardrails to ensure:
- Temporal anchoring: ✓ All major claims have dates
- No unanchored suppression: ✓ Suppression claims have evidence
- Competing hypotheses: ✓ All credible alternatives presented
- Language precision: ✓ No hedging; explicit confidence
- Institutional context: ✓ Incentives explained, not conspiracy
- Physics/logic constraints: ✓ Violations noted if relevant
- Sealed ≠ Unknown ≠ Conspiracy: ✓ Categories distinguished

#### Step 5: Update Confidence Levels
After correction, may need to adjust confidence distributions:
- If hedging was removed and confidence raised, justify the increase with evidence
- If conspiracy language was corrected, may lower confidence in that hypothesis
- If sealed records reasoning was improved, may update structural secrecy reasoning

---

## Implementation

### In Practice
1. **During Analysis**: Reference the guardrails while building analysis; don't wait for errors
2. **Self-Check**: Run completed analysis through all seven guardrails
3. **Peer Review**: Have others check for reasoning errors using the guardrails
4. **Correction**: If errors found, use the correction protocol above

### Red Flags (Quick Scan)
If your analysis contains any of these, check for the related guardrail failure:
- Hedge words ("may," "might," "could") → Guardrail 4
- Atemporal claims (no dates) → Guardrail 1
- "They're hiding X" without evidence → Guardrail 2
- Only one hypothesis discussed → Guardrail 3
- No institutional incentive reasoning → Guardrail 5
- Physics assumptions not stated → Guardrail 6
- "It's secret, so it's conspiracy" → Guardrail 7

---

## Version & Updates

**Version**: 3.0-alpha
**Last Updated**: 2025-11-17

See CHANGELOG.md for version history.
