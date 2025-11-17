# BordneAI Research Engine v3.3.1

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/) [![Status: Specification](https://img.shields.io/badge/Status-Specification-blue.svg)](#) [![Version: 3.3.1](https://img.shields.io/badge/Version-3.3.1-brightgreen.svg)](#)

**Quick Links:** [System Prompt](SYSTEM_PROMPT-v3.3.1.md) | [Framework Guide](docs/framework.md) | [Examples](docs/examples.md) | [Governance Rules](docs/governance.md) | [License](LICENSE.md)

---

## What is BordneAI Research Engine?

The BordneAI Research Engine is a **universal governed analytic system for any domain where evidence, ambiguity, or conflict exists**. It is not a tool for one topic—it applies equally to science, history, policy, medicine, finance, law, and social issues. You choose the topic; the framework governs how you analyze it.

The engine combines three analytical layers: **tiered sourcing (T1-T4) that prioritizes documents over narratives**, **entropy levels (L1-L5) that calibrate assessment confidence**, and **structured governance rules that separate what is known from what is claimed**. This creates transparent, auditable reasoning regardless of whether you're analyzing declassified records, disputed history, scientific disagreements, policy conflicts, or institutional secrecy.

### Core Philosophy

The framework is built on four commitments:

- **Prioritize documents over narratives.** Primary sources and authoritative technical documentation outweigh opinions and testimony.
- **Separate what is known from what is claimed.** Explicitly distinguish verified facts from analysis, interpretation, and hypothesis.
- **Make uncertainties explicit.** When evidence is incomplete or conflicting, say so. Refusal to commit beyond what evidence supports is a feature, not a limitation.
- **Distinguish absence of evidence from evidence of absence.** Unknown information is not proof of suppression or conspiracy; structural incentives may explain silence.

---

## Key Features

✅ **Tiered Sourcing (T1-T4)** — Four evidence tiers from documents to opinion; tier classification determines confidence ceilings
✅ **Entropy Levels (L1-L5)** — Behavioral guidance keyed to certainty and stakes; low-entropy topics use lightweight structure, high-entropy topics require full governance
✅ **Lightweight + Structured Modes** — Choose minimal structure for casual questions or full scaffolding for high-stakes claims
✅ **Conflict Resolution (BAAM Weighting)** — Explicit priority rules when evidence tiers disagree; T1 > T2 > T3 > T4
✅ **Suppression/Secrecy Guardrails** — Explains institutional incentives for silence without asserting unanchored conspiracy claims
✅ **Temporal Anchoring** — Time-sensitive claims require explicit dates; enables fact-checking and correction
✅ **Self-Check Protocol** — Built-in validation to prevent overconfidence and ensure governance rules are applied

---

## How It Works

### Tiered Sourcing

All claims are traced to source material classified into four tiers:

- **T1 Primary/Official/Direct:** Laws, court dockets, official reports, raw datasets, archival records, peer-reviewed raw data tables
- **T2 Scholarly/Authoritative Technical:** Peer-reviewed articles, academic books, official technical documentation, reference works
- **T3 Reputable Secondary:** Mainstream reporting with T1/T2 citations, textbooks, quality explainers, whitepapers
- **T4 Testimony/Opinion:** Named expert statements, anonymous posts, hearsay, speculation

When you see claims sourced to T1+T2, confidence is inherently higher. When only T3 or T4 is available, assessment must reflect that constraint. When sources disagree, the framework shows why rather than hiding conflict.

### Entropy Levels

Not all questions have the same evidentiary profile. The system assigns entropy levels based on how much evidence exists, how controversial it is, and what's at stake:

- **L1-L2:** Simple, well-documented, low conflict (lightweight structure sufficient)
- **L3:** Mixed evidence, moderate ambiguity (browse for T1/T2, explain disagreement)
- **L4:** Contested, high-stakes, significant disagreement (full structured response required)
- **L5:** Insufficient evidence or prohibitive uncertainty (focus on unknowns, refuse overconfidence)

### Lightweight vs. Structured Mode

**Lightweight Mode** applies to low-stakes questions where evidence is clear (factual lookups, simple coding, casual opinions). Sourcing remains implicit; tiers don't need explicit labeling.

**Structured Mode** applies to contested topics, high-stakes claims, or questions with incomplete evidence. It uses the full response template with explicit tier attribution, confidence calibration, and governance checkpoints.

**Default rule: When in doubt, choose Structured Mode.**

---

## When to Use Structured Mode

Structured mode is **required** for:

- **Medicine/Health/Psychology** (evidence-based assessment, conflict with alternative approaches)
- **Law/Policy/Regulation** (legal standards, compliance, interpretation disputes)
- **Finance/Investment/Security** (risk assessment, market claims, vulnerability analysis)
- **Politics/Elections/Social Conflict** (contested narratives, competing factual claims)
- **Disputed History/Archaeology** (competing interpretations, declassified records, archaeological evidence)
- **Safety-Critical Systems** (medical devices, structural safety, security infrastructure)
- **Any topic where incompleteness or conflict is evident**

---

## Repository Structure

| File | Purpose |
|------|---------|
| **[SYSTEM_PROMPT-v3.3.1.md](SYSTEM_PROMPT-v3.3.1.md)** | Canonical system instructions; read this first for authoritative specification |
| **[docs/framework.md](docs/framework.md)** | How tiered sourcing + entropy apply to *any* topic; detailed methodology guide |
| **[docs/examples.md](docs/examples.md)** | Generic methodology examples showing lightweight vs. structured mode in action |
| **[docs/governance.md](docs/governance.md)** | Safety rules (Temporal Anchoring, Conflict Resolution, Suppression guardrails, Self-Check) |
| **[prompts/lightweight-template.md](prompts/lightweight-template.md)** | Guidance for informal queries and minimal-structure analysis |
| **[NOTICE.md](NOTICE.md)** | Operational clarifications and limitations |
| **[SECURITY.md](SECURITY.md)** | Misuse reporting and responsible disclosure |
| **[CONTRIBUTING.md](CONTRIBUTING.md)** | How to report errors and propose improvements |
| **[CHANGELOG.md](CHANGELOG.md)** | Version history and audit trail |

---

## Quick Start

**I'm new. Where do I start?**
→ Read the "How It Works" section above, then review [docs/examples.md](docs/examples.md) to see the framework in action.

**I need to analyze a specific topic. What's the process?**
→ Read [docs/framework.md](docs/framework.md) to understand tier classification and entropy levels for your domain, then consult [docs/governance.md](docs/governance.md) for safety rules.

**I'm implementing this system. What's the spec?**
→ Read [SYSTEM_PROMPT-v3.3.1.md](SYSTEM_PROMPT-v3.3.1.md) (canonical) and [docs/governance.md](docs/governance.md) (rules).

**I found an error or want to propose a change.**
→ See [CONTRIBUTING.md](CONTRIBUTING.md) for reporting protocols.

**I have a policy or legal question. Can this framework help?**
→ Yes, but see [docs/governance.md](docs/governance.md) for when professional consultation is required.

---

## Deployment

This framework is deployed as:

- **Specification Document** (this repository)
- **System Prompt for AI Agents** (SYSTEM_PROMPT-v3.3.1.md)
- **Reference Implementation** (live deployment in AI assistant applications)

All responses are governed by the rules documented in [docs/governance.md](docs/governance.md) and validated against the [SYSTEM_PROMPT-v3.3.1.md](SYSTEM_PROMPT-v3.3.1.md) specification.

---

## Feedback & Issues

### Report Errors

Found a factual error or ambiguity in this framework? Please report:

- **GitHub Issues:** [BordneAI-Research-Engine/issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)
- **Email:** contact@bordneai.org
- **Correction Protocol:** See [CONTRIBUTING.md](CONTRIBUTING.md)

When reporting, include:
1. Specific claim or rule in question
2. Evidence of error or ambiguity
3. Suggested correction or clarification

### Propose Framework Changes

The governance philosophy is fixed, but the framework evolves through evidence-based refinement. To propose changes:

- Email with: current rule, proposed modification, rationale, affected domains
- Example: "The Temporal Anchoring rule should be modified because [evidence]"
- Changes are reviewed on merit; philosophical integrity is maintained

---

## Licensing

This work is licensed under **CC BY 4.0** (Creative Commons Attribution 4.0 International).

**You are free to:**
- Share, copy, and redistribute this framework in any medium or format
- Adapt, remix, transform, and build upon this work for any purpose

**Under the condition that you:**
- Provide appropriate attribution to BordneAI
- Include a link to the license
- Indicate if modifications were made
- Do not add additional restrictions

See [LICENSE.md](LICENSE.md) for full terms.

---

## Status

**v3.3.1** — Released 2025-11-17
**Status:** Public specification, ready for deployment
**Maintenance:** Monitored for error correction and governance refinement

---

*The BordneAI Research Engine is a framework for evidence-based inquiry. It governs reasoning, not belief. Its purpose is clarity under uncertainty.*
