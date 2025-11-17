# Structural Secrecy: Reasoning About Sealed Records

## Framework for Analyzing What We Don't Know

---

## What is Structural Secrecy?

**Definition:** The deliberate withholding of information by legitimate authorities to serve specified institutional purposes, governed by law, regulation, or policy.

Structural secrecy is **not** conspiracy. It is a system of **legitimate** information compartmentalization.

### Why Seal Information?

Legitimate reasons for information sealing include:

| Reason | Example | Institutional Purpose |
|---|---|---|
| **Operational Security** | Ongoing investigation details | Prevent interference with active operations |
| **Personnel Privacy** | Personnel records, medical histories | Comply with privacy law (HIPAA, GDPR, etc.) |
| **National Security** | Classified military operations | Prevent disclosure to foreign adversaries |
| **Proprietary Information** | Trade secrets, patent details | Protect commercial competitive advantage |
| **Legal Privilege** | Attorney-client communications, deliberative process | Preserve legal functioning |
| **Diplomatic Sensitivity** | Foreign agent identities, allied relationships | Protect international relationships |
| **Compartmentalization** | "Need to know" classified information | Control who has access to sensitive information |

All of these are **legitimate** reasons for sealing information. The fact that information is sealed does **not** indicate conspiracy.

### Key Principle: Sealed ≠ Unknown ≠ Conspiracy

These are three distinct categories with different handling:

| Category | Definition | Characteristics | Handling |
|---|---|---|---|
| **Sealed** | Legitimately withheld by authority | Has legal basis; likely declassifiable; reasoning possible | Use structural secrecy framework |
| **Unknown** | We lack information; no evidence of sealing | Natural gap; may close through research | Acknowledge gap; identify what would resolve it |
| **Conspiracy** | Illegitimate suppression despite obligation | Requires explicit suppression evidence | Refuse to analyze; require evidence first |

---

## The Three Categories: How to Distinguish Them

### Sealed Records

**Recognition:** Information is classified, sealed by law, or protected by regulation.

**Evidence of Sealing:**
- Explicit classification markings ([CLASSIFIED], [REDACTED], etc.)
- FOIA exemptions (national security, privacy, deliberative process)
- Legal protection (attorney-client privilege, medical privacy)
- Official statements refusing to disclose ("This is classified for reasons of...")

**Handling:**
- Accept that information is sealed
- Do NOT assume it doesn't exist
- DO reason about likely content using institutional incentive reasoning
- DO reference declassification patterns
- DO acknowledge that future declassification will add evidence

**Example Framing:**
```
This information is classified. The classification serves [legitimate purpose].
The document was likely created around [inference based on adjacent events].
Given [institutional incentive], the content likely addresses [inference].
Confidence: XX% because [reasoning is indirect].
```

### Unknown Information

**Recognition:** We lack information; there is no evidence that it was deliberately withheld.

**Characteristics:**
- No explicit evidence of sealing
- Information was never gathered, discovered, or made public
- Gap is natural; not evidence of suppression
- Future research might discover it

**Handling:**
- Acknowledge the gap explicitly
- Do NOT assume suppression
- DO identify what evidence would resolve the gap
- DO continue analysis without the unknown information
- DO note uncertainty caused by unknown information

**Example Framing:**
```
We lack information about [X]. This is not evidence of suppression; rather, [specific reason for gap]:
- The information may not have been gathered
- The question may not have been studied
- Access may be limited for legitimate reasons

If [specific evidence] became available, analysis would shift toward [hypothesis].
```

### Conspiracy (Illegitimate Suppression)

**Recognition:** Claim that information is being suppressed illegitimately despite an obligation to disclose.

**Required Evidence:**
- Explicit evidence of suppression (destroyed records, denied FOIA, legal violation)
- Documented obligation to disclose (law, regulation, contract)
- Failure to disclose despite obligation

**Handling:**
- Do NOT analyze pure conspiracy claims without evidence
- DO require explicit suppression evidence before treating as possible
- DO distinguish from legitimate sealing
- DO refuse analysis if evidence is absent

**Example Refusal:**
```
This claim assumes illegitimate suppression. However, there is no evidence of suppression—only
absence of public disclosure. The absence of public disclosure is consistent with legitimate
classification, not conspiracy. Analysis is refused until explicit evidence of suppression is provided.
```

---

## Institutional Incentives Framework

How to reason about what sealed records likely contain:

### Step 1: Identify the Sealing Authority
- Who sealed the information? (Government agency? Court? Company?)
- What authority do they have? (Law? Regulation? Policy?)
- What is their mandate? (National security? Privacy protection? Business interest?)

### Step 2: Infer Institutional Incentives
Given the sealing authority and their mandate, what incentives drive the sealing decision?

