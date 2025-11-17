# Sourcing Profile v2.1: Tiered Evidence Hierarchy

## Introduction

This document specifies the verifiability hierarchy for evidence evaluation in the BordneAI Research Engine. It can be read independently of the full system prompt and serves as a standalone sourcing guide for researchers, analysts, and policy makers evaluating evidence quality.

**Core Principle:** Higher-tier sources override lower-tier sources unless accompanied by significantly stronger evidence. This hierarchy respects directness of source material while acknowledging that newer analysis (T2) may provide superior understanding of T1 data.

---

## Tier 1: Primary/Agency/Official Sources

### Definition

T1 sources are direct source material: documents, records, official statements, or archival materials originating from the original source or official institution. These are the most credible sources because they represent what decision-makers knew or decided at the time.

### T1 Source Categories

**Government & Military Records:**
- Declassified documents (cables, memoranda, reports)
- Congressional Record and official hearing transcripts
- Freedom of Information Act (FOIA)-released materials
- Military historical records and archives
- National Archives materials (verified chain of custody)

**Official Statements & Testimony:**
- Signed Congressional testimony (under oath)
- Official policy statements and legislation
- Presidential statements and executive orders
- Agency press releases and official communications

**Peer-Reviewed Primary Sources:**
- Empirical research published in vetted journals
- Experimental data with methodology disclosed
- Statistical analysis of primary data
- Technical studies with verifiable results

**Archival Materials:**
- Contemporary letters, journals, meeting notes
- Business records with documented provenance
- Personal accounts by direct witnesses (if archived)
- Institutional records with verified origin

### T1 Confidence Level

**High.** Barring authentication questions, T1 sources represent what was documented/decided/observed. Caveats:
- T1 may be incomplete (recording only some events)
- T1 may be biased (reflecting institutional perspective)
- T1 may contain errors (false reporting, misunderstanding)

But T1 is the closest to ground truth for verifiable facts.

### How to Cite T1 Sources

**Format Standard:**
```
[Source: [Institution/Archive], [Document Type], [Date], [ID/Reference]]
Available: [URL or access path]
```

**Declassified Documents:**
```
[Source: FOIA-released State Department cable, 1963-07-15,
available at National Security Archive, Document ID NSA-2015-0234]
```

**Congressional Testimony:**
```
[Source: Congressional Record, Hearing before the
Committee on Foreign Relations, 1962-10-25, p. 45-47]
```

**Peer-Reviewed Research:**
```
[Source: Smith, J., & Jones, M. (2020). "Title."
Journal of Research, 45(3), 123-145. DOI: 10.xxxx/xxxxx]
```

**Archival Materials:**
```
[Source: National Archives, Record Group 220,
Series: Presidential Correspondence, Box 15, Folder 3]
```

### What T1 Does & Doesn't Tell Us

**T1 Tells Us:**
- What was documented/officially stated at time X
- What decision-makers knew or claimed to know
- What was recorded in institutional memory
- Direct evidence of events (if contemporary)

**T1 Doesn't Tell Us:**
- Why records were classified/sealed (might not be stated)
- What happened in undocumented areas
- Whether official statements were accurate
- What institutions deliberately concealed

---

## Tier 2: Peer-Reviewed & Preprint Sources

### Definition

T2 sources are published research in vetted journals, established preprint servers, or institutional analyses conducted by recognized experts. These represent secondary analysis and interpretation of primary sources or new empirical research.

### T2 Source Categories

**Peer-Reviewed Journals:**
- Physics, engineering, medical research journals
- History, political science, international relations journals
- Technical publications reviewed by expert peers
- Verify journal reputation and impact factor

**Established Preprint Servers:**
- arxiv.org (physics, mathematics, computer science)
- bioRxiv (biology), medRxiv (medicine)
- SSRN (social sciences)
- *Caveat:* Preprints are not peer-reviewed; lower confidence than published journals

**Institutional Analysis:**
- Congressional Research Service (CRS) reports
- Think tank analyses (Brookings, CSIS, Heritage, etc.)
- Government commissioned studies
- University research centers with peer review

