# NOTICE: Scope and Limitations

## What This Repository Contains

The BordneAI Research Engine is a **specification document** describing a governed epistemic system for evidence-based inquiry. This repository contains:

- **Documentation**: System instructions, methodology guides, sourcing specifications, governance rules
- **Templates**: Example prompts for deployment in LLM systems
- **Examples**: Generic (non-incident-specific) methodology demonstrations
- **No executable code**: No software, no model weights, no deployed system

This is **not a software package**. It is **instructional specification documentation** designed to be copied into language model systems as a system prompt or context.

---

## Important Disclaimers

### 1. Non-Production Status
The BordneAI Research Engine v3.0-alpha is **specification documentation only**. It has not been deployed in production systems. It is suitable for:
- Research and study of epistemic systems
- Testing in controlled environments
- Deployment as a system prompt in LLM APIs (Claude, ChatGPT, etc.)
- Educational examination of evidence-based reasoning

### 2. No Automated Reasoning
This framework describes methodology for **human-guided analysis** using LLM systems. The LLM executes the reasoning process under human direction; humans are responsible for:
- Formulating questions
- Evaluating whether the analysis is sound
- Making decisions based on the analysis
- Verifying claims against sources

### 3. Knowledge Cutoff Limitations
The framework applies only to questions that can be anchored to evidence available at the time of analysis. The framework explicitly refuses to analyze:
- Pure speculation (no T1/T2 evidence base)
- Questions post-dating available evidence
- Unanchored conspiracy claims

### 4. Domain Applicability
The framework is **universal and domain-agnostic**. It can be applied to any contested domain. However:
- **Appropriate domains**: Historical research, institutional analysis, policy analysis, scientific disputes, intelligence assessment
- **Inappropriate domains**: Personal advice, medical diagnosis, legal guidance requiring professional expertise
- **User responsibility**: The user must determine whether the framework is appropriate for their question

### 5. Not a Source of Truth
The BordneAI Research Engine is not a source of truth about any domain. It is a **method for analyzing evidence**. The framework's output is only as good as:
- The evidence available
- The accuracy of source tier assignments
- The completeness of hypothesis identification
- The application of guardrails

Users are responsible for independently verifying claims and evaluating analysis quality.

### 6. Evidence Limitations
The framework is subject to fundamental limitations:
- **Sealed records**: Information that is sealed cannot be directly accessed
- **Unknown information**: Gaps in evidence may be large or systematic
- **Source bias**: All sources reflect incentives and perspectives
- **Interpretation uncertainty**: Competing hypotheses may have similar confidence levels

The framework acknowledges these limitations; it does not overcome them.

---

## Use Cases

### Recommended Uses
- **Research and Analysis**: Systematic examination of contested questions using documented evidence
- **Educational**: Learning how to reason rigorously about incomplete information
- **Policy Analysis**: Understanding institutional behavior and decision-making
- **Historical Research**: Analyzing competing historical narratives with source evaluation
- **Scientific Disputes**: Weighing competing scientific hypotheses and research findings
- **Intelligence Analysis**: Reasoning about sealed records using institutional incentive frameworks

### Not Recommended Uses
- **Personal Decisions**: Do not use for medical, legal, or personal advice requiring specialized expertise
- **Real-Time Emergencies**: Not designed for time-critical decision-making
- **Replacing Professional Expertise**: Not a substitute for specialized professionals (doctors, lawyers, etc.)
- **Automated Decision-Making**: Framework requires human judgment; do not automate decisions based on framework output alone

---

## Attribution & Licensing

This work is released under **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

**You must:**
- Provide attribution to BordneAI Research Engine
- Include the license text (see LICENSE.md)
- Indicate if changes were made
- Include a copy of the license with any distribution

**You may:**
- Use for any purpose (commercial or noncommercial)
- Modify and adapt the framework
- Distribute or republish

See LICENSE.md for full licensing terms.

---

## Governance & Feedback

### Errors or Issues
If you find errors in the specification or examples, report them:
- See CONTRIBUTING.md for reporting procedure
- Include specific location of error
- Describe the problem and suggest fix if possible

### Security or Misuse Concerns
See SECURITY.md for responsible disclosure of potential misuse.

### Governance Improvement Proposals
For suggestions on improving the governance framework or adding guardrails, see CONTRIBUTING.md.

---

## Version Information

**Current Version**: v3.0-alpha
**Release Date**: 2025-11-17
**Status**: Specification complete; ready for alpha testing and deployment

This is an **alpha release**. The framework is stable and ready for use, but may be updated as deployment experience accumulates.

See CHANGELOG.md for version history and planned updates.

---

## Contact & Support

This is specification documentation; it does not have traditional "support." However:
- **Questions about framework**: See the README.md and docs/ folder
- **Questions about system instructions**: See SYSTEM_PROMPT-v3.0.md
- **Questions about sourcing**: See SOURCING_PROFILE_V2.1.md
- **Questions about guardrails**: See GOVERNANCE.md
- **Errors or suggestions**: See CONTRIBUTING.md

---

**BordneAI Research Engine v3.0-alpha**
Specification documentation released under CC BY 4.0
