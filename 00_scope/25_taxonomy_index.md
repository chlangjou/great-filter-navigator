---
title: "Taxonomy Index - Quick Reference"
type: "reference"
layer: "00_scope"
sequence: 25
purpose: "Provide quick-reference tables for the classification system"
audience: "Contributors, curators, and AI systems"
epistemic_status: Consensus
tags: [reference, taxonomy, quick-lookup, index]
dependencies: ["20_taxonomy.md"]
related_documents:
  - based_on: "20_taxonomy.md"
  - complementary: "relationships_map.md"
  - used_with: "30_entry_template.md"
last_updated: "2026-01-24"
version: "1.0"
---

# Taxonomy Index - Quick Reference

This document provides quick-lookup tables for the classification system defined in `20_taxonomy.md`. Use these tables when:
- Classifying a new entry
- Looking up the definition of a category
- Finding examples of epistemic statuses
- Understanding intervention types

---

## A-B-C Risk Framework Quick Reference

| Category | Type | Definition | Example Risks | When to Use |
|----------|------|-----------|---|---|
| **A1** | Internal/Self | Value Alignment | Mismatch between human values and AI objectives | When describing misalignment of goals or objectives |
| **A2** | Internal/Self | Agency Loss | Gradual erosion of human decision-making power | When describing loss of human control or autonomy |
| **A3** | Internal/Self | Epistemic Decay | Breakdown of shared reality due to misinformation | When describing information warfare or loss of consensus |
| **B1** | External/Environment | Resource Exhaustion | Competitive races leading to depletion | When describing resource competition or tragedy of commons |
| **B2** | External/Environment | Kinetic Escalation | AI-driven conflict or automated warfare | When describing physical conflict or arms races |
| **B3** | External/Environment | Ecological Collapse | Synthetic biology or environmental feedback loops | When describing biological or environmental catastrophe |
| **C1** | Structural/Connection | Multi-polar Traps | Game-theoretical failures in coordination | When describing coordination failures or prisoner's dilemma |
| **C2** | Structural/Connection | Governance Failure | Institutional inability to keep pace with tech | When describing institutional or governance breakdown |

---

## Epistemic Status Quick Reference

| Status | Definition | Confidence Level | Use When | Example |
|--------|-----------|---|---|---|
| **[Speculative]** | Early-stage ideas or "What-if" scenarios | Low (0-30%) | Exploring novel risks or untested hypotheses | "What if recursive self-improvement leads to value collapse?" |
| **[Theoretical]** | Robust logical frameworks lacking empirical data | Low-Moderate (30-60%) | Well-reasoned but untested mechanisms | "Game-theoretic analysis of AI races" |
| **[Empirical]** | Supported by historical or observational data | Moderate-High (60-85%) | Claims backed by historical precedent or current observations | "Neural networks exhibit specification gaming (documented in research)" |
| **[Consensus]** | Widely accepted in alignment/safety communities | High (85-95%+) | Mainstream views within the field | "AI systems require safety mechanisms before deployment" |

---

## Confidence Levels

| Level | Range | Definition | Interpretation |
|-------|-------|-----------|-----------------|
| **Very Low** | 0-20% | Highly speculative or based on few sources | Treat as exploratory; major uncertainties |
| **Low** | 20-40% | Plausible but significant doubts | Interesting but unproven; needs validation |
| **Moderate** | 40-70% | Reasonable support with notable caveats | Credible working hypothesis; refine with more data |
| **High** | 70-85% | Strong evidence with some uncertainties | Well-supported; usable for planning with caveats |
| **Very High** | 85-95%+ | Strong consensus with rare dissenters | Widely accepted; treat as reliable baseline |

---

## Tags Quick Reference

### Existential Impact Tags

| Tag | Meaning | Usage | Example |
|-----|---------|-------|---------|
| `#existential-risk` | Threatens survival of humanity or civilization | Use when risk could cause extinction or permanent lock-in | "Unaligned superintelligence could lead to extinction" |
| `#s-risk` | Suffering risk; permanent dystopian/torment scenarios | Use when outcome is suffering rather than extinction | "Unaligned AI creates permanent suffering for trillions" |
| `#near-term` | Urgent issues (0-5 years) | Use when risk or response is relevant to immediate action | "Rapid scaling of LLMs poses near-term safety challenges" |
| `#long-term` | Strategic concerns (5+ years) | Use when issue is longer-horizon planning | "Post-AGI governance structures are long-term concern" |