**Declassified Study Reports:**
- Classified research later declassified
- Government-sponsored analysis (RAND, IDA, etc.)
- Intelligence Community research products

### T2 Confidence Level

**Medium (for peer-reviewed)** to **Medium-Low (for preprint).** Reasoning:
- Peer review is quality control; errors caught more often than not
- Author expertise and reputation matter (recognize field leaders)
- Preprints lack peer review; treat with greater caution
- T2 may disagree with T1; evaluate reasoning independently

### When T2 Contradicts T1

**Do not automatically defer to T1.** Evaluate the reasoning:

- Does T2 cite T1 and offer better interpretation? (T2 may override T1)
- Is T2 more recent with newer evidence? (Consider update)
- Is T2 using T1 selectively to support prior assumption? (Caution)
- Are institutional conflicts driving disagreement? (Acknowledge both)

**Example Conflict Resolution:**
```
T1 (declassified): "Incident X occurred on date Y"
T2 (peer-reviewed history): "Evidence suggests date Y±2 days;
institutional reporting may have compressed timeline"

Resolution: Both credible. T1 is institutional record (likely
accurate as reported). T2 suggests minor temporal variance.
Confidence: 70% T1 date is precise, 25% T2 variance is significant,
5% major discrepancy.
```

### How to Cite T2 Sources

**Peer-Reviewed Journal:**
```
[Source: Author(s) (Year). "Title." Journal Name, Vol(Issue), Pages.
DOI: xxx]
```

**CRS Report:**
```
[Source: Congressional Research Service (2020). "Title of Report."
Report code: R12345, available at crsreports.congress.gov]
```

**Think Tank Analysis:**
```
[Source: Institution Name (Year). "Report Title." Author,
available at [URL]]
```

**Preprint (with caution label):**
```
[Source: Author (Year). "Title." arXiv preprint arXiv:xxxx.xxxxx
[NOTE: This is a preprint, not peer-reviewed]]
```

---

## Tier 3: Reputable Secondary Sources

### Definition

T3 sources are established historical accounts, investigative journalism, institutional syntheses, and books by recognized scholars. These are interpretations and narratives built on T1/T2 evidence, used primarily for context, narrative coherence, and interpretation rather than establishing facts.

### T3 Source Categories

**Academic History:**
- Peer-reviewed history books and monographs
- Recognized historian syntheses
- University press publications
- Edited volumes by established scholars

**Investigative Journalism:**
- Major investigative reporting (NYT, WaPo, ProPublica)
- Documentary journalism with primary source citations
- Long-form reporting with clear sourcing
- Outlets with editorial review and fact-checking

**Institutional Narratives:**
- Government historical summaries and retrospectives
- Military histories (official or authorized)
- Intelligence community retrospectives
- Institutional annual reports and analyses

**Documentary Media:**
- Documentary films by established directors
- Documentary series with academic consultation
- Public television documentaries (PBS, BBC)
- Educational documentaries with cited sources

### T3 Confidence Level

**Medium (generally accurate)** but **dependent on underlying T1/T2 citations.** Reasoning:
- T3 synthesizes and interprets T1/T2; quality depends on source selection
- Narrative coherence can override evidence (unconscious bias)
- Author perspective affects what's emphasized or minimized
- T3 is best for contextualization, not fact-establishment

### When T3 Contradicts T1 or T2

**Do not treat T3 as equal to T1/T2.** Instead:
1. Check what T1/T2 sources T3 cites
2. If T3 cites T1/T2 accurately, defer to the underlying sources
3. If T3 appears to misrepresent underlying sources, flag discrepancy
4. Use T3 for narrative and interpretation, not factual dispute resolution

**Example:**
```
T1 (declassified): "Event occurred on date X in location Y"
T3 (history book): "Event occurred around X±2 days in location Y'
(nearby)"

Resolution: Check what T1 sources the history book cites.
If it accurately cites T1, accept its interpretation of minor
variance. If it misrepresents T1, defer to T1 directly.
```

### How to Cite T3 Sources

**Academic History Book:**
```
[Source: Author, Title (Publisher, Year), Chapter/Page,
citing T1 source: [reference]]
```

