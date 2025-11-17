# Five Generic Methodology Examples

## How the Framework Works in Practice

Each example demonstrates the mandatory analysis structure and guardrail verification. These are **hypothetical generic scenarios**, not real incidents.

---

## Example 1: T1/T2 Source Conflict

### Query
"Two sources give different accounts of institutional policy change. One says X, one says Y. How do we weight them?"

### System Response

**Header:**
```
Question: How to resolve conflicting source accounts about institutional policy change?
Entropy Level: L3 (Mixed evidence)
Source Tier Mix: T1: 40%, T2: 60%, T3: 0%, T4: 0%
Analysis Date: 2025-11-17
```

**Verified Facts (T1/T2 Only):**
```
- T1: Official agency statement released [date]: Policy position is [X], confidence: 95%
- T2: Academic research published [year]: Research suggests policy interpretation [Y],
  methodology: peer-reviewed, confidence: 85%
```

**Analysis & Interpretation:**
```
Conflict Identified:
T1 Source (agency statement) claims position X.
T2 Source (peer research) claims policy interpretation Y.

Resolution Using Conflict Hierarchy:
Default hierarchy (T1 > T2) suggests position X is primary, but contradiction is significant.
This may indicate: (1) agency statement is incomplete, (2) researcher interpretation differs from
official position, (3) both are correct in different contexts.

Likely explanation: Agency statement (T1) establishes official position (X).
Research (T2) identifies implementation variation [specific variation], which is technically
consistent with position X but described differently.

Confidence Assessment:
- Confidence in official position X: 92% (T1 source)
- Confidence in implementation variation: 78% (T2 finding; consistent with T1)
- Confidence in complete resolution: 70% (apparent conflict explained)
```

**Competing Hypotheses:**
```
Hypothesis A: Positions X and Y describe different aspects of same policy, 72% confidence
  Supporting: Both T1 and T2 agree on underlying principle; difference is descriptive

Hypothesis B: Agency overstated policy coherence; actual implementation diverges, 20% confidence
  Supporting: T2 research suggests fragmentation not mentioned in T1 statement

Hypothesis C: Researcher misinterpreted policy; T1 is correct, 8% confidence
  Supporting: T1 is direct source; T2 is interpretation
```

**Guardrail Verification:**
```
✓ Temporal Anchoring: Dates specified for both sources
✓ No Unanchored Suppression: No suppression claims (just source conflict)
✓ Competing Hypotheses: Three hypotheses presented with confidence weights
✓ Language Precision: Explicit confidence percentages; no hedging ("may," "might")
✓ Institutional Context: Conflict explained through policy complexity, not conspiracy
✓ Physics/Logic: No physics/logic constraints relevant
✓ Sealed ≠ Unknown ≠ Conspiracy: N/A; both sources are public
```

**Next Steps:**
```
Evidence that would increase confidence in Hypothesis A: Additional T1 sources clarifying
  how both descriptions fit together
Evidence that would increase confidence in Hypothesis B: T2 research showing systematic
  implementation variation across regions/time periods
```

---

## Example 2: Testimony Without Corroboration

### Query
"A named former official provides testimony about historical decision-making. No other sources confirm the details. How do we treat this testimony?"

### System Response

**Header:**
```
Question: How to weight T4_named testimony without direct corroboration from T1/T2?
Entropy Level: L3 (Mixed evidence; testimony-dependent)
Source Tier Mix: T1: 0%, T2: 20%, T3: 0%, T4: 80%
Analysis Date: 2025-11-17
```

**Verified Facts:**
```
- T2: Academic synthesis of declassified documents [year]: General institutional framework,
  confidence: 88%
```

**Analysis & Interpretation:**
```
Testimony Received:
[Named individual]: [Title/credentials], [date of employment]: [testimony about decision-making]

Credibility Assessment:
- Individual credentials: [Professional history], verified
- Potential conflicts of interest: [Institutional affiliations], [Career implications]
- Specificity of testimony: [Specific details suggesting direct knowledge vs. vague claims]
- Consistency with known facts: [Aligns with or contradicts T2 background]

Treatment:
This testimony provides insider perspective on decision-making process. No T1/T2 source directly
contradicts it, but no T1/T2 source directly confirms it either. Testimony stands as isolated
account from credible witness; confidence limited by lack of corroboration.

Confidence: 42% (named credible source, but uncorroborated by T1/T2)
```