**Example Incentive Analysis:**
```
Authority: National security agency
Mandate: Protect against foreign intelligence threats
Incentive: Seal operational details to prevent adversary interference
Inference: Sealed content likely addresses [specific operational concern]
Confidence: Medium (incentive is clear, but specific content is speculative)
```

### Step 3: Identify Declassification Patterns
Historical patterns show:
- What kinds of information do agencies typically declassify?
- After how long (30 years, 50 years, never)?
- What triggers declassification (FOIA request, statute of limitations, historical release)?

**Example Pattern Analysis:**
```
Historical pattern: [Agency] declassifies operational records after 25-30 years
Current status: Records from [period] became eligible for declassification in [year]
Inference: [Current year - 30 years] documents may be available; earlier documents less likely
Confidence: High (based on documented agency practice)
```

### Step 4: Reason About Adjacent Evidence
What T1/T2 evidence exists in nearby areas that might illuminate sealed information?

**Example Adjacent Evidence:**
```
Sealed records: [Program details]
Adjacent evidence: Declassified documents from [related program] show [specific detail]
Inference: If [related program] operated on principle X, sealed program likely did too
Confidence: Medium (similar programs often have similar structures, but not always)
```

### Step 5: Quantify Uncertainty
How confident can you be about sealed record content?

**Confidence Ranges for Sealed Record Reasoning:**
- **High confidence (70-85%)**: Multiple incentive lines and adjacent evidence agree
- **Medium confidence (50-70%)**: Incentive reasoning is clear; adjacent evidence supports inference
- **Low confidence (30-50%)**: Incentive reasoning is plausible; weak adjacent evidence
- **Very low confidence (<30%)**: Incentive reasoning is speculative; little corroboration

**Rule:** Never assign high confidence to sealed record inferences; evidence is indirect by definition.

---

## Don't Know vs. Unknown vs. Speculation

### Three Different Situations

#### Situation 1: Don't Know (We Tried; Information is Sealed)
**What happened:** You searched for evidence; information exists but is sealed by legitimate authority.

**Characteristics:**
- Explicit evidence of sealing (classification markings, FOIA denials, etc.)
- Authority is legitimate (government agency, court, company with legal right)
- Information likely exists but is not accessible
- May be declassified in future

**Handling:**
- Use structural secrecy framework
- Reason about likely content using institutional incentives
- Acknowledge you're reasoning about sealed records
- Assign confidence proportional to indirectness of evidence

**Example:**
```
Information about [X] is classified. Reasoning about likely content: [inference based on incentives].
Confidence: 55% (reasoning is indirect; sealed record inference inherently uncertain).
```

#### Situation 2: Unknown (Information Was Not Gathered or Made Public)
**What happened:** You searched for evidence; information doesn't exist in public or documented form.

**Characteristics:**
- No evidence of deliberate sealing
- Information was simply not gathered, studied, or published
- Gap is natural; many things are not studied
- Future research might discover it

**Handling:**
- Acknowledge the gap explicitly
- Do NOT assume suppression
- Identify what evidence would resolve the gap
- Continue analysis without assuming what's in the gap

**Example:**
```
We lack documented evidence about [X]. This is not evidence of suppression; rather, the question
has not been studied in the available literature. If [specific research] were conducted, we would
have evidence about [Y].
```

#### Situation 3: Speculation (No Evidence of Existence or Sealing)
**What happened:** You have no evidence that information exists; you're guessing what might be true.

**Characteristics:**
- No evidence the information exists
- No evidence the information is sealed
- You're inventing possibilities without evidence anchoring
- This is pure speculation

**Handling:**
- REFUSE to analyze
- Explain why (no T1/T2 evidence; pure speculation)
- Offer to reframe to analyzable question if possible

**Example:**
```
This question requires speculation about information with no evidence base. Analysis is refused.
If you can provide evidence that [information] exists or was sealed, I can analyze using the
structural secrecy framework. Otherwise, the question lacks evidential grounding.
```

---

## Refusal Protocol for Speculation

When to refuse analysis:

### Refuse If:
1. **No T1/T2 Evidence Base**: Question requires inventing facts without documentation
2. **Unanchored Suppression Claim**: Claims information is suppressed without evidence of suppression
3. **Pure Invention**: No evidence the question addresses real phenomena

### Standard Refusal Response:
```
This question cannot be analyzed because [specific reason]:
- Requires speculation without T1/T2 evidence base
- Assumes suppression without evidence of suppression
- Invents facts not documented in available sources

The framework does not analyze pure speculation. If you can provide:
[Type of evidence] that would anchor the question, analysis becomes possible.

Alternatively, the reframed question [modified question] is analyzable because [reason].
```

### Offering a Reframe:
Often, refusal can be converted to analyzable analysis through reframing:

**Original (Speculative):** "What did [sealed program] do?"
**Refusal Reason:** "Program details are sealed; no adjacent evidence available to infer content"
**Reframed:** "Given institutional incentives and declassification patterns from similar programs, what operational structure would be consistent?"

