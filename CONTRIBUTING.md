# CONTRIBUTING.md: Governance Updates & External Feedback

## Repository Status

The BordneAI Research Engine is a **reference specification maintained by the BordneAI team**, not an open-source project accepting external pull requests or contributions.

**External PRs will not be accepted.** However, feedback and issue reports are welcome and will be reviewed on merit.

---

## Contributing Without PRs: How to Help

### 1. Report Errors or Misalignments

If you identify:
- Factual errors in examples or guidance
- Outdated information (e.g., declassification dates)
- Misaligned governance rules
- Prompt injection vulnerabilities
- Documentation clarity issues

**How to Report:**
- GitHub Issues (public): https://github.com/BordneAI/BordneAI-Research-Engine/issues
- Email (private): BordneAI@bordne.com
- Include: specific claim, evidence of error, suggested correction

**Response:** Verified errors will be incorporated in next version update and logged in CHANGELOG.md.

---

### 2. Propose Governance Changes

If you believe a governance rule should be modified:

**How to Propose:**
1. Email BordneAI@bordne.com with:
   - Current rule (cite GOVERNANCE.md or SYSTEM_PROMPT-v3.0.md section)
   - Proposed change
   - Rationale (why should this be modified?)
   - Impact analysis (what would change if adopted?)
   - Domain(s) affected

2. Provide context:
   - Is this based on a real query or scenario?
   - Have you identified a misalignment with stated principles?
   - Is this a performance issue or a philosophical disagreement?

3. Allow time for review (typically 2–4 weeks)

**Examples of Viable Proposals:**
- "GOVERNANCE.md disallows [claim], but the rule is too broad/narrow because [reasoning]"
- "SOURCING_PROFILE_V2.1.md doesn't address [edge case]. Suggestion: [addition]"
- "docs/domains.md needs updated declassification dates for [incidents]. Here's current info: [links]"

**Examples of Non-Viable Proposals:**
- "I want the system to make [unsubstantiated claim]" (contradicts governance)
- "The rules are too restrictive for my use case" (design choice; not changing)
- "Other systems allow [X]; why can't you?" (comparison, not substantive)

---

### 3. Suggest New Domains

If you believe a domain should be added:

**How to Propose:**
1. Email BordneAI@bordne.com with:
   - Domain name and scope (1–2 sentences)
   - Authoritative T1 sources available (what's declassified?)
   - Key T2 sources (what research exists?)
   - Domain-specific disallowed claims (what should be prevented?)
   - Guardrails needed (constraints specific to this domain?)
   - Use cases (what questions would this domain answer?)

2. Demonstrate evidence base:
   - Is there sufficient T1 declassified material?
   - Are there established T2 analytical frameworks?
   - Is this a topic with institutional complexity (not pure entertainment)?

3. Allow time for review (typically 4–8 weeks for full domain design)

**Example Viable Domain Proposal:**
```
Domain Name: arms_control_verification

Scope: Declassified arms control treaties, verification mechanisms,
inspection records, institutional challenges in verification

T1 Sources: State Department treaty archives, IAEA public records,
Congressional testimony on treaty compliance

T2 Sources: Academic analyses of verification mechanisms,
peer-reviewed policy research

Disallowed Claims: "Country X definitely violated [treaty]" (without
T1 evidence of violation)

Guardrails: Physics constraints on weapon systems, treaty language
precision, institutional inspection limitations

Use Cases: "What do declassified records show about [treaty]
compliance?", "How do verification mechanisms work?", "What
institutional incentives shape reporting?"
```

---

### 4. Contribute Examples or Case Studies

If you have a real-world query that illustrates governance principles:

**How to Submit:**
1. Email BordneAI@bordne.com with:
   - The query or scenario
   - Domain(s) involved
   - T1/T2/T3 evidence available
   - How it illustrates governance (which rules does it show?)
   - Permission to include in documentation

2. Provide context:
   - Is this declassified material?
   - Are there privacy concerns?
   - Is this relevant to multiple audiences?

3. If approved, example will be added to docs/examples.md with attribution

---

### 5. Identify Security or Misuse Concerns

See SECURITY.md for detailed guidelines on:
- Reporting vulnerabilities
- Reporting misuse
- Security disclosure best practices

---

## What Will NOT Be Accepted

- ❌ **Pull Requests:** External code/documentation PRs not merged (design choice; maintain architectural integrity)
- ❌ **Repository Forks for Production:** Don't fork without clear governance; maintain community alignment
- ❌ **Policy Disagreements:** Won't change governance because you want different rules (design philosophy is fixed)
- ❌ **Feature Requests Contradicting Stated Principles:** Won't add features that violate core governance (e.g., "make unanchored suppression claims")

---

## Update Process & Version Bumps

When feedback is accepted, here's what happens:

### Minor Corrections (Typos, Clarifications)
- ✅ Incorporated in next quarterly update
- ✅ Noted in CHANGELOG.md
- ❌ No version bump

### Factual Errors or Governance Clarifications
- ✅ Incorporated in next version update
- ✅ Logged in CHANGELOG.md
- ✅ Minor version bump (v3.Y)

### New Domains or Governance Rules
- ✅ Full review process (2–8 weeks)
- ✅ Design documentation completed
- ✅ Updated GOVERNANCE.md, SYSTEM_PROMPT-v3.0.md
- ✅ Examples added to docs/
- ✅ Minor or major version bump (depending on scope)

### Major Governance Revisions
- ✅ Architectural review (1–3 months)
- ✅ Stakeholder consultation
- ✅ Major version bump (vX+1.0)

---

## Governance Framework Stability

The BordneAI Research Engine's core governance principles are **intentionally stable**:

- **Verifiability First** (non-negotiable)
- **Structural Secrecy Respect** (non-negotiable)
- **Competing Hypotheses Valued** (non-negotiable)

These pillars will not be changed, even if requested. Domain-specific rules, examples, and clarifications can be updated, but the foundational philosophy is fixed.

---

## Code of Conduct

Feedback and contributions should:
- ✅ Be respectful and constructive
- ✅ Cite evidence for claims
- ✅ Acknowledge legitimate alternative views
- ✅ Distinguish between factual errors and policy disagreements
- ✅ Provide specific, actionable suggestions

Hostile, abusive, or spam submissions will be closed without response.

---

## Questions?

For questions about the contribution process:

**Email:** BordneAI@bordne.com (subject: "CONTRIBUTING QUESTION")

**Or check:**
- GOVERNANCE.md (governance rules)
- SECURITY.md (security/misuse concerns)
- NOTICE.md (repository scope and disclaimers)

---

## Attribution

All accepted feedback and contributions will be:
- ✅ Logged in CHANGELOG.md
- ✅ Attributed to contributor (if desired)
- ✅ Incorporated into version history

When you submit feedback or a suggestion, you grant permission to:
- Include it in the public repository
- Distribute it under CC BY 4.0 license
- Attribute it to you (or anonymously, if preferred)

---

## Thank You

Feedback helps improve clarity, catch errors, and ensure the governance framework is robust. We appreciate thoughtful contributions, even if they're not all accepted.

---

**Repository:** BordneAI Research Engine v3.0-alpha
**License:** CC BY 4.0
**Maintained By:** David Bordne
**Last Updated:** 2025-11-17
