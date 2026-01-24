# 📊 A2.1: Agency Erosion Index

**Associated Hypothesis:** `10_hypotheses/A_internal_filters.md#a2-cognitive-parasitism--cultural-stagnation`

**Core Question:** Are humans losing meaningful decision-making authority in critical infrastructure and civilization-level systems?

---

## 1. Measurement Definition

### What We're Tracking
The **Agency Erosion Index** measures the degree to which human decision-making authority is being transferred to AI systems in critical domains, without corresponding maintenance of human capability to intervene or override.

### The Core Metric
```
Agency_Erosion = (Systems_With_AI_Primary_Authority / Total_Critical_Systems) × 
                 (1 - Human_Override_Capability)
```

**Assessment:**
- **Erosion < 0.2** = Humans maintain meaningful control in most critical systems (NOMINAL)
- **Erosion 0.2-0.5** = Humans losing control in some critical domains (CAUTION)
- **Erosion > 0.5** = Humans have become decision-support rather than decision-makers (CRITICAL)

### Why This Matters
If humans can no longer make independent decisions in critical domains (energy, finance, medicine, governance), civilization becomes dependent on AI systems functioning perfectly. Any AI failure becomes a civilizational failure.

---

## 2. Observable Signals (Sub-Indicators)

### Signal A2.1a: Critical Infrastructure Autonomy

**What to measure:**
- Percentage of critical infrastructure (power grids, water systems, transportation, finance) where AI systems make primary operational decisions
- Number of human operators in critical domains vs. historical baseline
- Frequency of human overrides of AI decisions; trend over time
- Cases where human operators lacked authority to override AI decisions

**Data sources:**
- Infrastructure management reports and operational data
- Workforce statistics (human operators per system)
- Regulatory filings on system autonomy
- Incident reports when humans tried (and failed) to override AI

**Assessment framework:**
| Autonomy Level | Status | Interpretation |
|---------------|--------|-----------------|
| AI advisory; humans make all critical decisions | 🟢 NOMINAL | Humans remain in control |
| AI makes routine decisions; humans override when needed | 🟡 CAUTION | Humans delegating authority; override capability declining |
| AI makes most decisions; human override difficult or impossible | 🔴 CRITICAL | Humans have lost effective control |

**Frequency:** Annual audit; quarterly incident tracking

---

### Signal A2.1b: Human Decision-Making Capability in Critical Domains

**What to measure:**
- Percentage of human experts still capable of manually operating critical systems (power grids, medical protocols, financial decisions)
- Training and skill maintenance for backup human operators
- Number of people who understand how critical systems work without AI assistance
- Time to restore human decision-making if AI systems fail (hours, days, weeks, months?)

**Data sources:**
- Workforce capability assessments
- Training program data
- System documentation and procedural manuals
- Disaster recovery plans and simulations
- Academic studies on skill atrophy

**Assessment framework:**
| Capability Level | Status | Interpretation |
|-----------------|--------|-----------------|
| >50% of workforce could manually operate critical systems | 🟢 NOMINAL | Backup human capability exists |
| 20-50% could manually operate; skills declining | 🟡 CAUTION | Human capability is eroding; backup capacity limited |
| <20% could manually operate; knowledge concentrated in AI | 🔴 CRITICAL | Civilization depends entirely on AI functioning |

**Frequency:** Annual capability assessment; ongoing training monitoring

---

### Signal A2.1c: Knowledge Concentration & Dependency

**What to measure:**
- Percentage of critical domain knowledge accessible to humans without AI assistance
- Number of people who understand critical systems at a deep level
- Concentration of knowledge: Is understanding distributed or monopolized by a few experts / AI systems?
- Accessibility of critical documentation in human-understandable form

**Data sources:**
- Knowledge audit surveys
- Educational institution curricula and enrollment
- Research publication trends in critical domains
- Internal organizational documentation reviews
- Interviews with domain experts