**Original:** "Is the organization hiding evidence of X?"
**Refusal Reason:** "Unanchored suppression claim; no evidence of suppression"
**Reframed:** "What institutional incentives explain why information about X is not publicly disclosed?"

---

## Quantifying Uncertainty About Sealed Records

### The Challenge
When records are sealed, confidence is inherently limited because reasoning is **indirect**:
- You don't have direct evidence
- You're inferring from incentives and adjacent information
- Sealed content might contradict your reasoning

### Confidence Reduction
Apply systematic reductions to confidence based on:

**Base Confidence (if fully documented):** 85%
**Sealed Record Reductions:**
- Information is sealed (not directly accessible): -20% → 65%
- Reasoning relies on incentive inference: -15% → 50%
- Adjacent evidence is ambiguous: -10% → 40%
- Multiple interpretations of incentives exist: -15% → 25%

### Result: Sealed Record Confidence Range
- **High inference confidence (70-80%)**: Multiple independent lines of reasoning agree; adjacent evidence corroborates
- **Medium confidence (50-70%)**: Incentive reasoning is clear; some corroboration
- **Low confidence (30-50%)**: Reasoning is plausible but has gaps; weak corroboration
- **Very low confidence (<30%)**: Reasoning is speculative; little corroboration

**Never claim high confidence about sealed records.** Direct evidence gives higher confidence.

---

## Generic Hypothetical Examples

### Example 1: Sealed Operational Records
**Scenario:** An agency conducted an operation. Details remain classified.

**Analysis:**
```
Operation [X] was conducted from [date] to [date]. Details remain classified under [classification authority].

Institutional context:
- Agency mandate: [Specific mission]
- Likely incentive for classification: [Operational security reason]
- Classification likely lifts: [Future date based on historical patterns]

Adjacent evidence:
- [Declassified document Y] describes similar operation from earlier period
- Structure suggests [operational pattern]

Inference about sealed operation:
- Likely operational scope: [Based on adjacent evidence], XX% confidence
- Likely institutional purposes: [Based on agency mandate], XX% confidence
- Likely timeline: [Based on adjacent events], XX% confidence

Confidence Summary:
These inferences are indirect (based on reasoning about sealed records). Confidence: 40-55%.
Future declassification will provide direct evidence.
```

### Example 2: Unknown but Not Sealed
**Scenario:** A question about a phenomenon with no public research.

**Analysis:**
```
We lack documented evidence about [phenomenon X].

Why knowledge gap exists:
- The phenomenon has not been widely studied (no funded research program)
- Research may exist but is not in peer-reviewed literature
- The question is new (emerging interest)

What would resolve the gap:
- Peer-reviewed research study of [phenomenon]
- Systematic data collection on [specific measurement]
- [Type of] documentation from participants

Current confidence: Unable to assess hypotheses; insufficient evidence base.
```

### Example 3: Sealed Records with Clear Incentive
**Scenario:** Government protects identity of intelligence operatives (legitimate secrecy).

**Analysis:**
```
Intelligence operative identities remain classified indefinitely.

Institutional context:
- Agency: Intelligence service
- Mandate: Conduct intelligence operations and protect operatives
- Incentive for classification: Operative safety (personal security threat if identity exposed)

Conclusion:
Classification is legitimate. Identities will remain sealed indefinitely (not subject to
standard declassification timelines). Reasoning about sealed identities is not possible
without independent evidence about specific individuals.

Analysis refused: Cannot reason about classified operative identities without independent evidence.
```

---

## Practice: Distinguishing Categories

### Test Yourself: Which Category?

**Scenario 1:** "What is the content of classified government documents from 1965?"
- Sealed (legitimate classification) / Unknown (not studied) / Conspiracy (illegitimate suppression)?
- **Answer:** Sealed. Classification is explicit and legitimate. Reasoning possible using institutional incentives.

**Scenario 2:** "What percentage of [population] experienced [phenomenon]? No published research exists."
- Sealed / Unknown / Conspiracy?
- **Answer:** Unknown. Not deliberately sealed; simply not researched. Gap is natural, not evidence of suppression.

**Scenario 3:** "Is organization X hiding evidence of wrongdoing?"
- Sealed / Unknown / Conspiracy?
- **Answer:** Conspiracy (without evidence). Unless you have explicit evidence of suppression (destroyed records, denied FOIA, etc.), this is speculation. Refusal appropriate.

**Scenario 4:** "Personnel records of employees are not public. Why?"
- Sealed / Unknown / Conspiracy?
- **Answer:** Sealed. Legal requirement (privacy law). Legitimate sealing, not suppression or conspiracy.

---

## Version & References

**Version**: 1.0
**Last Updated**: 2025-11-17

For guardrails on suppression claims, see GOVERNANCE.md (Guardrail 2).
For reasoning about sealed institutional behavior, see docs/examples.md.
