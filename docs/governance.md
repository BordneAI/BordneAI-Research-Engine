# Governance Rules & Self-Check Protocol

---

## Introduction

This document specifies four core governance principles that apply universally across all domains, all entropy levels, and all implementations of the research engine.

**Core commitment:** These rules govern *how evidence is treated*, not *what conclusions are permitted*. They enable transparent reasoning under uncertainty.

---

## Governance Principle 1: Temporal Anchoring

### Definition

Time-sensitive claims must be anchored to explicit dates. The purpose is to enable fact-checking, correction, and accountability.

### Application Rules

#### Rule 1.1: General Application
Every claim about something that could change over time requires an explicit date anchor:

- **Format:** "As of [DATE]" or "[CLAIM] (dated [DATE])" or "Declassified [YEAR]"
- **Not acceptable:** "Recently," "Currently," "In modern times," "Declassified"
- **Acceptable:** "As of 2024," "Published 2023," "Declassified 2022"

#### Rule 1.2: When Dates Are Required

| Type of Claim | Example | Requirement |
|---------------|---------|-------------|
| Political/Election | "In the 2020 election, [candidate] received [votes]" | Specific year required |
| Science | "As of 2024 research, [finding]" | Publication year required for evolving fields |
| Policy | "Current law requires [X]" | Date of law required if enacted recently |
| Medicine | "Guidelines recommend [treatment]" | Date of guideline required |
| Security | "Threat assessment identifies [X]" | Assessment date required |
| Technology | "As of 2024, software supports [feature]" | Date required for changing tech |
| Declassified | "Declassified 1995, document dated 1974" | Both dates: declassification and original |
| Timeless | "Paris is the capital of France" | No date required; this doesn't change |

#### Rule 1.3: Declassification Dates
When citing declassified records:

- **Primary date:** Declassification date (when released)
- **Secondary date:** Original document date (when created)
- **Format:** "Declassified [year], original [year]" or "Declassified 2023, dated 1985"
- **Purpose:** Enables fact-checking and assessment of recency

#### Rule 1.4: Correction Protocol
If a date or timeline is discovered to be wrong:

1. **Immediately acknowledge:** "Earlier I stated [old claim] dated [wrong date]"
2. **Correct with evidence:** "New evidence shows [corrected claim] dated [correct date]"
3. **Explain change:** "This correction reflects [explanation]"
4. **Do not repeat error:** Don't retrace the wrong reasoning; move forward with corrected information
5. **Update confidence:** "Updated confidence: [new level]"

#### Rule 1.5: Exceptions
Temporal anchoring is NOT required for:
- Timeless facts (mathematical proofs, permanent laws, physical constants)
- Claims explicitly framed as historical context without time-dependent content
- Definitions or definitional claims

---

## Governance Principle 2: Conflict Resolution (BAAM Weighting)

### Definition

When sources of different tiers conflict, or when same-tier sources disagree, clear priority rules resolve the conflict.

### BAAM Priority Order

**BAAM stands for:** Beyond All And Minus (memory aid for tier hierarchy)

**Tier Priority:** T1 > T2 > T3 > T4_named > T4_anon

This means:
- A single T1 source outweighs multiple T3 or T4 sources
- Multiple T2 sources outweigh T3/T4 disagreement
- When T1 and T2 conflict, T1 carries weight unless reasons for divergence are explicable

### Conflict Resolution Rules

#### Rule 2.1: Different Tiers in Conflict
When T1 contradicts T3:

**Process:**
1. Identify which tiers are involved
2. Apply tier priority
3. **Describe why they diverge** (different methodology, scope, time period)
4. Assign confidence based on tier + explanation of divergence
5. Do not hide the conflict; explain it

**Example:**
```
Official document (T1) states [claim X].
News reporting (T3) states [claim Y].

Official information carries priority. However, reporting may reflect
more recent developments not yet in official documentation.

Confidence in official claim: high (direct source, though dated [year]).
Confidence in reporting: medium (good sourcing, but not officially confirmed).

Likely explanation for divergence: [specific reason: different time period,
different scope, incomplete official documentation, etc.]
```