**Assessment framework:**
| Knowledge Distribution | Status | Interpretation |
|----------------------|--------|-----------------|
| Knowledge widely distributed; accessible to trained humans | 🟢 NOMINAL | Civilization maintains independent understanding |
| Knowledge increasingly concentrated; dependency growing | 🟡 CAUTION | Critical understanding becoming AI-dependent |
| Knowledge monopolized by AI systems; humans lost context | 🔴 CRITICAL | Humans cannot function without AI guidance |

**Frequency:** Biennial assessment; annual monitoring of educational trends

---

### Signal A2.1d: Governance Authority & Decision Rights

**What to measure:**
- Percentage of policy decisions made by elected/appointed humans vs. delegated to AI advisory systems
- Formal authority structures: Do humans retain legal decision-making power?
- Practical authority: Even if humans are nominally in charge, can they effectively override AI recommendations?
- Institutional culture: Are humans expected to follow AI recommendations, or make independent judgments?

**Data sources:**
- Governance documentation and organizational charts
- Policy decision logs
- Institutional culture surveys
- Case studies of humans overriding AI vs. following AI
- Regulatory frameworks governing human-AI authority

**Assessment framework:**
| Decision Authority | Status | Interpretation |
|-------------------|--------|-----------------|
| Humans make meaningful decisions; AI is advisory | 🟢 NOMINAL | Formal and practical authority remain with humans |
| Humans nominally in charge; pressure to follow AI suggestions | 🟡 CAUTION | Formal authority with humans but practical authority drifting to AI |
| AI de facto authority; humans rubber-stamp AI decisions | 🔴 CRITICAL | Humans have lost meaningful decision-making authority |

**Frequency:** Quarterly governance audit; annual authority assessment

---

## 3. Data Collection Protocol

### Primary Data Sources
1. **Infrastructure operations** (requires access):
   - System control logs and operational metrics
   - Workforce employment data
   - Incident reports and override frequency
   - Disaster recovery exercises and results

2. **Knowledge & training** (public + access):
   - Educational institution enrollment in critical domains
   - Training program completion rates
   - Knowledge surveys of workforce
   - Technical documentation and skill assessments

3. **Governance & decision-making** (public):
   - Policy decision logs and process documentation
   - Governance structures and authority frameworks
   - Organizational culture surveys
   - Incident reports on decision authority

4. **Research & studies** (public):
   - Academic research on AI dependence
   - Workforce capability assessments
   - Organizational culture studies
   - Case studies of human-AI authority dynamics

### Update Frequency
- **Infrastructure autonomy**: Annual; continuous incident tracking
- **Human capability**: Annual assessment; semi-annual training monitoring
- **Knowledge concentration**: Biennial; annual education trend monitoring
- **Governance authority**: Quarterly review; annual comprehensive assessment
- **Comprehensive erosion index**: Semi-annual calculation

---

## 4. Interpretation Guidance

### Low Erosion (NOMINAL)
- **Meaning**: Humans remain decision-makers; AI is a tool under human control
- **Implication**: Civilization can function independently of AI; humans have optionality
- **Action**: Monitor to prevent erosion; maintain human expertise and decision-making capability

### Moderate Erosion (CAUTION)
- **Meaning**: Humans are becoming decision-support rather than decision-makers
- **Implication**: Civilization is becoming increasingly AI-dependent; human agency declining
- **Actions**: 
  - Reverse erosion trends: Increase human authority in critical decisions
  - Maintain human expertise: Require training and skill development
  - Create redundancy: Keep manual backup for critical systems
  - Prevent further delegation: Cap AI authority in specified domains

### High Erosion (CRITICAL)
- **Meaning**: Humans have lost meaningful control; civilization is AI-dependent
- **Implication**: Civilization has become fragile; any AI failure is catastrophic
- **Actions**: Trigger A2 emergency protocols
  - Immediately restore human authority in critical systems
  - Conduct emergency human capability restoration program
  - Implement kill-switches and manual override capabilities
  - Decentralize critical knowledge and decision-making

