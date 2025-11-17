# CHANGELOG

All changes to the BordneAI Research Engine are tracked here for auditability and transparency, consistent with the verifiability principle.

---

## [v3.0-alpha] — 2025-11-17

### Initial Public Release

This is the first public release of the BordneAI Research Engine governance specification.

#### Summary
Complete reference documentation for the governance framework, sourcing hierarchy, and operational guidelines for the BordneAI GPT research assistant. Specification-only; no executable code included.

#### Added

**Core Governance Files:**
- `SYSTEM_PROMPT-v3.0.md` — Canonical system instructions and prompt configuration
- `SOURCING_PROFILE_V2.1.md` — Tiered evidence hierarchy (T1–T4) with conflict resolution rules
- `GOVERNANCE.md` — Domain-specific rules, safety guardrails, and correction protocols

**Documentation & Examples:**
- `docs/domains.md` — Per-domain methodology deep dives:
  - Nuclear history & NC3 secrecy treatment
  - Intelligence oversight and institutional analysis
  - UAP/UFO/USO sensor data and physics constraints
  - Scientific/historical anomalies and competing hypotheses
- `docs/structural-secrecy.md` — Framework for respecting institutional secrecy without speculation
- `docs/examples.md` — Five representative query/response pairs demonstrating governance in action

**Reference & Licensing:**
- `README.md` — High-level overview, quick-start guide, and repository structure
- `LICENSE.md` — CC BY 4.0 legal text and attribution requirements
- `NOTICE.md` — Operational safety disclaimers and usage guidance
- `CHANGELOG.md` — This file; version history and audit trail

**Optional Administrative Files:**
- `SECURITY.md` — Vulnerability reporting and misuse guidance
- `CONTRIBUTING.md` — External feedback and governance update procedures
- `prompts/research-engine-v3.0.md` — System prompt copy for experimentation
- `prompts/menu-template.md` — Guided menu structure for interactive mode

#### Configuration

**Enabled Domains (Core 4):**
- `nuclear_history_Okinawa` — Nuclear near-misses, NC3 protocols, declassified incidents
- `politics_intel_elections` — Oversight records, FOIA releases, intelligence assessments
- `uap_ufo_usos` — UAP kinematics, sensor data, physics constraints
- `3i_atlas_core` — [Scope per implementation]

**Key Features:**
- Tiered sourcing with T1 (Primary/Agency), T2 (Peer-Reviewed), T3 (Secondary), T4 (Testimony) hierarchy
- Temporal anchoring requirement: all factual claims tied to specific documents or dates
- Entropy control and BAAM weighting for uncertainty quantification
- Structural secrecy respect: distinction between "sealed (unknown)" and "declassified (unresolved)"
- Competing hypotheses framework with confidence distribution
- David Bordne as T4_named researcher; T4 contributions always flagged
- Domain-specific disallowed claims and guardrails

**Governance Principles:**
- Verifiability First: sources citable, claims checkable
- Structural Secrecy Respect: institutional sealing is legitimate, not conspiracy
- Competing Hypotheses Valued: uncertainty quantified, not hedged
- Correction protocol: user flagging, developer feedback integration

**Safety Gates:**
- Refusal of unanchored suppression claims ("hidden docs definitely exist")
- Physics plausibility checks (UAP domain)
- Neutral language enforcement (contested domains: politics, intelligence, UAP)
- Temporal anchoring verification
- T4 testimony isolation (never sufficient alone)

#### Documentation Completeness

- README serves as entry point with repository structure diagram
- All 16+ files per specification completed
- Cross-references validated
- Tone consistency verified (professional, neutral, specification-forward)
- Examples span all enabled domains
- Readability tested for multiple audiences

#### License

- CC BY 4.0 with explicit attribution requirement
- Applicable to governance content only (no executable code)
- Derivative works permitted with attribution and disclaimer

#### Known Limitations

- `3i_atlas_core` scope to be defined per implementation
- Entropy levels and BAAM weighting parameters marked as [specify] in SYSTEM_PROMPT-v3.0.md
- GPT Store deployment URL placeholder ([GPT_STORE_URL])
- Contact email placeholder (BordneAI@bordne.com — verify during publication)

---

## Versioning & Future Updates

### Version Bump Triggers

The following events will trigger a version update:

1. **Prompt Modifications:** Changes to SYSTEM_PROMPT-v3.0.md logic, disallowed claims, or guardrails
2. **New Domains:** Addition or removal of enabled research domains
3. **Safety Gate Changes:** Significant modifications to governance rules or correction procedures
4. **Sourcing Rules:** Updates to tiered hierarchy, conflict resolution, or T4 testimony protocols
5. **Documentation Clarification:** Substantial rewrites or corrections affecting interpretation

Minor clarifications or typo corrections will not trigger version bumps but will be noted in this file.

### Version Numbering Scheme

- **Major (X.0):** Fundamental changes to core governance or domain structure
- **Minor (3.Y):** New features, domains, or significant documentation additions
- **Alpha/Beta:** Pre-release versions (e.g., v3.0-alpha, v3.1-beta)
- **Release:** Stable, production-recommended versions

### Update Process

1. Changes proposed and documented
2. CHANGELOG.md entry drafted with proposed changes
3. Safety and consistency review performed
4. SYSTEM_PROMPT-v3.0.md updated if applicable
5. All related files (GOVERNANCE.md, docs/) updated for consistency
6. New version committed with descriptive message
7. CHANGELOG.md finalized with version number and date
8. Release announced via GitHub and documentation

### Template for Future Versions

```markdown
## [vX.Y-stage] — YYYY-MM-DD

### Release Title

Brief summary of major changes.

#### Added
- [New features, domains, files]

#### Changed
- [Modified files, rule updates]

#### Fixed
- [Corrections, clarifications]

#### Known Issues
- [Limitations, placeholders]

#### Migration Notes (if applicable)
- [Instructions for adapting prior implementations]
```

---

## Feedback & Error Reporting

To report errors, request clarifications, or propose improvements:

1. **GitHub Issues:** [https://github.com/BordneAI/BordneAI-Research-Engine/issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)
2. **Email:** BordneAI@bordne.com
3. **Correction Protocol:** See GOVERNANCE.md for formal correction submission procedure

Issues will be reviewed and prioritized. Accepted corrections will be incorporated in the next version bump.

---

## Audit & Verifiability

This CHANGELOG serves as an audit trail for the BordneAI Research Engine specification. All changes are documented here, enabling:

- **Transparency:** Users can see what has changed and when
- **Accountability:** Attribution of changes to development phases
- **Reproducibility:** Earlier versions are identifiable for comparison
- **Trust:** Version consistency verifiable across deployments

The git commit history (visible via `git log`) provides the underlying verification mechanism.

---

**Last Updated:** 2025-11-17
**Current Version:** v3.0-alpha
**Maintained By:** David Bordne
**License:** CC BY 4.0
