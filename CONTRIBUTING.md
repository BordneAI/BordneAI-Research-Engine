# Contributing: Error Reporting & Feedback

## Overview

The BordneAI Research Engine v3.0 is a specification for evidence-based reasoning. This is **not traditional open-source software**; it does not accept code contributions via pull requests. However, we welcome feedback on:

- **Specification errors**: Inconsistencies, unclear language, logical gaps
- **Guardrail improvements**: Suggestions for additional or refined guardrails
- **Governance feedback**: Ideas for improving the framework
- **Documentation clarity**: Confusing explanations or missing examples
- **Misuse reports**: See SECURITY.md for responsible disclosure

---

## How to Report Errors

### Step 1: Identify the Error

Clearly describe what is wrong:
- **Location**: Which file and section?
- **Error type**: Is it a typo, logical error, inconsistency, or unclear language?
- **Description**: What is the error and why is it a problem?
- **Impact**: Does this affect: (a) the framework's integrity, (b) practical application, or (c) clarity?

### Step 2: Provide Context

Help us understand the error:
- **The text as written**: Include exact quote
- **What it should be**: What is the correct version?
- **Why it's wrong**: Explain the problem
- **Reference**: Does this error appear elsewhere in the documentation?

### Step 3: Submit the Report

Create a document with the following format:

```
ERROR REPORT
============
File: [filename]
Location: [section/line number if applicable]
Severity: [Critical / High / Medium / Low]

Error Description:
[Clear description of what's wrong]

Current Text:
"[Quote the problematic text]"

Suggested Fix:
[What should it say instead?]

Reasoning:
[Why this matters; impact on framework integrity or clarity]

References:
[Links to related sections or examples]

---
Reporter: [Your name/identifier]
Date: [Date of report]
```

### Step 4: Submit Through Appropriate Channel

Since this is specification documentation:
- **Documentation errors**: Include in issue report
- **Guardrail improvements**: Include in governance feedback section
- **Security/misuse concerns**: See SECURITY.md for responsible disclosure process

---

## Types of Errors We Address

### 1. Logical Inconsistencies
**Example**: "Guardrail A says X, but Guardrail B implies not-X"

**We address this because**: Framework integrity requires internal consistency.

**How to report**: Show which sections contradict each other; explain the logical problem.

### 2. Unclear Language
**Example**: "A key term is defined inconsistently across documents"

**We address this because**: Users need clear, unambiguous definitions.

**How to report**: Quote the unclear passages; explain what's ambiguous; suggest clearer language.

### 3. Missing Examples
**Example**: "Guardrail X is explained but has no concrete example"

**We address this because**: Examples improve understanding and implementation.

**How to report**: Suggest where an example would help; offer an example if possible.

### 4. Specification Gaps
**Example**: "The framework doesn't address [scenario]. How should it be handled?"

**We address this because**: Completeness is essential for a governance framework.

**How to report**: Describe the scenario; explain why the framework doesn't address it; suggest how it should be handled.

### 5. Guardrail Improvements
**Example**: "Guardrail X catches some errors but misses [related error]"

**We address this because**: Guardrails are the core mechanism for preventing reasoning failures.

**How to report**: Describe what the guardrail is designed to catch; identify gaps; suggest refinements.

---

## Types of Errors We Don't Address

### 1. Disagreement with Framework Philosophy
**Example**: "I disagree with the entire approach of treating sealed records as analyzable"

**Why**: The framework's philosophy is fundamental. Disagreement leads to alternative frameworks, not framework improvements.

**Alternative**: Develop your own framework; or document disagreement as academic critique rather than error.

### 2. Domain-Specific Application Disagreement
**Example**: "Your example for historical research would never work in practice"

**Why**: Practical application varies by domain. The framework provides methodology, not guarantees.

**Alternative**: Report if the framework documentation misrepresents application feasibility.

### 3. Requests for Executable Code or Software
**Example**: "Please create a software implementation of this framework"

**Why**: This repository is specification documentation, not software. Software development is a separate effort.