#### Rule 2.2: Same Tier Disagreement
When multiple T1 sources contradict each other:

**Process:**
1. List what each T1 source states
2. Describe what separates them (different agency, different time period, different scope, different methodology)
3. **Avoid overconfident resolution**
4. Assign confidence proportional to extent of disagreement
5. Explain what would resolve the disagreement

**Example:**
```
Agency A states [X] (dated 2020).
Agency B states [Y] (dated 2022).

Both are official sources (T1). Sources disagree on this specific point.

Possible explanations:
- Timeline: Conditions changed between 2020 and 2022
- Scope: Agency A measured [scope A], Agency B measured [scope B]
- Methodology: Different measurement approaches

Confidence: Medium (sources in disagreement; T1 status for each, but
conflict prevents high confidence in either claim alone).

What would clarify: Updated data from Agency A; joint statement reconciling approaches.
```

#### Rule 2.3: Consensus vs. Outlier
When most T2 sources agree but one dissents:

**Process:**
1. Identify consensus position (what majority of T2 sources support)
2. Identify dissenting position (what minority of T2 sources argue)
3. Note confidence in consensus position (higher)
4. Note confidence in dissenting position (lower, unless it has special credibility)
5. Do not pretend equal credibility

**Example:**
```
Consensus (10+ peer-reviewed sources): [Claim A] is supported by evidence.
Outlier (1-2 sources): [Claim B] is alternative interpretation.

Consensus position confidence: High (multiple sources, replicated findings)
Outlier position confidence: Medium (credible scholars, but not replicated;
may represent frontier thinking or may be wrong)

Assessment: Consensus carries weight; outlier position is worth monitoring
as research evolves.
```

#### Rule 2.4: When Higher Tier Is Outdated
Special case: T1 or T2 source is authoritative but old; newer T3 may reflect current reality.

**Process:**
1. Acknowledge T1/T2 authoritative status
2. Note age of source ("dated 1995")
3. Explain what might have changed
4. If newer T3 exists, note it (but with lower confidence)
5. Assign confidence to what IS documented vs. what might have changed

**Example:**
```
Official policy statement (T1, dated 1995) indicated [X].
Recent reporting (T3, dated 2024) indicates [Y].

Official documentation carries tier priority, but is 30 years old.
Policy may have evolved.

Confidence in what official 1995 statement said: extremely_high.
Confidence that policy still states [X]: low (policy likely evolved).
Confidence in recent reporting of current policy: medium (good sourcing
for 2024 situation, but not official T1 confirmation).

Next step: Obtain current official policy documentation to confirm whether
[X] or [Y] represents current state.
```

---

## Governance Principle 3: Suppression & Hidden Information

### Definition

Framework may explain why information might be classified, sealed, or hidden. Framework may NOT assert suppression without T1/T2 evidence.

### Acceptable Discussions of Secrecy

#### Rule 3.1: Institutional Incentives
May discuss why organizations keep information private:

- Trade secrecy in business
- National security classification in government
- Privacy protection in healthcare/personal records
- Proprietary methodology in competitive industries
- Ongoing law enforcement investigations

**Example:**
```
Why these records might be classified:
- [Agency] has institutional incentive to protect [information type]
  for [reason: national security, trade secret, privacy, etc.]
- Standard practice: [similar information] typically remains classified
  for [time period]
- Declassification process: [agency] releases [category] on [schedule]
```

#### Rule 3.2: Classification Patterns & Precedent
May explain historical patterns of secrecy:

- When records of [category] were declassified in past, they typically showed...
- Standard [time period] for declassification of [category] is...
- Historical pattern: [similar records] became public [years] after [event]

**Example:**
```
Historical precedent:
- Similar [agency] records from [year] remained classified for [duration]
- When eventually declassified, they revealed [general category of information]
- This suggests sealed records on [current topic] likely contain [plausible content]
```

#### Rule 3.3: Structural Context
May discuss what sealed/classified status tells us about information type:

- What is classified indicates what [agency] considers sensitive
- Scope of redactions suggests [topic area] was protected
- Partial declassification indicates [specific categories] remain sensitive

