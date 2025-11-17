# Changelog

All notable changes to the BordneAI Research Engine are documented in this file.

---

## [3.0-alpha] - 2025-11-17

### First Release: Universal, Domain-Agnostic Framework

This is the first release of BordneAI Research Engine v3.0-alpha, a complete specification for evidence-based reasoning into contested domains.

#### Added

**Core Framework Components:**
- `SYSTEM_PROMPT-v3.0.md` - Complete system instructions for LLM deployment
- `SOURCING_PROFILE_V2.1.md` - Tiered sourcing hierarchy (T1-T4) with detailed definitions and citation standards
- `GOVERNANCE.md` - Seven universal guardrails and failure mode recovery procedures
- `README.md` - Framework overview and quick start guide

**Documentation:**
- `docs/framework.md` - Five-step methodology for applying framework to any domain
- `docs/structural-secrecy.md` - Framework for reasoning about sealed records and distinguishing from conspiracy claims
- `docs/examples.md` - Five generic methodology examples demonstrating framework application

**Templates & Deployment:**
- `prompts/research-engine-v3.0.md` - System prompt copy for direct LLM deployment
- `prompts/menu-template.md` - Domain-agnostic guided menu for users

**Governance & Licensing:**
- `LICENSE.md` - CC BY 4.0 license with attribution requirements
- `NOTICE.md` - Scope, limitations, and appropriate use cases
- `SECURITY.md` - Responsible disclosure and misuse scenarios
- `CONTRIBUTING.md` - Error reporting and feedback process

#### Key Features

**Universal Methodology:**
- Domain-agnostic framework applies to historical research, intelligence analysis, scientific disputes, policy analysis, and any contested domain
- Same methodology, sourcing hierarchy, and guardrails across all domains

**Evidence-Based Reasoning:**
- T1-T4 tiered sourcing hierarchy with explicit confidence levels
- Bayesian weighting of competing hypotheses
- Mandatory analysis structure ensuring transparency and reproducibility

**Governance Guardrails:**
1. Temporal Anchoring - All claims specify *when* they apply
2. No Unanchored Suppression - Suppression claims require explicit evidence
3. Competing Hypotheses - All credible interpretations presented
4. Language Precision - Explicit confidence levels instead of hedging
5. Institutional Context - Behavior explained through incentives, not conspiracy
6. Physics/Logic Constraints - Violations explicitly noted
7. Sealed ≠ Unknown ≠ Conspiracy - Three distinct categories

**Structural Secrecy Framework:**
- Legitimate reasoning about sealed records using institutional incentives
- Clear distinction between sealed (legitimate), unknown (natural gap), and conspiracy (unanchored)
- Refusal protocol for pure speculation

**Accessibility:**
- Clear documentation for researchers, analysts, policy makers, and developers
- Five-step workflow for applying framework to any question
- Generic examples (no incident-specific references)
- Guided menu for choosing research domain

---

## Planned Enhancements (Future Versions)

### Version 3.1 (Planned)
- Guardrail refinement based on alpha testing feedback
- Additional example types and application scenarios
- Expanded structural secrecy reasoning patterns
- Formal Bayesian model specification document

### Version 3.2 (Planned)
- Software implementation (Python or similar)
- LLM API integration examples
- Batch analysis capabilities
- Analysis quality validation tools

### Version 4.0 (Planned)
- Major restructuring based on deployment experience
- Domain-specific application guides (while maintaining universality)
- Advanced hypothesis generation methods
- Quantified guardrail violation detection

---

## Release Notes

### v3.0-alpha

**Status:** Specification complete; ready for deployment and testing

**Stability:** Stable specification; may receive clarifications and error corrections

**Deployment:**
- Ready for use as system prompt in Claude API, ChatGPT, and other LLM systems
- Suitable for research, educational, and professional analysis
- Not recommended for real-time emergency decision-making

**Known Limitations:**
- Framework is specification only; no software implementation
- Sealed records reasoning has inherent uncertainty (typically 30-50% confidence)
- Framework effectiveness depends on source tier classification accuracy
- Requires human judgment for question scoping and evidence evaluation

---

## Version Numbering

The BordneAI Research Engine uses semantic versioning:
- **Major version** (3, 4, etc.) - Fundamental framework restructuring
- **Minor version** (3.1, 3.2, etc.) - New features or significant improvements
- **Patch version** (3.0.1, 3.0.2, etc.) - Bug fixes and error corrections
- **Release status** (-alpha, -beta, none) - Maturity level

---

## Feedback & Contributions

For error reports, suggestions, and governance feedback, see CONTRIBUTING.md.

For security concerns, see SECURITY.md.

---

**BordneAI Research Engine v3.0-alpha**
Released 2025-11-17 under Creative Commons Attribution 4.0 International (CC BY 4.0)
