# Contributing to BordneAI Research Engine

---

## Important: This Specification Is Maintained by BordneAI

The BordneAI Research Engine is a **specification maintained by BordneAI**, not an open-source community project. We do not accept external pull requests.

**However, we welcome:**
- Error reports
- Clarity suggestions
- Framework improvement proposals
- Application examples and case studies
- Implementation feedback

---

## How to Report Errors

Found a factual error, ambiguity, or mistake in the specification?

### Step 1: Identify the Issue

Be specific:

- **File:** Which document? (README.md, SYSTEM_PROMPT-v3.3.1.md, docs/framework.md, etc.)
- **Location:** Section, paragraph, or line number
- **What's wrong:** The specific error or ambiguity
- **Evidence:** Why is this an error? (cite source if applicable)

### Step 2: Report It

**For public issues:** [GitHub Issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)

**Format:**
```
Title: [Brief description of error]

File: [specific file]
Location: [specific section]

Error: [What is stated incorrectly]

Correction: [What should be stated instead]

Evidence/Justification: [Why this is wrong]
```

**For sensitive issues:** Email research@bordneai.org

### Step 3: We'll Investigate and Fix

- If error is confirmed, we'll update the specification
- We'll note the contribution in [CHANGELOG.md](CHANGELOG.md)
- We'll follow up with you on resolution

---

## How to Suggest Clarity Improvements

Is the framework hard to understand? Is an example unclear?

### Step 1: Identify the Clarity Issue

Be specific:

- **What's confusing:** Which part of the text is hard to follow?
- **What would help:** More explanation, examples, diagrams, restructuring?
- **Why it matters:** Does this affect understanding of governance rules? Implementation?

### Step 2: Report It

**Via GitHub Issues:**

```
Title: Clarity improvement: [section name]

Location: [specific file and section]

Current text: [quote the confusing part]

What's confusing: [explain what's hard to understand]

Suggested improvement: [propose how to clarify]
```

### Step 3: We'll Improve It

- If improvement is justified, we'll update the documentation
- We'll acknowledge contributions in [CHANGELOG.md](CHANGELOG.md)
- We'll follow up on resolution

---

## How to Propose Framework Changes

Do you think a governance rule should change? A tier should be re-defined?

### Important Notes

The **core philosophy is fixed:**
- Prioritize documents over narratives
- Separate known from claimed
- Make uncertainty explicit
- Refuse unanchored suppression claims

**Governance principles are stable:**
- Temporal Anchoring
- Conflict Resolution (BAAM Weighting)
- Suppression guardrails
- Self-Check protocol

**However, we consider refinements** if they:
- Improve clarity without changing meaning
- Strengthen governance without compromising flexibility
- Add necessary exceptions without creating loopholes

### Step 1: Develop Your Proposal

**What we need:**

1. **Current rule or principle:** What exists now?
2. **Proposed change:** What should change?
3. **Rationale:** Why is this change needed?
4. **Evidence:** What evidence supports this change?
5. **Scope:** What domains/use cases are affected?
6. **Risks:** What could go wrong if we make this change?

### Step 2: Submit for Review

**Email:** research@bordneai.org

**Format:**
```
Subject: Proposal: [Framework change]

Current Rule/Principle:
[Cite the rule from SYSTEM_PROMPT-v3.3.1.md or governance docs]

Proposed Change:
[State the change clearly]

Rationale:
[Why this change is needed]

Evidence:
[Cite examples, research, or use cases supporting change]

Affected Domains:
[Where does this apply?]

Implementation Impact:
[How would this affect existing implementations?]

Risks:
[What could go wrong?]

Implementation Notes:
[How would this work in practice?]
```

### Step 3: We'll Review and Decide

- We'll evaluate against framework philosophy and principles
- We'll consider impact on implementations
- We'll discuss with you if clarification is needed
- We'll decide whether to adopt, modify, or decline
- We'll explain our reasoning either way

---

## How to Share Implementation Examples

Have you built something using this framework? Found interesting applications?

### We Welcome:

✅ Case studies: "We used this framework to analyze [domain]"
✅ Implementation notes: "Here's how we implemented [feature]"
✅ Lessons learned: "We discovered [insight] using the framework"
✅ Challenges: "We found [difficulty] and solved it by [approach]"
✅ Feedback: "Here's what worked well and what was hard"

### How to Share

**Via GitHub Issues (public):**
- Start a discussion with examples and lessons learned
- Include: domain, what worked, what didn't, insights
- This helps others and demonstrates framework utility

**Via Email (private):**
- Email research@bordneai.org if you prefer private feedback
- We may ask permission to share anonymized lessons

---

## Code of Conduct

When contributing feedback, discussions, or proposals:

1. **Be specific.** "This is confusing" is less useful than "The term 'entropy level' is used inconsistently in sections 2.1 and 3.2"
2. **Cite evidence.** If proposing a change, provide evidence or examples
3. **Acknowledge alternatives.** If others disagree with your proposal, engage with their perspective
4. **Distinguish fact from opinion.** "The framework states X" (fact) vs. "I think X should be Y" (opinion)
5. **Assume good faith.** Framework decisions reflect principles, not arbitrary choices

We reserve the right to decline contributions that:
- Contradict core principles without substantial evidence
- Propose domain-specific categories (contradicts universality)
- Suggest weakening governance guardrails
- Include disrespect or bad faith arguments

---

## What Won't Be Accepted

We will **not accept:**

❌ PRs that modify the framework without prior discussion (see "How to Propose" above)
❌ Requests to add predefined domains or categories (framework is universal)
❌ Requests to weaken Temporal Anchoring, BAAM Weighting, or Suppression guardrails
❌ Proposals that enforce particular political, ideological, or religious positions
❌ Feature requests for unrelated software
❌ Contributions that misrepresent the framework's capabilities or limitations

---

## Attribution & Recognition

**When we accept your contribution:**

- We'll acknowledge you in [CHANGELOG.md](CHANGELOG.md) with your name (or pseudonym if preferred)
- Error corrections are attributed as "Reported by [name]"
- Improvement suggestions are attributed as "Suggested by [name]"
- Major proposals are attributed with explanation of contribution
- You retain copyright in CC BY 4.0 attribution model

---

## Timeline for Review

- **GitHub Issues:** Reviewed within 2-4 weeks
- **Email proposals:** Reviewed within 2-4 weeks
- **Critical errors:** Reviewed and resolved within 1 week
- **Implementation feedback:** Reviewed and incorporated into next version

---

## Questions?

- **About framework usage:** See [README.md](README.md) or [docs/](docs/)
- **About governance rules:** See [docs/governance.md](docs/governance.md)
- **About this contribution process:** Email research@bordneai.org

---

## Summary

| Type | Method | Expectation |
|------|--------|-------------|
| **Error report** | GitHub Issues or email | Fix if confirmed |
| **Clarity suggestion** | GitHub Issues | Improve documentation if justified |
| **Framework proposal** | Email with full analysis | Review and respond with decision |
| **Implementation feedback** | Email or GitHub discussion | Inform future improvements |
| **No PRs** | N/A | Maintain specification integrity |

---

*BordneAI Research Engine v3.3.1 | Contribution Guidelines | 2025-11-17*