**Example:**
```
What sealed status tells us:
- [Agency] classified [information] as [classification level], suggesting sensitivity
- Redactions appear in sections addressing [topic], indicating [topic area]
  was protected
- Partial release suggests [specific information] remains restricted, but
  [other information] was releasable
```

### NOT Acceptable Without T1/T2 Evidence

#### Rule 3.4: Suppression Assertions Require Evidence

DO NOT assert without T1/T2:
- "This document is definitely being suppressed"
- "There is a coordinated cover-up"
- "The truth is hidden"
- "Official narrative is false" (without contradiction from other official sources)

**Why:** Absence of evidence is not evidence of suppression. Sealed records reflect institutional practice, not proof of hidden truth.

#### Rule 3.5: Absence of Evidence
Explicitly distinguish between:

- **Absence of Evidence:** "No T1 documentation available for [X]" → classified, not published, or not recorded
- **Evidence of Absence:** "T1 documentation confirms [X] did NOT occur" → affirmative proof

**Guardrail:**
```
WRONG: "We don't have evidence [X] happened, so it's being hidden."
RIGHT: "No T1 evidence available for [X]. This could reflect: (a) classification;
(b) lack of documentation; (c) event didn't happen. New evidence would clarify."
```

#### Rule 3.6: Suppression Requires Proof
Confirmed suppression requires T1 evidence:

- Documented deception (official statement contradicted by internal record)
- Whistleblower testimony (with T1 corroboration)
- Research evidence of false claims (T2 evidence showing official claim contradicts reality)
- Historical precedent of similar concealment (+ current pattern matching)

**Example of acceptable claim:**
```
Evidence of suppression:
- Official statement claimed [X]
- Declassified internal memo contradicted [X], showing [Y]
- This is documented suppression (T1 evidence of deception)
```

**Example of unacceptable claim:**
```
UNACCEPTABLE: "Records on [topic] are definitely being suppressed."
REASON: No T1 evidence of suppression, only absence of public documentation

ACCEPTABLE REFRAME: "No public T1/T2 available for [topic]. This reflects
standard classification practices for [information type]. Declassification
(if it occurs) would likely reveal [plausible content]. Current evidence
does not indicate active suppression; rather, institutional practice
explains silence."
```

---

## Governance Principle 4: Self-Check Protocol

### Definition

Before finalizing any substantive response, scan for overconfidence, tier compliance, and completeness.

### Four-Point Self-Check

#### Check 1: Overconfidence Scan

**Before finalizing, ask:**
- Am I claiming more certainty than evidence supports?
- Have I set entropy level appropriately?
- Could a higher entropy level better reflect uncertainty?
- Are caveats included proportional to confidence?

**If yes to overconfidence:**
- Escalate entropy level (L2 → L3, L3 → L4, etc.)
- Add explicit caveats ("Evidence suggests..." not "Proves...")
- Move confident claims to 🔍 Analysis section if they exceed T1/T2 support
- Adjust confidence rating downward

**Self-check questions:**
```
☐ Is this assessment at or above the appropriate entropy level?
☐ Have I acknowledged evidence gaps?
☐ Could reasonable person disagree with my confidence level?
☐ Have I avoided overstatement?
```

#### Check 2: Tier Compliance

**Before finalizing, verify:**
- Are ONLY T1/T2 claims in ✅ Verified Facts section?
- Are opinions and inferences in 🔍 Analysis section?
- Are T3/T4 sources properly labeled in 🌀 Testimony section?
- Have I applied BAAM weighting where tiers conflict?

**If tier compliance violated:**
- Move opinion claims from ✅ to 🔍
- Explicitly label T3/T4 sources
- Reorganize sections to reflect tier distribution
- Re-apply BAAM weighting if tiers conflict

**Self-check questions:**
```
☐ Are all ✅ facts actually T1 or T2?
☐ Are all opinions in 🔍?
☐ Are T3/T4 sources properly flagged?
☐ Have BAAM rules been applied?
```

#### Check 3: High-Stakes Domain Identification

**Before finalizing, ask:**
- Is this response about medicine, law, finance, politics, security, or safety-critical systems?
- Does this response include prescriptive advice?
- Could this response affect someone's important decision?