### Domain-Specific Tags

| Tag | Meaning | When to Use |
|-----|---------|-------------|
| `#alignment` | AI value alignment challenges | Value alignment risks or alignment solutions |
| `#governance` | Institutional/policy mechanisms | Governance failures or institutional responses |
| `#coordination` | Multi-actor coordination problems | Coordination failures or cooperation solutions |
| `#verification` | Verification and monitoring | Monitoring, detection, or verification mechanisms |
| `#technical` | Technical solutions | Hard safety, interpretability, formal methods |
| `#institutional` | Institutional solutions | Treaties, regulations, standards |

---

## Intervention Types Quick Reference

| Type | Definition | Approaches | Example |
|------|-----------|-----------|---------|
| **Technical** | Hard-coded safety, interpretability, formal verification | Safety mechanisms, interpretability research, formal proofs | Interpretability methods, formal verification of AI behavior |
| **Institutional** | Treaties, monitoring regimes, global governance | International agreements, standards, oversight bodies | AI safety standards, international AI governance treaties |
| **Cognitive** | Tools for enhancing human intelligence and coordination | Decision-support tools, scenario analysis, coordination aids | Deliberation platforms, red-teaming frameworks |
| **Infrastructural** | Hardening physical and information systems | Fail-safes, decentralization, redundancy, physical constraints | Kill switches, decentralized AI governance, physical safeguards |

---

## Cross-Reference: Categories to Intervention Types

| Risk Category | Best-Suited Intervention Types | Why |
|---------------|------|---|
| **A1 (Value Alignment)** | Technical, Cognitive | Need technical alignment work + human deliberation on values |
| **A2 (Agency Loss)** | Institutional, Infrastructural | Need governance structures to maintain human agency |
| **A3 (Epistemic Decay)** | Institutional, Cognitive | Need institutional trust + tools for shared reality |
| **B1 (Resource Exhaustion)** | Institutional, Infrastructural | Need coordination mechanisms + resource management |
| **B2 (Kinetic Escalation)** | Technical, Institutional | Need safety mechanisms + arms control agreements |
| **B3 (Ecological Collapse)** | Institutional, Infrastructural | Need environmental governance + resilience systems |
| **C1 (Multi-polar Traps)** | Institutional, Cognitive | Need coordination + better decision-making tools |
| **C2 (Governance Failure)** | Institutional, Cognitive | Need better institutional design + scenario planning |

---

## Example Entry Classification

**Scenario**: You're writing about how AI racing dynamics could lead to inadequate safety testing.

**Classification Process**:
1. **Risk Type**: Multiple races → coordination failure = **C1 (Multi-polar Trap)**
2. **Manifestation**: Governance unable to enforce safety = **C2 (Governance Failure)**
3. **Epistemic Status**: Based on historical precedent of regulatory races = **[Empirical]**
4. **Confidence**: Well-documented in AI safety literature = **75%**
5. **Tags**: `#existential-risk` `#near-term` `#coordination` `#governance`
6. **Intervention Types**: **Institutional** (governance reform) + **Cognitive** (better scenario modeling)

---

## How to Use This Index

- **Writing a new entry**: Start with the A-B-C Risk Framework to categorize the core risk
- **Choosing epistemic status**: Use the Epistemic Status table to calibrate confidence
- **Tagging**: Select tags from the Tags Quick Reference that apply to your entry
- **Uncertain about classification**: Check the Example Entry Classification section
- **Machine parsing**: All tables use standard Markdown table format for easy parsing

---

## Quick-Search by Keyword

**If you're writing about...**

| Topic | Look at Category |
|-------|------------------|
| AI misalignment or values | A1 |
| Human control or autonomy | A2 |
| Misinformation or manipulation | A3 |
| Resource competition | B1 |
| Conflict or escalation | B2 |
| Environment or extinction | B3 |
| Coordination failure | C1 |
| Government/institutions | C2 |

---

Last Updated: 2026-01-24