**Alternative**: Consider forking this documentation as a basis for software development.

### 4. Requests for Domain-Specific Presets
**Example**: "Add a domain-specific module for [specific field]"

**Why**: The framework is intentionally domain-agnostic. Domain-specific modules would undermine universality.

**Alternative**: Document how domain-specific specialization would be done using the framework methodology.

---

## Governance Feedback Process

If you have suggestions for improving the governance framework itself (not just fixing errors):

### Governance Feedback Format

```
GOVERNANCE FEEDBACK
===================
Topic: [What aspect of governance?]
Current State: [How does the framework currently address this?]
Proposed Improvement: [What should change?]
Reasoning: [Why is this improvement valuable?]
Examples: [Scenarios where this would help]

Alternatives Considered:
[Other ways to address this issue]

---
Submitter: [Your name/identifier]
Date: [Date of submission]
```

### What Governance Feedback We Consider

- **New guardrails**: Proposals for additional guardrails to catch reasoning errors
- **Guardrail refinements**: Ways to make existing guardrails more effective
- **Process improvements**: Better ways to apply the framework
- **Institutional context**: Insights on how the framework applies to specific contexts
- **Conflict resolution**: Proposals for handling cases where guardrails conflict

---

## Code of Conduct

This project follows a simple code of conduct:

### Be Respectful
- Assume good faith in others' feedback
- Disagree on substance, not on person
- Avoid inflammatory language

### Be Specific
- Clear, concrete error reports are more useful than vague complaints
- Provide examples and context
- Quote problematic passages exactly

### Be Constructive
- If you identify a problem, suggest a solution
- Explain why your suggestion is better
- Acknowledge limitations of your own suggestions

### Be Honest
- Don't submit false error reports
- Acknowledge if you're reporting opinion rather than error
- Distinguish facts from interpretation in your feedback

---

## Response Timeline

**Critical errors** (framework integrity compromised):
- Acknowledgment: Within 1 week
- Resolution: Within 2 weeks

**High-priority errors** (clarity, important gaps):
- Acknowledgment: Within 2 weeks
- Resolution: Within 1 month

**Medium-priority errors** (documentation clarity, minor issues):
- Acknowledgment: Within 1 month
- Resolution: Within 2 months (may be batched with other updates)

**Low-priority feedback** (suggestions, minor improvements):
- May be reviewed as part of version planning

---

## Version Updates

The framework is released in versions. Error corrections and governance improvements are incorporated into:

- **Point releases** (3.0.1, 3.0.2): Bug fixes and critical corrections
- **Minor releases** (3.1, 3.2): New guardrails or significant improvements
- **Major releases** (4.0): Fundamental restructuring

---

## Example Error Report

```
ERROR REPORT
============
File: GOVERNANCE.md
Location: Guardrail 1 section
Severity: High

Error Description:
The definition of temporal anchoring is unclear about whether it applies to
hypothetical scenarios or only historical claims. The section shows examples
only for historical events.

Current Text:
"Every claim must specify *when* it applies. Historical change is real;
temporal drift is a serious error."

Suggested Fix:
"Every claim must specify *when* it applies (or specify that it's hypothetical).
Temporal specificity applies to all claims about facts: historical events,
current states, and hypothetical scenarios. Temporal drift is a serious error."

Reasoning:
The framework applies to any contested domain, including policy analysis and
scientific disputes where hypothetical scenarios are discussed. The current
wording might suggest temporal anchoring only applies to historical claims.
Clarification would help users apply the guardrail to non-historical domains.

References:
- Framework.md states this framework is domain-agnostic
- Example 3 in examples.md discusses hypothetical scenarios

---
Reporter: Alice Smith
Date: 2025-11-17
```

---

## Questions?

For questions about the contribution process:
- See README.md for framework overview
- See GOVERNANCE.md for guardrail details
- See SECURITY.md for security concerns

---

**BordneAI Research Engine v3.0-alpha**
Specification for evidence-based reasoning. Released under CC BY 4.0.