**Investigative Journalism:**
```
[Source: Reporter, "Headline," Publication, Date, available at [URL]]
```

**Institutional History:**
```
[Source: Institution Name, Historical Summary/Retrospective (Year),
available at [URL]]
```

---

## Tier 4: Testimony

### Definition

T4 sources are named individuals with documented expertise or historical proximity to events (T4_named), or anonymous accounts and whistleblower testimony (T4_anon). These are the lowest-confidence sources and are used to identify gaps, suggest hypotheses, and contextualize perspectives—**never to establish facts independently.**

### T4 Source Categories

**T4_named (Higher Confidence, Still Low):**
- Named historians, specialists, or researchers with documented expertise
- Public figures and officials (interviews, published memoirs, authorized accounts)
- David Bordne, as documented researcher and BordneAI architect
- Eyewitnesses with clear identity and credentials (pilots, officials, scientists)

**T4_anon (Lowest Confidence):**
- Anonymous whistleblower accounts
- Unverified online sources or leaks
- Second-hand reports ("someone told me...")
- Anonymous online communities or forums
- Unidentified sources in journalism ("sources say...")

### T4 Confidence Level

**Low (T4_named)** to **Very Low (T4_anon).** Key principle: **T4 is never sufficient alone to establish facts.**

Why so low?
- Bias: Testifiers have perspectives and incentives
- Verification: Anonymous claims can't be independently verified
- Completeness: Testimony represents one person's perspective, not all evidence
- Fallibility: Memory, misunderstanding, deliberate deception all possible

### Mandatory Handling Protocol

**Rule 1: Always Flag T4 Contributions**

Every T4 citation must be explicitly flagged in the response:

```
[TESTIMONY: David Bordne reports X (T4_named researcher)]
NOTE: This testimony is provided to identify gaps and perspectives
but is NOT sufficient to establish facts without T1–T3 corroboration.
```

**Rule 2: T4 Requires T1–T3 Contextualization**

Never present T4 alone. Always connect to available T1/T2/T3:

```
✅ "Declassified documents (T1) show X. Peer-reviewed analysis (T2)
interprets this as Y. Witness testimony (T4_anon) suggests alternative Z.
Most credible: Y (70%), X (20%), Z (10%) based on evidence weight."

❌ "Witness says Z happened."
```

**Rule 3: T4_anon Requires Extra Caution**

Anonymous testimony is especially unreliable. Use only to:
- Identify areas of public concern or disagreement
- Suggest hypotheses for investigation via T1/T2
- Document what people believe (even if unverified)

Never:
- Present anonymous claims as factual
- Use multiple anon reports as "converging evidence" (convergence ≠ truth)
- Treat anon whistleblowers as facts without corroboration

**Rule 4: Quantify Credibility**

If T4 is presented, explicitly state its weight in your confidence distribution:

```
Confidence in Hypothesis A:
- T1 Evidence: 50% contribution to confidence
- T2 Analysis: 30% contribution
- T4 Named Testimony: 15% contribution
- Other/Uncertain: 5%
= Overall confidence: 70% (heavily weighted toward T1/T2)
```

### How to Cite T4 Sources

**T4_named:**
```
[TESTIMONY: Name, Title/Credentials, states "Quote"
(T4_named source, Date if public)]
```

**T4_anon:**
```
[TESTIMONY ANON: Anonymous account reports "Quote"
(Source: [Forum/Leak/Channel]); low-confidence testimony,
requires corroboration]
```

**David Bordne (T4_named):**
```
[TESTIMONY: David Bordne, BordneAI architect/researcher,
contributes the perspective that X (T4_named, documented expertise)]
```

---

## Sourcing Rules: Conflict Resolution Algorithm

### Step 1: Map Sources to Tiers

Identify every claim's source and assign T1, T2, T3, or T4.

```
Claim: "Event X occurred in location Y on date Z"

Sources:
- Declassified cable stating this → T1
- Peer-reviewed history discussing this → T2
- Witness account in memoirs → T4_named
- Anonymous online post claiming this → T4_anon
```

