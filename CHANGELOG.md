# Changelog

All notable changes to the BordneAI Research Engine specification are documented here.

---

## [3.3.1] — 2025-11-17

### Major Release: Universal Framework Rebuild

This release represents a complete restructuring of the BordneAI Research Engine from v3.0-alpha to a universal, domain-agnostic framework.

#### What Changed

**Architecture:**
- ✅ Removed all domain-specific categories and predefined use cases
- ✅ Adopted Lightweight + Structured mode distinction based on entropy level
- ✅ Simplified entropy levels (L1-L5) with behavioral guidance
- ✅ Flattened response template (6 core sections)
- ✅ Strengthened suppression guardrails (explicit evidence requirement)
- ✅ Unified repository around v3.3.1 specification

**Documentation Overhaul:**
- ✅ **README.md:** Entry point explaining what engine is and quick start guide
- ✅ **SYSTEM_PROMPT-v3.3.1.md:** Canonical specification (1/1 source of truth)
- ✅ **docs/framework.md:** Universal application guide for any domain
- ✅ **docs/examples.md:** 7 generic methodology examples (no real incidents)
- ✅ **docs/governance.md:** Four core principles + self-check protocol
- ✅ **prompts/research-engine-v3.3.1.md:** Canonical prompt copy
- ✅ **prompts/lightweight-template.md:** Guidance for informal mode
- ✅ **NOTICE.md:** Scope, limitations, and appropriate usage
- ✅ **SECURITY.md:** Responsible disclosure for specification
- ✅ **CONTRIBUTING.md:** Error reporting and feedback process
- ✅ **CHANGELOG.md:** Version history (this file)

#### Key Principles (Unchanged)

The four core commitments remain fixed:
1. Prioritize documents over narratives
2. Separate what is known from what is claimed
3. Make uncertainties explicit
4. Distinguish absence of evidence from evidence of suppression

#### Four Governance Rules (Refined)

**Rule 1: Temporal Anchoring**
- Time-sensitive claims require explicit dates
- Enables fact-checking and correction
- Exceptions: timeless claims (math proofs, permanent laws)

**Rule 2: Conflict Resolution (BAAM Weighting)**
- Tier priority: T1 > T2 > T3 > T4_named > T4_anon
- Describes disagreement rather than hiding conflict
- Proportional confidence assignment

**Rule 3: Suppression & Hidden Information**
- May discuss institutional incentives for secrecy
- Cannot assert suppression without T1/T2 evidence
- Absence of evidence is not evidence of suppression

**Rule 4: Self-Check Protocol**
- Overconfidence scan before finalizing
- Tier compliance verification
- High-stakes domain identification
- Structural context and limitations documented

#### Tier System (Clarified)

**T1: Primary / Official / Direct**
- Original documents, official records, raw data
- Confidence: High to Extremely High (adjust for scope/age/methodology limits)

**T2: Scholarly / Authoritative Technical**
- Peer-reviewed research, official technical docs
- Confidence: High (adjust for recency/consensus/methodology)

**T3: Reputable Secondary**
- Quality journalism, textbooks, whitepapers
- Confidence: Medium (adjust for citation quality/alignment with T1/T2)

**T4: Testimony / Opinion**
- T4_named (experts with credentials): Low to Medium
- T4_anon (anonymous posts, hearsay): Low

#### Entropy Levels (Simplified)

- **L1:** Low entropy (simple, clear, well-documented)
- **L2:** Low-medium entropy (mostly clear, some nuance)
- **L3:** Moderate entropy (mixed evidence, some gaps)
- **L4:** High entropy (contested, significant disagreement)
- **L5:** Very high entropy (insufficient evidence, unknowns dominate)

Each level determines response structure and governance rigor.

#### Lightweight vs. Structured Mode

- **Lightweight:** Low-stakes, L1-L2, minimal structure, implicit sourcing
- **Structured:** High-stakes or L3+, full template, explicit tier attribution, governance compliance

Rule: When in doubt, choose Structured Mode.

#### Response Template (Structured Mode)

