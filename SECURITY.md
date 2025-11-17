# Security & Responsible Disclosure

---

## Important: This Is Not Software

The BordneAI Research Engine v3.3.1 is **instructional documentation**, not executable code.

**Traditional software security vulnerabilities do not apply** to this repository:

- ❌ No buffer overflows (no executable code)
- ❌ No injection attacks (no input-processing code)
- ❌ No cryptographic flaws (no cryptography implementation)
- ❌ No dependency vulnerabilities (no external dependencies)
- ❌ No memory safety issues (not a compiled program)
- ❌ No API exploitation (framework is not an API endpoint)

---

## What "Security" Means for This Framework

Security concerns relevant to a governance specification are:

### 1. Misrepresentation of Scope

**Concern:** Framework presented as having capabilities it doesn't have, or restrictions it doesn't enforce.

**Example:** Claiming the framework "guarantees accuracy" or "is safe for all decision-making."

**How to report:** See section below.

### 2. Misuse in Harmful Contexts

**Concern:** Framework being used to justify unanchored claims, dismiss expert consensus, or replace professional judgment in critical domains.

**Example:** Using "suppression guardrails" to dismiss medical expertise, or "entropy levels" to claim evidence is unknowable.

**How to report:** See section below.

### 3. Misinterpretation of Governance Rules

**Concern:** Framework rules interpreted in ways that contradict their intended function.

**Example:** Using "BAAM weighting" to dismiss T2 consensus in favor of T4 opinion.

**How to report:** See section below.

### 4. Documentation Accuracy

**Concern:** Errors, ambiguities, or misleading statements in the specification itself.

**Example:** Governance rule stated incorrectly, or example that doesn't follow framework principles.

**How to report:** See section below.

---

## Reporting Security Concerns

### For Implementation-Level Issues (Builders Using This Framework)

If you are building an AI system or tool based on this framework and discover:

- A rule that enables harmful outputs
- An ambiguity that leads to unsafe behavior
- A governance gap that allows misuse
- An unintended interpretation that creates risk

**Report privately:** email security@bordneai.org

**Include:**
1. What the issue is
2. How it manifests in practice
3. Suggested fix or mitigation
4. Whether you're willing to discuss publicly

**Response time:** We aim to respond within 2 weeks.

### For Framework Specification Issues (Clarity, Accuracy)

If you identify:

- Contradictions in the specification
- Governance rules that are ambiguous
- Examples that don't match the rules
- Language that could be misunderstood

**Report publicly:** [GitHub Issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)

**Include:**
1. Specific location (file, section)
2. What the issue is
3. Why it's a problem
4. Suggested clarification

### For Misuse Concerns (Framework Being Misrepresented)

If you observe the framework being misrepresented or used to justify harmful claims:

**For research/educational misuse:** Email research@bordneai.org

**For commercial/deployed misuse:** Email security@bordneai.org

**What helps:** Specific example of misuse, URL or screenshot, nature of harm.

---

## What We Will Do

### We Will:

✅ **Investigate credible reports** of framework misuse or misrepresentation
✅ **Fix documentation errors** that enable misuse
✅ **Clarify ambiguous rules** that create security gaps
✅ **Provide guidance** to implementers on secure usage
✅ **Acknowledge contributions** of researchers reporting issues
✅ **Publish corrections** when significant errors are found

### We Will NOT:

❌ **Restrict topics.** The framework is domain-agnostic. No topics are off-limits for evidence-based inquiry.
❌ **Enforce conclusions.** The framework governs reasoning, not beliefs.
❌ **Censor implementation.** Implementers decide how to deploy the framework.
❌ **Retract governance principles.** Core rules (Temporal Anchoring, BAAM Weighting, Suppression guardrails, Self-Check) are stable.

---

## Responsible Implementation

If you are building a system using this framework, consider:

1. **Accuracy of Sourcing:** Does your system correctly classify sources into T1-T4 tiers?
2. **Entropy Assessment:** Does your system accurately assess uncertainty levels?
3. **Governance Compliance:** Do responses follow the four governance principles?
4. **Mode Selection:** Does your system correctly choose between Lightweight and Structured modes?
5. **Limitation Disclosure:** Do outputs clearly state scope limitations and when professional consultation is needed?
6. **Testing:** Have you tested responses against the framework specification to ensure compliance?

---

## Not a Substitute for Professional Standards

This framework does **not** exempt implementation from:

- **Professional ethics** in relevant domains (medical ethics, legal ethics, etc.)
- **Regulatory compliance** (HIPAA for health, GDPR for data, SEC for finance, etc.)
- **Local legal requirements** (varying by jurisdiction)
- **Professional standards** (medical boards, bar associations, engineering standards, etc.)
- **Institutional governance** (your organization's policies and procedures)

---

## Vulnerability Disclosure Timeline

If we discover a significant issue with the framework specification:

1. **Day 1-7:** Assess severity and scope
2. **Day 7-14:** Develop correction or clarification
3. **Day 14-21:** Release public correction
4. **Follow-up:** Monitor for misuse of the error

For critical errors (e.g., a governance rule that demonstrably enables harmful outputs), we prioritize faster release.

---

## Transparency

We maintain:

- **Version history** in [CHANGELOG.md](CHANGELOG.md)
- **Governance documentation** in [docs/governance.md](docs/governance.md)
- **Limitation statements** in [NOTICE.md](NOTICE.md)
- **Contribution guidelines** in [CONTRIBUTING.md](CONTRIBUTING.md)

All changes are documented and attributed.

---

## Questions?

- **About this framework's usage:** consult [README.md](README.md) or [docs/framework.md](docs/framework.md)
- **About governance rules:** consult [docs/governance.md](docs/governance.md)
- **About limitations:** consult [NOTICE.md](NOTICE.md)
- **About reporting:** see above

---

*BordneAI Research Engine v3.3.1 | Responsible Disclosure Policy | 2025-11-17*