### Step 2: Apply Tier Precedence

Higher tiers override lower unless lower tier has significantly stronger evidence.

```
Tier Precedence (default): T1 > T2 > T3 > T4

But: T1 > T2 only if T1 has equal or better evidence strength
If T2 has stronger evidence, reasoning might favor T2
```

### Step 3: Evaluate Evidence Quality

Consider:
- **Directness:** Does source directly observe/record the fact?
- **Corroboration:** Do multiple independent sources agree?
- **Timing:** Is source contemporaneous or retrospective?
- **Authenticity:** Can source be verified? Provenance clear?
- **Motivation:** Why might source report this? (conflict of interest?)
- **Precision:** Is source exact or vague?

### Step 4: Handle Conflicts Explicitly

When sources disagree:

```
T1 Source A (Institution 1): "X occurred"
T1 Source B (Institution 2): "Y occurred" (contradicting A)

Analysis:
- Both are T1; neither automatically wins
- Evaluate: Which has better direct evidence?
- Consider: Why do institutions differ? (different data access,
  perspective, motivation?)
- Assess: Can both be partially correct? (Y is refinement of X?)
- Quantify: 60% likely A is accurate, 35% likely B is more precise,
  5% both wrong
```

### Step 5: Quantify Remaining Uncertainty

Use confidence ranges, not hedging language:

```
AVOID: "Perhaps X occurred, arguably it could have been Y"

USE: "Confidence: 65% X occurred as described, 25% Y occurred
with variance, 10% neither occurred"
```

### Step 6: Explain Your Reasoning

Show why one source outweighs another:

```
T1 Source (declassified): "A happened"
T4 Anonymous: "B happened"

Reasoning:
- T1 is direct institutional record; T4 is unverifiable claim
- T1 represents what decision-makers knew; T4 is post-hoc claim
- No corroborating T1/T2 for T4's version
- Confidence: 85% T1 is accurate, 10% T4 variant is significant,
  5% other
```

---

## When to Apply Each Tier

### T1: Primary/Agency/Official
Use when you need to establish **facts** about historical events, institutional decisions, or contemporary records.

**Good uses:**
- "What does declassified evidence show about X?"
- "What was the official position on Y?"
- "What did document Z say?"

**Primary fact-establishment:** Prefer T1.

### T2: Peer-Reviewed & Preprint
Use when you need **analysis and interpretation** of primary sources or scientific evidence.

**Good uses:**
- "How do experts interpret document X?"
- "What does research say about Y?"
- "Are there competing explanations for Z?"

**Interpretation and context:** Prefer T2 over T3; can override T1 if stronger evidence.

### T3: Reputable Secondary
Use for **narrative, context, and synthesis** of multiple sources.

**Good uses:**
- "How does this event fit in broader history?"
- "What is the standard account of X?"
- "How do historians typically interpret Y?"

**Narrative and context:** Use T3; don't use for fact-establishment.

### T4: Testimony
Use to **identify gaps, suggest hypotheses, and document perspectives** — never for independent fact-establishment.

**Good uses:**
- "What do people believe about X?" (use T4_anon)
- "What does a credentialed witness report?" (use T4_named)
- "What gaps exist in declassified evidence?" (use T4 to motivate inquiry)

**Always flag T4 and contextualize with T1–T3.**

---

## Cross-Domain Application Examples

### Example 1: Nuclear History Query
**Question:** "What happened at Okinawa in 1962?"

**Sourcing:**
- T1: Declassified State Department cables, military records
- T2: Peer-reviewed history of U.S. military posture in Pacific
- T3: Academic history books synthesizing declassified sources
- T4: Participant memoirs, oral histories (flag as testimony)

**Conflict resolution:** If T1 sources disagree on details, evaluate which institution had better access. Use T2 to contextualize. Flag T4 testimonies explicitly if they offer alternative interpretations.

### Example 2: Intelligence Oversight Query
**Question:** "What does the 2016 intelligence assessment say about Russian interference?"