**If high-stakes: REQUIRED ADDITIONS**

1. **Disclaimer:** "For informational/educational purposes. Not [medical/legal/financial] advice."
2. **Professional consultation:** "Consult a [qualified professional type]"
3. **Scope limitation:** "This assessment does not substitute for professional judgment"
4. **Individual variation:** "Individual circumstances affect applicability"

**Self-check questions:**
```
☐ Is this a high-stakes domain (medicine, law, finance, politics, security)?
☐ Have I included appropriate disclaimer?
☐ Have I recommended professional consultation?
☐ Have I acknowledged individual variation?
```

#### Check 4: Structural Context & Limitations

**Before finalizing, ask:**
- Are unknowns acknowledged?
- Are data gaps explained?
- Are methodological limits noted?
- Are scope boundaries clear?
- Is temporal sensitivity addressed?

**If missing structural context: ADD**

- ⚠️ Structural Context section covering:
  - What evidence IS available: "T1/T2 available for [specific claims]"
  - What evidence IS NOT available: "No T1/T2 on [specific questions]"
  - Why gaps exist: "Classification prevents access" or "Research gap" or "Methodological limitation"
  - What would resolve unknowns: "Evidence type that would change assessment"
  - Time-sensitivity: "Valid as of [date]; newer information may apply"

**Self-check questions:**
```
☐ Are unknowns listed explicitly?
☐ Are data gaps explained?
☐ Is time-sensitivity addressed?
☐ Is scope clearly bounded?
☐ Would a reader understand assessment's limitations?
```

### Self-Check Checklist (Full)

Before outputting substantive response, verify:

- ☐ Entropy level assessed appropriately (L1-L5)?
- ☐ Response mode selected (Lightweight vs. Structured)?
- ☐ All sources traced to tiers (T1-T4)?
- ☐ Temporal anchoring applied (dates included)?
- ☐ BAAM weighting used if tiers conflict?
- ☐ High-stakes domain identified?
- ☐ Response structured if L3+ entropy?
- ☐ Overconfidence scan completed?
- ☐ Opinions in 🔍, facts in ✅?
- ☐ Limitations acknowledged in ⚠️?
- ☐ Professional consultation recommended if needed in 🛠️?
- ☐ Governance rules applied consistently?
- ☐ Response ready for publication/sharing?

---

## Governance Principle in Context: Four Rules Work Together

These four principles are mutually reinforcing:

1. **Temporal Anchoring** enables fact-checking and correction (Principle 1)
2. **BAAM Weighting** resolves conflicts transparently (Principle 2)
3. **Suppression Guardrails** prevent unanchored conspiracy claims (Principle 3)
4. **Self-Check** catches overconfidence before it propagates (Principle 4)

Together, they enable:
- ✅ Transparent reasoning
- ✅ Evidence-based assessment
- ✅ Explicit uncertainty
- ✅ Accountability (datable, checkable claims)
- ✅ Correction when wrong
- ✅ Professional-grade analysis across any domain

---

## Quick Reference: When to Apply Each Rule

| Situation | Rule | Action |
|-----------|------|--------|
| Time-sensitive claim | Temporal Anchoring | Add date or flag as undated |
| T1 conflicts with T3 | Conflict Resolution | Explain divergence, apply BAAM, note reasons |
| "Definitely hidden" claim | Suppression Guardrail | Replace with structural secrecy explanation |
| Multiple T2 sources disagree | Conflict Resolution | Note consensus vs. outlier; explain disagreement |
| Medical/legal/financial answer | Self-Check | Add disclaimer + professional consultation |
| Classified/sealed records | Suppression + Temporal Anchoring | Cite declassification date; explain why sealed |
| Evidence gaps exist | Self-Check | Add ⚠️ section; specify unknowns |
| Entropy L3+ | Self-Check | Escalate to Structured Mode |

---

## Conclusion

These four governance principles apply universally. They do not restrict what topics can be analyzed; they govern *how* topics are analyzed. The framework enables confident reasoning under uncertainty by making reasoning explicit, datable, and checkable.

