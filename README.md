# BordneAI Research Engine v3.0-alpha

## Overview

The BordneAI Research Engine is a governance specification and reference architecture for evidence-based inquiry into historically complex, institutionally sensitive domains. This repository documents the operational framework, sourcing hierarchy, and safety guardrails for the BordneAI GPT—a specialized research assistant designed to reason about declassified material, institutional secrecy, and competing hypotheses in evidence evaluation.

**This is a specification-only repository.** No executable code, model weights, or proprietary runtime logic is included. It is designed for transparency, auditability, and public release under Creative Commons BY 4.0 (CC BY 4.0) license.

## Core Principles

The BordneAI Research Engine operates on three foundational principles:

1. **Verifiability First:** All factual claims are anchored to sources (declassified documents, peer-reviewed research, institutional records) and enabled for independent verification. Speculation is labeled as such; uncertainty is quantified rather than hedged.

2. **Structural Secrecy Respect:** The system acknowledges that institutional secrecy—particularly in military and intelligence contexts—is often legitimate and normative. Sealed records are treated as "don't know" rather than "conspiracy;" the system quantifies what remains unknown without assuming hidden content.

3. **Competing Hypotheses Valued:** Uncertainty is not a failure. When evidence supports multiple competing explanations, all are presented with confidence distributions and reasoning made transparent.

## Enabled Research Domains

The current system (v3.0-alpha) is fully enabled for four core domains:

- **nuclear_history_Okinawa:** Nuclear near-misses, declassified incidents, NC3 (Nuclear Command & Control & Communications) protocols, weapons history, and associated institutional secrecy norms.

- **politics_intel_elections:** Oversight records, declassified intelligence assessments, Congressional testimonies, FOIA releases, and institutional analysis of electoral and intelligence processes.

- **uap_ufo_usos:** Unidentified Aerial Phenomena, declassified sensor data, kinematics analysis, physics plausibility constraints, and official incident documentation.

- **3i_atlas_core:** Astronomy and astrophysics analysis; enforces T1-prioritized sourcing (NASA-JPL, peer-reviewed journals) for celestial phenomena with rigorous physics constraints.

Each domain has dedicated safety guardrails, mandatory citation standards, and domain-specific reasoning constraints documented in GOVERNANCE.md.

## Tiered Sourcing & Governance Model

Evidence evaluation follows a four-tier hierarchy:

- **T1 (Primary/Agency/Official):** Declassified documents, official statements, archival records, peer-reviewed primary sources. Highest confidence.
- **T2 (Peer-Reviewed & Preprint):** Published research, vetted journals, institutional analyses. Medium confidence.
- **T3 (Reputable Secondary):** Historical syntheses, investigative journalism, established commentaries. Medium-Low confidence.
- **T4 (Testimony):** Named researchers (T4_named, including David Bordne) and anonymous accounts (T4_anon, lowest confidence). Used to identify gaps; never sufficient alone.

Conflicts between tiers are resolved via explicit reasoning; higher tiers override lower unless accompanied by stronger evidence. Full details in SOURCING_PROFILE_V2.1.md.

## Entropy Levels & Uncertainty Quantification

The system manages uncertainty through:

- **Entropy control:** Default entropy level L3 (mixed evidence, elevated uncertainty); escalates to L4 for contested domains; refuses L5 speculation.
- **BAAM weighting:** Bayesian auxiliary analysis model for confidence distribution across competing hypotheses.
- **Temporal anchoring:** All factual claims tied to specific documents, dates, or declassification events.
- **Quantified uncertainty:** Confidence ranges (e.g., "70% likely X, 20% Y, 10% Z") replace hedged language.

See SYSTEM_PROMPT-v3.0.md for full specification.

## How to Use This Repository

### For Researchers & Analysts
This repository serves as a reference specification for evidence-based inquiry in sensitive domains. Use SOURCING_PROFILE_V2.1.md as a standalone sourcing guide; consult docs/domains.md for per-domain methodologies; review docs/examples.md to see governance in action.

### For Policy Makers & Oversight Bodies
Review GOVERNANCE.md to understand domain-specific safety rules and disallowed claims. NOTICE.md clarifies what this system is and is not. docs/structural-secrecy.md explains how the system respects institutional secrecy without speculating about hidden content.

### For GPT Users
Access the live GPT deployment at https://chatgpt.com/g/g-6917fec50494819197debd06e289bd42-bordneai-research-engine for interactive queries. All responses are governed by rules documented here. To flag errors or misalignment, use the correction protocol defined in GOVERNANCE.md.

### For Developers & Architects
SYSTEM_PROMPT-v3.0.md is the canonical system instruction set—single source of truth for prompt configuration. prompts/research-engine-v3.0.md provides a copy for experimentation. See CONTRIBUTING.md for governance update procedures.

## Repository Structure

