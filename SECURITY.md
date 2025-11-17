# SECURITY.md: Vulnerability & Misuse Reporting

## What This Repository Is

The BordneAI Research Engine is a **specification and governance document**, not executable software or a deployed system. This repository contains:

- Instructional governance documentation
- Sourcing frameworks and methodology
- Domain-specific reasoning guidelines
- Examples of reasoning patterns

**This repository does NOT contain:**
- Executable code
- Model weights or neural network parameters
- Proprietary algorithms
- Authentication logic
- Data processing systems
- Security-critical infrastructure

---

## Security Scope

Because this is a specification-only repository, traditional software security concerns do not apply:

### Not Applicable

- ❌ No code vulnerabilities (no code to exploit)
- ❌ No memory corruption or injection attacks
- ❌ No authentication bypass (no authentication system)
- ❌ No data breach risk (no database)
- ❌ No dependency vulnerabilities (no production dependencies)
- ❌ No cryptographic weaknesses (no cryptography used)

### Potentially Applicable

- ✅ Prompt injection vulnerabilities (if used as system prompt for LLM)
- ✅ Governance misalignment (if used to guide high-stakes decisions)
- ✅ Misuse scenarios (if applied to malicious purposes)
- ✅ Documentation errors (factual inaccuracies in examples)
- ✅ Outdated information (if not kept current with declassification)

---

## Responsible Disclosure

### If You Find a Security Concern

**Do:**
1. Email BordneAI@bordne.com with:
   - Clear description of the concern
   - Specific location in repository (file, section, line)
   - Reason it's a security issue
   - Suggested remediation
2. Allow reasonable time (30 days) for response before public disclosure
3. Provide enough detail for the team to verify and reproduce

**Don't:**
- Public GitHub issues for security concerns (use private email)
- Disclose vulnerabilities publicly before notification
- Use issue reports as a vector for attacks or social engineering

### Examples of Valid Security Concerns

1. **Prompt Injection Vulnerability:** "The governance rules in SYSTEM_PROMPT could be bypassed via [injection technique]. Suggested fix: [mitigation]"

2. **Governance Misalignment:** "The disallowed claims list in GOVERNANCE.md doesn't prevent [malicious use case]. Suggested update: [rule addition]"

3. **Factual Error with Security Implication:** "The example in docs/examples.md contains factually incorrect information about [topic], which could mislead [stakeholder]. Correction: [accurate information]"

4. **Outdated Information:** "The declassification date referenced in docs/domains.md is wrong; correct date is [X]. This affects [reasoning]."

5. **Misuse Scenario Not Addressed:** "These governance rules could be applied to [harmful purpose]. Suggest adding guardrail: [proposal]"

---

## Misuse Reporting

### If You Observe This System Being Misused

Report to: BordneAI@bordne.com (subject: "MISUSE REPORT")

**Include:**
- Description of misuse (what is the system being used for?)
- How it contradicts stated governance
- Any relevant evidence or links
- Stakeholders affected

**Examples of reportable misuse:**

1. **Deceptive Use:** System applied to generate persuasive-sounding misinformation about sensitive topics

2. **Adversarial Use:** Governance rules bypassed or inverted to support unsubstantiated claims in high-stakes context

3. **Supply Chain Compromise:** System deployed with modified governance rules without attribution or disclosure

4. **Escalation Risk:** System applied to contexts not intended (e.g., high-stakes military decision-making without human oversight)

5. **Malicious Implementation:** Code implementation of governance that deliberately undermines stated principles

---

## What NOT to Report

These are **not** security concerns in this context:

- ❌ "I disagree with the governance philosophy" (legitimate policy disagreement, not security issue)
- ❌ "The system limits what it will say about X" (designed guardrail, not bug)
- ❌ "I wish the system would make [claim] without sourcing" (violates intentional design)
- ❌ "Other systems are less constrained" (comparison, not vulnerability)
- ❌ "The examples don't cover my use case" (feature request, not security issue)

---

## Responsible Use Guidelines

### If You Implement This Framework

**Do:**
1. Conduct independent safety review appropriate to your context
2. Establish human oversight and review procedures
3. Audit outputs for accuracy before public or high-stakes use
4. Monitor for adversarial input or misuse
5. Report errors or misalignment issues
6. Maintain attribution and license compliance

**Don't:**
- Use in critical infrastructure without additional safety validation
- Deploy in high-stakes decision contexts without human oversight
- Modify governance rules without clear documentation and review
- Claim greater capability or reliability than documented
- Hide errors or misalignments

### If You Fork or Adapt This Repository

1. Maintain clear attribution (CC BY 4.0 required)
2. Document all modifications
3. Establish equivalent or stronger governance safeguards
4. Conduct independent safety review
5. Provide comparable security/misuse reporting procedures
6. Consider contributing improvements back to original project

---

## Security Practices

### Version Tracking

All changes documented in CHANGELOG.md for auditability:
- Users can verify what's changed between versions
- Researchers can reproduce analysis using specific version
- Misalignments can be flagged against version history

### Cross-Reference Validation

Critical governance rules cross-referenced across files:
- GOVERNANCE.md references SYSTEM_PROMPT-v3.0.md (rules consistent)
- docs/examples.md shows governance in action (alignment visible)
- SOURCING_PROFILE can be used standalone (no hidden dependencies)

### Attribution & License

CC BY 4.0 license requires:
- Attribution: "By David Bordne, licensed under CC BY 4.0"
- Derivative works must maintain license and attribution
- Modifications must be clearly marked

This creates accountability trail for who modified what.

### Correction Protocol

Errors can be flagged and tracked:
1. User or researcher identifies error
2. Developer verifies and documents
3. Correction incorporated in next version
4. Change logged in CHANGELOG.md
5. Versioning allows retroactive identification of error

---

## Privacy Considerations

### What This Repository Collects

**This repository does not collect data.** It is static documentation.

If deployed as a live service:
- Query content may be logged (user privacy concern)
- Metadata (query timestamps, domain, user ID) may be tracked
- Correction submissions may be retained

**Users should assume:** Any input to a live deployment may be logged and used for improvement.

### Declassified Information Respect

This repository discusses declassified information, which is by definition public.

However, sensitive topics are treated with care:
- Techniques for declassified material are not used to deduce classified material
- Institutional secrecy is respected (not assumed to hide specific content)
- Personnel identities in declassified material are handled per source document

---

## Support & Questions

For security questions or concerns:

**Email:** BordneAI@bordne.com
**Subject line:** "SECURITY" (for confidential concerns)

Response timeline: Good-faith security reports will receive acknowledgment within 7 days and substantive response within 30 days.

---

## Disclaimer

This repository is provided "as-is" with no guarantee of security, safety, or fitness for any purpose.

Users deploying implementations based on this specification are responsible for:
- Independent security review
- Safety validation for their context
- Compliance with applicable laws and regulations
- Responsible use monitoring

---

**Version:** Part of BordneAI Research Engine v3.0-alpha
**Last Updated:** 2025-11-17
**License:** CC BY 4.0
**Maintained By:** David Bordne