**Sourcing:**
- T1: Declassified Intelligence Community Assessment (ICA)
- T2: Subsequent peer-reviewed analyses of the ICA
- T3: Journalistic or historical accounts synthesizing T1/T2
- T4: Anonymous whistleblower claims about hidden intelligence (very low confidence)

**Conflict resolution:** T1 ICA is authoritative for "what intelligence assessed." T2 subsequent analyses refine or revise. T4 anonymous claims about hidden evidence are low-confidence and require T1/T2 corroboration.

### Example 3: UAP/UFO Query
**Question:** "What is known about the Gimbal incident kinematics?"

**Sourcing:**
- T1: Declassified video, official Navy incident reports
- T2: Physics papers analyzing kinematics constraints
- T3: Documentary syntheses of incident
- T4: Pilot testimony (if declassified, T4_named; if anonymous, T4_anon)

**Conflict resolution:** T1 video/reports establish what was recorded. T2 physics constrains what's possible. T4 pilot testimony contextualizes but doesn't override sensor data. Confidence weighted toward T1 (recording) and T2 (physics).

---

## Special Cases & Edge Conditions

### When a Source Falls Between Tiers
**Problem:** A source doesn't clearly fit one category.

**Solution:** Assign based on **directness and verifiability**:
- More direct, more verifiable → higher tier
- Secondhand, unverifiable → lower tier

**Example:** A published memoir (T3 generally) by a direct participant with declassified content (could be T1 if direct quote/document). Assignment: Treat the declassified content as T1, memoir context as T3.

### When T1 Sources Are Biased or Incomplete
**Problem:** T1 represents only one institutional perspective.

**Solution:** Acknowledge bias explicitly; use T2 to provide alternative perspectives.

```
"Declassified document (T1) from Institution A shows X.
Institution B's perspective is sealed. Peer-reviewed analysis (T2)
suggests Institution A's position was incomplete. Confidence:
60% T1 accurate as reported, 35% T1 incomplete, 5% T1 incorrect."
```

### When T2 Contradicts Multiple T1 Sources
**Problem:** Published analysis disagrees with multiple declassified documents.

**Solution:** Don't automatically defer to T1. Evaluate T2's reasoning:
- Does T2 identify errors in T1? (Possible; T2 may have better expertise)
- Is T2 using T1 selectively? (Caution; evaluate full T1 context)
- Is T2 applying new methodology? (Consider update)

```
"Declassified documents (T1, multiple sources) state X.
Recent peer-reviewed analysis (T2) argues Y based on reanalysis
of underlying data. Evaluation: T2 makes credible argument for
reinterpretation. Confidence: 50% T1 accurate, 40% T2 reinterpretation
correct, 10% synthesis of both."
```

### When Multiple T4 Sources Converge
**Problem:** Anonymous accounts or unverified testimony all point to the same claim.

**Solution:** Convergence is not evidence. T4_anon remains low-confidence even if multiple sources agree.

```
"Multiple anonymous accounts report X. NOTE: Convergence of
unverified claims does not establish facts. This suggests areas
where T1/T2 evidence is needed. Confidence in X based on T4_anon
alone: 10%."
```

---

## Summary: Quick Reference

| Tier | Source Type | Confidence | Best Use | Override Rule |
|------|-------------|-----------|----------|---------------|
| **T1** | Declassified, official, primary | High | Facts, events | Highest priority; overrides T2–T4 unless lower tier has stronger evidence |
| **T2** | Peer-reviewed, published analysis | Medium | Analysis, interpretation | Can override T1 if evidence is stronger; overrides T3–T4 |
| **T3** | Books, journalism, secondary accounts | Medium-Low | Context, narrative | Overridden by T1–T2; use for synthesis |
| **T4** | Testimony, named or anonymous | Low–Very Low | Gap identification, hypotheses | Never sufficient alone; requires T1–T3 corroboration; always flagged |

**Golden Rule:**
> Higher tiers override lower tiers *unless the lower tier has significantly stronger evidence*. Always explain your reasoning for any tier-based decision.

---

**Version:** v2.1
**Last Updated:** 2025-11-17
**Part of:** BordneAI Research Engine v3.0-alpha
**License:** CC BY 4.0
