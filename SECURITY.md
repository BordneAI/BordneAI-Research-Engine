# Security: Responsible Disclosure

## What This Framework Can Do

The BordneAI Research Engine is a specification for evidence-based reasoning. It:
- Analyzes contested questions using structured evidence evaluation
- Applies systematic guardrails to catch reasoning errors
- Distinguishes legitimate sealed records from conspiracy claims
- Weights competing hypotheses using Bayesian reasoning

**This is not a security-critical system** and contains no executable code. It is specification documentation for use in LLM systems.

---

## Potential Misuse Scenarios

### Scenario 1: Using to Support Unanchored Conspiracy Claims
**Potential Misuse:** Someone claims the framework validates a conspiracy theory by "reasoning about sealed records."

**Reality:** The framework explicitly refuses to analyze unanchored conspiracy claims. Sealed records ≠ conspiracy (Guardrail 7). Any analysis supporting an unanchored conspiracy claim violates the framework's core principles and should be treated with skepticism.

**Detection:** Legitimate analysis using the framework will:
- Explicitly state what is sealed vs. what is conspiracy
- Show T1/T2 evidence base
- Present competing hypotheses with confidence levels
- Apply all seven guardrails

### Scenario 2: Using to Bypass Institutional Oversight
**Potential Misuse:** Someone uses the framework to rationalize institutional secrecy or justify suppression.

**Reality:** The framework is designed to enable **accountability** by reasoning about sealed records. It:
- Requires explicit evidence for suppression claims
- Distinguishes legitimate sealing from conspiracy
- Asks what institutional incentives justify secaling
- Encourages declassification pattern analysis

Using the framework to justify suppression would violate its core purpose.

### Scenario 3: Using to Fabricate False Confidence
**Potential Misuse:** Someone uses the framework's language of confidence levels to make unfounded claims sound rigorous.

**Reality:** The framework requires explicit source tier basis for confidence levels. Claims without T1/T2 evidence are either:
- Explicitly assigned low confidence (L4-L5)
- Refused as analysis (pure speculation)

Any analysis claiming high confidence without T1/T2 evidence violates the framework.

---

## Responsible Disclosure

If you identify potential misuse of the framework, or discover that someone is using the framework to support unanchored claims while falsely claiming framework legitimacy:

### Report Procedure
1. **Document the misuse**: Record the specific claim and how it violates the framework
2. **Identify the violation**: Which guardrail is violated? What T1/T2 evidence is missing?
3. **Contact**: See CONTRIBUTING.md for how to report framework issues
4. **Include**: Specific location of misuse and analysis of the framework violation

### What Constitutes Reportable Misuse
- Using framework output to support unanchored suppression claims
- Claiming framework authority for analysis that violates guardrails
- Misrepresenting sealed records as equivalent to conspiracy
- Using framework language to fabricate false confidence in speculation
- Claiming framework validation for analysis that lacks T1/T2 evidence base

### What Does Not Constitute Reportable Misuse
- Disagreement with analysis conclusion (substantive disagreement is fine)
- Use of framework for domains not recommended (user responsibility)
- Analysis that's wrong but honest (errors happen; correction is through CONTRIBUTING.md)
- Competitive or alternative frameworks (disagreement on methodology is fine)

---

## Framework Vulnerabilities (Inherent Limitations)

The framework has known limitations that users should understand:

### 1. Garbage In, Garbage Out
If sources are misclassified (calling a T4 testimony "T1 evidence"), analysis will be wrong.

**Mitigation**: Verify source tier assignments yourself. Don't blindly trust T1/T2 designations.

### 2. Hypothesis Incompleteness
The analysis is only as good as the hypotheses identified. If a credible hypothesis is missed, it won't appear in the output.

**Mitigation**: Generate your own hypotheses; don't rely solely on the framework's identification.

### 3. Guardrail Application Variance
Human implementation of the guardrails may be inconsistent. One analysis might catch an error; another might not.

**Mitigation**: Review analyses against all seven guardrails yourself. Verify guardrail compliance.

### 4. Sealed Records Reasoning Limitations
Even with institutional incentive reasoning, inferences about sealed records have inherently lower confidence (typically 30-50%).

**Mitigation**: Don't treat sealed-record inferences as if they were direct evidence. Acknowledge the indirectness.

### 5. Confidence Level Calibration
The framework provides explicit confidence levels, but these are only as good as the evidence evaluation.

**Mitigation**: Verify that confidence levels match the evidence base. Question if confidence seems too high for the evidence provided.

---

## Ethical Use Guidelines

### Do:
- Use the framework to reason rigorously about contested questions
- Distinguish sealed records (legitimate) from conspiracy claims (unanchored)
- Apply guardrails to catch your own reasoning errors
- Acknowledge evidence limitations and uncertainty
- Report misuse or framework violations

### Don't:
- Use the framework to support unanchored suppression claims
- Claim the framework validates conspiracy theories
- Ignore guardrail violations in analyses you encounter
- Use framework output as sole basis for high-stakes decisions
- Treat sealed record inferences as direct evidence

---

## Contact

For security concerns or responsible disclosure of potential misuse:

1. **Document the issue clearly**: Describe what misuse occurred
2. **Identify the framework violation**: How does it violate guardrails or misrepresent the framework?
3. **Report through CONTRIBUTING.md**: Follow the error reporting process

Do not publicly disclose potential misuse before allowing the maintainers opportunity to respond. Responsible disclosure protects the framework's integrity.

---

**BordneAI Research Engine v3.0-alpha**
Specification for evidence-based reasoning. Released under CC BY 4.0.
