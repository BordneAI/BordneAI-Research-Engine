# BordneAI Research Engine v3.0-alpha

**A Universal, Governed Epistemic Framework for Evidence-Based Inquiry into Contested Domains**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Status: Alpha](https://img.shields.io/badge/Status-Alpha-yellow)]()
[![Framework: Universal](https://img.shields.io/badge/Framework-Universal-brightgreen)]()

---

## What is BordneAI Research Engine?

The BordneAI Research Engine is a **universal, governed epistemic framework** for evidence-based inquiry. It applies to contested domains across multiple disciplines—historical research, intelligence analysis, scientific anomalies, policy decisions, institutional analysis, and more.

This is not a domain-specific tool. Rather, it is a **governance system** that ensures rigorous, transparent reasoning about questions where evidence is incomplete, contested, or sealed. The framework prioritizes:

- **Verifiability**: All claims traceable to sources
- **Structural Secrecy Respect**: Distinction between sealed (legitimate) and conspiratorial (unanchored)
- **Competing Hypotheses**: No single narrative privileged without evidence

The engine is designed for researchers, analysts, policy makers, and knowledge workers who need to reason rigorously about contested questions while maintaining intellectual integrity.

---

## Core Principles

### 1. **Verifiability Through Tiered Sourcing**
Evidence is classified into four tiers (T1-T4), each with distinct confidence levels and handling rules:
- **T1**: Primary evidence, agency documents, official sources (highest confidence)
- **T2**: Peer-reviewed and preprint literature (high confidence)
- **T3**: Reputable secondary sources (medium confidence)
- **T4**: Direct testimony (lowest confidence; distinguished as T4_named with credentials or T4_anon)

Every claim maps to a source tier. No tier is privileged a priori; the tier assignment depends on the domain and question.

### 2. **Structural Secrecy Respect**
Sealed records are legitimate. The framework distinguishes:
- **Sealed**: Classified or protected by law; reasoning about what's sealed is possible using institutional incentives
- **Unknown**: Information we lack; absence of evidence is not evidence of absence
- **Conspiracy**: Unanchored suppression claims; requires explicit evidence, not assumption

Respecting this distinction prevents both naive trust in official narratives and descent into unfounded speculation.

### 3. **Competing Hypotheses Framework**
Contested domains have multiple credible interpretations of available evidence. The framework:
- Identifies all reasonable hypotheses consistent with the evidence base
- Assigns Bayesian weights based on T1-T4 sourcing
- Tracks confidence distributions rather than settling on a single narrative
- Updates weights as evidence accumulates

---

## How It Works

### The Sourcing Hierarchy
All analysis begins by classifying evidence:

1. **Gather Available Evidence** across all tiers (T1, T2, T3, T4)
2. **Classify by Tier** using explicit rules (is it peer-reviewed? official? testimony?)
3. **Map Conflict Resolution** when sources conflict (T1 > T2 > T3 > T4 by default, but context matters)
4. **Assign Entropy Levels** (L1-L5) indicating overall confidence:
   - L1-L2: Strong T1 baseline
   - L3: Mixed evidence (default for contested domains)
   - L4: Highly contested domains
   - L5: Refused (pure speculation; no clear T1/T2 evidence)

### The Guardrails
Seven universal guardrails prevent common reasoning errors:

1. **Temporal Anchoring**: Claims must specify *when* they apply
2. **No Unanchored Suppression**: "They're hiding X" requires evidence of suppression, not just absence of disclosure
3. **Competing Hypotheses**: Present all credible interpretations
4. **Language Precision**: Avoid hedging ("may," "could," "possibly") in favor of Bayesian weights
5. **Institutional Context Without Conspiracy**: Explain institutional behavior through incentives, not malice
6. **Physics/Logic Constraints**: If a hypothesis violates basic physics or logic, explicitly note it
7. **Sealed ≠ Unknown ≠ Conspiracy**: Treat these as distinct categories

### The Mandatory Analysis Structure
Every analysis follows this structure:

- **Header**: Entropy level, source tier mix, date analyzed
- **Verified Facts**: Only T1/T2 sources; explicitly flagged by tier
- **Analysis/Interpretation**: Separates fact from inference; shows reasoning
- **Testimony Attribution**: T4_named or T4_anon explicitly identified
- **Structural Secrecy Context**: What's sealed, what's unknown, what's conspiratorial
- **Competing Hypotheses**: Bayesian weights for credible interpretations
- **Next Steps**: What evidence would change the analysis

---

## Key Features

### ✓ Universal Application
Apply to any contested domain—no predefined categories. The framework is methodology, not substance.

### ✓ Transparent Governance
All analysis decisions are traceable. Show your work. Explain tier assignments, confidence weights, and reasoning.

### ✓ Institutional Literacy
Understand how institutions operate without assuming malice. Institutional incentives shape behavior; use them to reason about sealed records.

### ✓ Bayesian Reasoning
Confidence is distributed across hypotheses, not collapsed into binary true/false. Track uncertainty explicitly.

### ✓ Secure Against Common Errors
The seven guardrails catch reasoning failures at the source: hedging language, unanchored suppression claims, temporal drift, conspiracy thinking, etc.

### ✓ Domain-Agnostic
Same framework applies to historical research, intelligence analysis, scientific anomalies, policy decisions, institutional analysis, and beyond.

---

## Repository Structure

```
BordneAI-Research-Engine/
├── README.md                          # You are here
├── LICENSE.md                         # CC BY 4.0 license
├── NOTICE.md                          # Disclaimers and scope
├── CHANGELOG.md                       # Version history
│
├── SYSTEM_PROMPT-v3.0.md              # Full system instructions
├── SOURCING_PROFILE_V2.1.md           # Tiered sourcing specification
├── GOVERNANCE.md                      # Guardrails and governance
│
├── docs/
│   ├── framework.md                   # How to apply framework to any domain
│   ├── structural-secrecy.md          # Sealed records and uncertainty
│   └── examples.md                    # 5 generic methodology examples
│
├── prompts/
│   ├── research-engine-v3.0.md        # System prompt (copy)
│   └── menu-template.md               # Domain-agnostic guided menu
│
├── SECURITY.md                        # Responsible disclosure
└── CONTRIBUTING.md                    # Error reporting and feedback
```

---

## Quick Start

### For Researchers & Analysts
1. **Start here**: [SOURCING_PROFILE_V2.1.md](SOURCING_PROFILE_V2.1.md) — Understand the tier system
2. **Then read**: [docs/framework.md](docs/framework.md) — See how to apply it
3. **Study**: [docs/examples.md](docs/examples.md) — Learn through generic examples
4. **Reference**: [GOVERNANCE.md](GOVERNANCE.md) — Guardrails and correction protocols

### For Policy Makers & Decision-Makers
1. **Start here**: [README.md](README.md) (you are here) — Understand the principles
2. **Then read**: [docs/structural-secrecy.md](docs/structural-secrecy.md) — How to reason about sealed information
3. **Consult**: [docs/examples.md](docs/examples.md) — See methodology in action

### For Developers & Integration
1. **Start here**: [SYSTEM_PROMPT-v3.0.md](SYSTEM_PROMPT-v3.0.md) — Full system instructions
2. **Copy**: [prompts/research-engine-v3.0.md](prompts/research-engine-v3.0.md) or [prompts/menu-template.md](prompts/menu-template.md)
3. **Deploy**: Use in Claude API, ChatGPT, or other LLM interfaces

### For Newcomers
1. **Start here**: [README.md](README.md) (you are here)
2. **Read**: [docs/framework.md](docs/framework.md) — Five-step workflow
3. **Explore**: [docs/examples.md](docs/examples.md) — See it in practice
4. **Deep dive**: [SOURCING_PROFILE_V2.1.md](SOURCING_PROFILE_V2.1.md) for full sourcing rules

---

## Licensing

This work is licensed under a **Creative Commons Attribution 4.0 International License** ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)).

**You are free to:**
- Share and adapt this framework
- Use it for any purpose (commercial or noncommercial)

**You must:**
- Provide attribution (see [LICENSE.md](LICENSE.md) for requirements)
- Indicate if changes were made
- Include a copy of the license

---

## Deployment & Integration

This framework is available as a system prompt for use with:
- **ChatGPT** (through the system prompt feature)
- **Claude API** (through system context)
- **Other LLM Interfaces** (supporting system prompts)

**GPT Store Link**: [BordneAI Research Engine](https://chatgpt.com/gpts/BordneAI-Research-Engine-v3-0)

---

## Contact & Issues

**This is specification documentation only**—not software with executable code.

- **Bug reports or specification issues**: See [CONTRIBUTING.md](CONTRIBUTING.md)
- **Responsible disclosure**: See [SECURITY.md](SECURITY.md)
- **Content errors or feedback**: Follow the contribution process in [CONTRIBUTING.md](CONTRIBUTING.md)

---

## Version

**Current Version**: v3.0-alpha
**Last Updated**: 2025-11-17
**Status**: Specification complete; ready for alpha testing

See [CHANGELOG.md](CHANGELOG.md) for version history and updates.

---

**BordneAI Research Engine** — Rigorous reasoning about contested knowledge, universal framework, transparent governance.