**Testimony Attribution:**
```
T4_named: [Individual], [credentials], employed [dates]: [specific testimony quote].
Corroboration status: Uncorroborated by T1/T2; consistent with general [T2 framework].
Confidence: 42%
```

**Next Steps:**
```
Evidence that would increase confidence: (1) Additional named witnesses with consistent
  testimony, (2) T1 declassified document supporting details, (3) T2 research on similar
  decision-making processes confirming plausibility
Evidence that would decrease confidence: (1) T1 source contradicting key detail,
  (2) Evidence of witness bias or misremembering
```

**Guardrail Verification:**
```
✓ Temporal Anchoring: Employment dates and testimony timing specified
✓ No Unanchored Suppression: Testimony not treated as evidence of suppression
✓ Competing Hypotheses: T4 treated as one hypothesis; alternatives identified
✓ Language Precision: Explicit confidence (42%); not "possibly reliable" or "credible"
✓ Institutional Context: Witness bias/incentives analyzed; no conspiracy assumption
✓ Physics/Logic: N/A
✓ Sealed ≠ Unknown ≠ Conspiracy: Testimony not treated as evidence of sealed information
```

---

## Example 3: Physics Constraints in Hypothesis Evaluation

### Query
"A hypothesis about a mechanism violates known physics. Should we eliminate it?"

### System Response

**Header:**
```
Question: How to handle hypotheses that violate known physics?
Entropy Level: L4 (Contested; physics constraints)
Source Tier Mix: T1: 30%, T2: 50%, T3: 20%, T4: 0%
Analysis Date: 2025-11-17
```

**Analysis & Interpretation:**
```
Hypothesis A (Primary): [Mechanism consistent with known physics], supported by [T1/T2]

Hypothesis B (Physics Constraint): [Mechanism appears to violate known physics]
Physics Constraint Analysis:
- Known physics principle: [Specific law or constraint]
- How hypothesis violates it: [Specific mechanism inconsistency]
- Severity: Requires [specific violation of established law]
- Certainty: Physics constraint is well-established; confidence in constraint: 98%

Treatment of Physics-Constrained Hypothesis:
Does NOT eliminate hypothesis, but LOWERS confidence:
- Baseline confidence from evidence: 50%
- Physics constraint reduction: -25% (significant but not complete elimination)
- Adjusted confidence: 25%

Reasoning:
Physics constraints are very strong, but: (1) edge cases exist, (2) known physics is sometimes
revised, (3) apparent violations sometimes reflect our incomplete understanding. Hypothesis
remains credible but at lower confidence.
```

**Competing Hypotheses:**
```
Hypothesis A: [Mechanism consistent with physics], 70% confidence
  Supporting: T1 evidence; T2 research

Hypothesis B: [Mechanism that appears to violate physics], 25% confidence
  Supporting: Some T2 findings; explicitly noted physics violation

Hypothesis C: [Alternative mechanism], 5% confidence
  Supporting: Speculative; resolves physics concern but less supported by evidence
```

**Guardrail Verification:**
```
✓ Guardrail 6 (Physics/Logic Constraints): Physics violation explicitly noted and quantified
  - Violation documented: [Specific constraint]
  - Does NOT eliminate hypothesis; reduces confidence from 50% to 25%
  - Readers understand the physics concern and confidence reduction
```

---

## Example 4: Sealed Records and Institutional Incentives

### Query
"Records about [institutional process] remain classified. Can we reason about their likely content?"

### System Response

**Header:**
```
Question: How to reason about classified records using institutional incentives?
Entropy Level: L4 (Sealed records; reasoning framework)
Source Tier Mix: T1: 35% (adjacent documents), T2: 40%, T3: 25%, T4: 0%
Analysis Date: 2025-11-17
```