```
BordneAI-Research-Engine/
├── README.md                          (this file)
├── LICENSE.md                         (CC BY 4.0 legal text & attribution)
├── NOTICE.md                          (operational safety notice)
├── CHANGELOG.md                       (version history & audit trail)
├── SYSTEM_PROMPT-v3.0.md             (canonical system instructions)
├── SOURCING_PROFILE_V2.1.md          (tiered evidence hierarchy)
├── GOVERNANCE.md                      (domain rules & safety guardrails)
├── SECURITY.md                        (optional; vulnerability & misuse reporting)
├── CONTRIBUTING.md                    (optional; external contribution guidance)
├── docs/
│   ├── domains.md                     (per-domain deep dives)
│   ├── structural-secrecy.md          (how system reasons about classified material)
│   └── examples.md                    (5 representative query/response pairs)
└── prompts/
    ├── research-engine-v3.0.md        (system prompt copy/variant)
    └── menu-template.md               (guided menu structure)
```

## Key Documents at a Glance

| Document | Purpose | Audience |
|----------|---------|----------|
| [SYSTEM_PROMPT-v3.0.md](SYSTEM_PROMPT-v3.0.md) | Canonical system instructions; single source of truth | Developers, operators |
| [SOURCING_PROFILE_V2.1.md](SOURCING_PROFILE_V2.1.md) | Tiered evidence hierarchy; standalone sourcing guide | Researchers, analysts |
| [GOVERNANCE.md](GOVERNANCE.md) | Domain-specific rules, safety gates, correction protocol | Policy makers, users, developers |
| [docs/domains.md](docs/domains.md) | Per-domain methodology & case studies | Domain specialists |
| [docs/structural-secrecy.md](docs/structural-secrecy.md) | How system respects institutional secrecy | Policy makers, oversight |
| [docs/examples.md](docs/examples.md) | 5 real/representative governance examples | All audiences |

## BordneAI EOS Philosophy

This research engine operationalizes principles from the broader BordneAI Epistemological Operating System (EOS):

- **Verifiability as epistemological foundation:** Claims must be checkable, sources must be citable.
- **Institutional incentives acknowledged:** Why records are sealed; what that reveals about institutional behavior.
- **Uncertainty as epistemic honesty:** Better to say "we don't know" than speculate.
- **Competing explanations as intellectual rigor:** Not all hypotheses have equal evidence, but multiple can coexist.

See GOVERNANCE.md for operationalization details.

## Licensing & Attribution

This repository is released under **Creative Commons Attribution 4.0 International (CC BY 4.0)**.

**Attribution Required:**
> BordneAI Research Engine by David Bordne, licensed under CC BY 4.0

For full legal text and attribution requirements, see [LICENSE.md](LICENSE.md).

This license covers the instructional and governance content. No executable runtime, model weights, or proprietary logic is included in this repository.

## Live Deployment

The BordneAI Research Engine GPT is deployed on the OpenAI GPT Store:

**https://chatgpt.com/g/g-6917fec50494819197debd06e289bd42-bordneai-research-engine**

## Feedback & Issue Reporting

- **For BordneAI architecture feedback:** Contact BordneAI@bordne.com
- **For GitHub issue tracking:** Report via [GitHub Issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)
- **For prompt misalignment or errors:** Use correction protocol in GOVERNANCE.md

## Version & Change Tracking

Current version: **v3.0-alpha**

All changes, domain additions, and governance updates are tracked in [CHANGELOG.md](CHANGELOG.md) for verifiability and transparency. Significant updates are announced there and reflected in SYSTEM_PROMPT version headers.

## What This Repository Is NOT

- **Not executable code:** No runtime logic, no model weights, no algorithms to execute.
- **Not production-certified:** Not safety-approved for critical infrastructure or high-stakes adversarial contexts.
- **Not a conspiracy framework:** This system respects institutional secrecy; it does not assume hidden content.
- **Not open-source for contributions:** External PRs are not accepted. This is a reference specification maintained by the BordneAI team.

See [NOTICE.md](NOTICE.md) for full safety disclaimers.

## Quick Start

1. **New to BordneAI?** Start with this README and [GOVERNANCE.md](GOVERNANCE.md).
2. **Need sourcing guidance?** Read [SOURCING_PROFILE_V2.1.md](SOURCING_PROFILE_V2.1.md).
3. **Want examples?** See [docs/examples.md](docs/examples.md) for representative queries and governance checkpoints.
4. **Curious about a specific domain?** Consult [docs/domains.md](docs/domains.md).
5. **Questions about sealed records?** Review [docs/structural-secrecy.md](docs/structural-secrecy.md).

---

**Repository Status:** Public Release (v3.0-alpha)
**License:** CC BY 4.0
**Maintenance:** Governed by David Bordne; version updates tracked in CHANGELOG.md
**Last Updated:** 2025-11-17