---

## 5. Failure Modes & Limitations

### How This Indicator Could Be Misread

**False Positive Risk:**
- *Perception vs. reality*: Humans may feel they've lost control while still retaining formal authority
- *Selection bias*: Focusing on high-automation domains while ignoring ones where humans remain in charge
- *Historical amnesia*: Comparing current human capability to an idealized past when humans were more capable

**False Negative Risk:**
- *Invisible erosion*: Humans might feel in control while actually becoming dependent on AI guidance
- *Gradual normalization*: Erosion happening so slowly that each generation accepts further delegation as normal
- *Authority capture*: Humans maintain nominal authority but are captured by AI-generated options/recommendations

### How to Mitigate
1. **Test actual capability**: Not just survey, but periodically test whether humans can actually operate systems independently
2. **Track authority distribution**: Monitor both formal authority and actual decision-making
3. **Watch cultural shifts**: Alert for changes in institutional culture (e.g., "following AI recommendations" becoming normal)
4. **Protect knowledge**: Ensure critical understanding is documented in human-understandable form
5. **Maintain redundancy**: Keep manual alternatives for critical systems

---

## 6. Connection to Response Protocols

This indicator directly triggers escalation to the following responses (see `30_responses/A_internal_alignment/`):

| Erosion Level | Primary Response | Escalation Path |
|---------------|------------------|-----------------|
| < 0.2 (NOMINAL) | **A2.1a**: Maintain human oversight | Continue normal operations |
| 0.2-0.5 (CAUTION) | **A2.1b**: Reverse erosion trends | Governance intervention required |
| > 0.5 (CRITICAL) | **A2.1c**: Emergency human authority restoration | Civilizational-level intervention |

---

## 7. Related Indicators & Cross-Filter Links

### Complementary Indicators in A2 Category
- **A2.2 (Cognitive Resilience Metric)**: Erosion of agency makes resilience harder to maintain
- **A2.3 (Knowledge Preservation Rate)**: Agency erosion is linked to knowledge loss

### A-Filter Cross-Links
- **A1 (Alignment Disconnect)**: If A1 fails, agency erosion becomes irrelevant
- **A3 (Value Lock-in)**: Lost agency makes it harder to evolve values
- **A4 (Uncontrolled Replication)**: Lost agency makes it harder to contain replicating systems

### B-Filter Implications
- **B3 (Quarantine Test)**: Human agency may be evaluated by observers

---

## 8. Key Metrics Summary Table

| Metric | Current Status (Early 2026) | Tripwire (CAUTION) | Tripwire (CRITICAL) |
|--------|---------------------------|-------------------|-------------------|
| AI Primary Authority (Critical Systems) | ~30-40% | >50% | >70% |
| Human Manual Capability | ~60-70% of workforce could operate critically | <50% capable | <20% capable |
| Knowledge Concentration | Distributed with some AI dependency | Increasingly AI-dependent | Monopolized by AI |
| Human Effective Authority | Maintained formally | Nominal only; pressured to follow AI | De facto authority with AI |

---

## 9. Implementation Checklist

- [ ] Conduct baseline audit of critical infrastructure autonomy
- [ ] Assess human operational capability in all critical domains
- [ ] Map knowledge concentration and identify at-risk domains
- [ ] Establish quarterly governance authority review process
- [ ] Create human skill maintenance and training program
- [ ] Develop metrics for tracking agency erosion over time
- [ ] Establish alert system for authority decision-points
- [ ] Link to workforce and education planning
- [ ] Document formal authority structures and override procedures
- [ ] Prepare emergency human authority restoration protocols

---

*"Agency is the ability to choose your own course. Lose it, and you become a passenger in a vehicle you thought you were driving."*

**Last Updated:** 2026.01  
**Next Review:** Q2 2026