**Structural Secrecy Context:**
```
Sealed Records:
[Specific records] remain classified under [classification authority].
Classification status as of [date]: Still classified
Declassification eligible: [Future date if applicable]

Institutional Incentive Analysis:
- Sealing authority: [Institutional agency]
- Institutional mandate: [Specific mission]
- Incentive for classification: [Specific reason: operational security, privacy, etc.]
- This is legitimate classification, not evidence of suppression

Declassification Pattern Reference:
Historical pattern: [Agency] has declassified [similar records] after [timeframe]
Precedent: [Related declassifications] suggest [pattern about likely content]

Reasoning About Sealed Records:
Given institutional mandate and incentive patterns, sealed content likely addresses:
- [Likely topic 1]: XX% confidence (based on incentive)
- [Likely topic 2]: XX% confidence (based on adjacent evidence)
- [Likely topic 3]: XX% confidence (speculative)

Confidence Summary: 50-65% (indirect reasoning; sealed records reasoning inherently uncertain)
```

**Next Steps:**
```
Evidence that would clarify sealed content: (1) Future declassification, (2) Testimony from
  participants, (3) Adjacent T1 documents providing context
Timeline: [Specific records] may become declassifiable [date]
```

**Guardrail Verification:**
```
✓ Guardrail 2 (No Unanchored Suppression): Classification treated as legitimate, not as
  evidence of suppression or conspiracy
✓ Guardrail 7 (Sealed ≠ Unknown ≠ Conspiracy): Sealed records analyzed using institutional
  incentive framework; clear that records exist but are sealed (not "unknown")
```

---

## Example 5: Institutional Incentives vs. Conspiracy Language

### Query
"Why would an institution make [controversial decision]? Was it conspiracy or institutional incentive?"

### System Response

**Header:**
```
Question: Institutional decision-making analysis (incentive-based, not conspiracy-based)
Entropy Level: L3 (Established facts; interpretation contested)
Source Tier Mix: T1: 60%, T2: 30%, T3: 10%, T4: 0%
Analysis Date: 2025-11-17
```

**Verified Facts:**
```
- T1: Official statement [date]: Institution made decision [X], confidence: 95%
- T2: Institutional analysis [year]: Context and precedent, confidence: 88%
```

**Analysis & Interpretation:**
```
Decision Made: [Specific institutional decision]

Alternative Explanations:

Explanation A (Institutional Incentive): The decision aligns with institutional mandate
  - Institutional incentive: [Specific budget, legal, or operational reason]
  - Supporting evidence: [T1/T2 sources showing incentive structure]
  - This explanation does NOT assume malice; just explains behavior through incentives
  - Confidence: 75%

Explanation B (Competing Institutional Incentive): Alternative institutional incentive
  - Institutional incentive: [Different reason]
  - Supporting evidence: [T1/T2 sources]
  - Also does NOT assume conspiracy; just different incentive analysis
  - Confidence: 20%

NOT ENTERTAINED (Conspiracy Without Evidence):
"The institution was engaged in conspiracy" - This assumes malice without evidence.
Do NOT confuse institutional behavior with conspiracy. Institutions act through incentives
and structure, not through hidden conspiracy.
```

**Guardrail Verification:**
```
✓ Guardrail 5 (Institutional Context Without Conspiracy): Decision explained through
  institutional incentives (budget constraints, legal requirements, mandate priorities),
  NOT through conspiracy assumptions
✓ Language Precision: Confidence levels explicit (75%, 20%); no conspiracy hedging
  ("seems like," "possibly hiding")
✓ Competitive Hypotheses: Multiple institutional incentive frameworks presented
```

---

## Common Pattern Across All Examples

Every example demonstrates:

1. **Mandatory Structure Followed**
   - Header with entropy level and source mix
   - Verified facts (T1/T2 only)
   - Analysis separating facts from interpretation
   - Testimony attribution (if applicable)
   - Competing hypotheses with confidence distributions
   - Guardrail verification

2. **Guardrails Applied Systematically**
   - All seven guardrails checked
   - Errors identified and corrected
   - Reasoning transparent and verifiable

3. **Confidence Explicit**
   - No hedging language ("may," "might," "could")
   - All confidence levels are percentages
   - Reasoning for confidence level is stated

4. **Domain-Agnostic Methodology**
   - Same structure applies whether analyzing history, science, policy, or institutions
   - Framework is methodology, not substance

---

## Version & References

**Version**: 1.0
**Last Updated**: 2025-11-17

For full methodology, see docs/framework.md
For guardrail details, see GOVERNANCE.md
For sourcing rules, see SOURCING_PROFILE_V2.1.md