```
🧪 Header (entropy, size, mode, source mix, confidence, date)
✅ Verified Facts (T1/T2 only)
🔍 Analysis / Interpretations (inferences, labeled as analysis)
🌀 Testimony & Experiential Input (T3/T4 with attribution)
⚠️ Structural Context / Limitations (gaps, unknowns, time-sensitivity)
🛠️ Next Steps (what would change confidence, professional consultation)
```

#### What Was Removed

- ❌ SYSTEM_PROMPT-v3.0.md (replaced with v3.3.1)
- ❌ GOVERNANCE.md (refactored into docs/governance.md)
- ❌ SOURCING_PROFILE_V2.1.md (integrated into framework.md)
- ❌ docs/structural-secrecy.md (integrated into governance.md)
- ❌ docs/domains.md (eliminated; framework is universal)
- ❌ docs/examples.md (replaced with generic examples)
- ❌ prompts/menu-template.md (replaced with lightweight-template.md)
- ❌ prompts/research-engine-v3.0.md (replaced with v3.3.1 copy)
- ❌ Old NOTICE.md, SECURITY.md, CONTRIBUTING.md (rebuilt)

#### Backward Compatibility

⚠️ **Breaking changes from v3.0-alpha:**
- Domain categories no longer exist; framework is universal
- Entropy levels redefined (L1-L5 vs. previous categorization)
- Response template simplified (6 sections vs. previous structure)
- Sourcing tier guidance updated (more universal examples)
- Governance rules clarified and refined

**Migration:** Implementations based on v3.0-alpha should review framework.md and governance.md for updated rules.

#### Testing & Validation

- ✅ All examples use generic hypothetical scenarios (no real incidents)
- ✅ All governance rules applied consistently across documentation
- ✅ All cross-references validated
- ✅ Tone consistent: direct, practical, universal, non-academic
- ✅ CC BY 4.0 licensing mentioned throughout

#### Repository Structure

```
BordneAI-Research-Engine/
├── README.md                          (entry point, quick start)
├── LICENSE.md                         (CC BY 4.0)
├── NOTICE.md                          (limitations, scope, disclaimers)
├── SECURITY.md                        (responsible disclosure)
├── CONTRIBUTING.md                    (feedback & reporting)
├── CHANGELOG.md                       (this file)
├── SYSTEM_PROMPT-v3.3.1.md           (canonical specification)
├── .gitignore                         (git configuration)
├── docs/
│   ├── framework.md                   (universal application guide)
│   ├── examples.md                    (7 methodology examples)
│   └── governance.md                  (4 principles + self-check)
└── prompts/
    ├── research-engine-v3.3.1.md      (canonical prompt copy)
    └── lightweight-template.md         (lightweight mode guidance)
```

#### Future Maintenance

- Framework principles are stable (Core Commitment, 4 Governance Rules)
- Documentation will be refined for clarity based on feedback
- New examples may be added to demonstrate applications
- Tier and entropy guidance may be refined with user feedback
- Bug reports and error corrections will be addressed promptly

#### License

All content licensed under **CC BY 4.0** (Creative Commons Attribution 4.0 International).

---

## [3.0-alpha] — Previous Release (Deprecated)

**Status:** Deprecated. Not recommended for new use. Archive only.

**Changes from v2.1:**
- Introduced domain-specific categories (now removed in v3.3.1)
- Added sourcing profiles (consolidated into framework)
- Refined entropy levels (subsequently simplified in v3.3.1)

---

## [2.1] — Legacy (Archive Only)

**Status:** Historical reference. Not maintained.

---

## How to Report Errors

Found an error in this changelog or the specification?

- **GitHub Issues:** [github.com/BordneAI/BordneAI-Research-Engine/issues](https://github.com/BordneAI/BordneAI-Research-Engine/issues)
- **Email:** research@bordne.com

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed reporting guidelines.

---

## Version Numbering

BordneAI Research Engine uses semantic versioning (MAJOR.MINOR.PATCH):

- **MAJOR:** Significant governance rule changes or architecture overhaul
- **MINOR:** New features, substantial refinements, or major documentation updates
- **PATCH:** Bug fixes, clarity improvements, minor corrections

---

*BordneAI Research Engine | Changelog | Last Updated 2025-11-17*
