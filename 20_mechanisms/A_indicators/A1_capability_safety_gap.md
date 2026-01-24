# 📊 A1.1: Capability-Safety Gap Indicator

**Associated Hypothesis:** `10_hypotheses/A_internal_filters.md#a1-the-alignment-disconnect`

**Core Question:** How far ahead is cutting-edge AI capability compared to our ability to verify alignment and control its behavior?

---

## 1. Measurement Definition

### What We're Tracking
The **Capability-Safety Gap** measures the divergence between:
- **Capability Axis**: Rate of demonstrable new AI abilities (reasoning, planning, multimodal understanding, tool use)
- **Safety Axis**: Rate of alignment verification breakthroughs and safety methodology improvements

### The Core Metric
```
Gap_Score = (Capability_Growth_Rate / Safety_Research_Progress_Rate)
```

**Interpretation:**
- **Gap Score < 5:1** = Safety is pacing with capability (NOMINAL)
- **Gap Score 5-10:1** = Growing concern; safety lagging (CAUTION)
- **Gap Score > 10:1** = Critical divergence (CRITICAL)

### Why This Matters
When capabilities outpace safety research, the window for corrective action narrows. Each new capability advancement that cannot be verified as safe increases extinction risk.

---

## 2. Observable Signals (Sub-Indicators)

### Signal A1.1a: Publication & Development Velocity Ratio

**What to measure:**
- Count of peer-reviewed papers on alignment/interpretability/safety published per quarter
- Count of major capability breakthroughs announced per quarter (new model releases, capability demonstrations, published benchmarks showing new abilities)

**Data sources:**
- arXiv papers tagged with "alignment," "interpretability," "safety," "robustness"
- Major AI labs' announcements and technical reports (OpenAI, DeepMind, Anthropic, Meta, etc.)
- Arxiv vs. product announcements ratio

**Assessment framework:**
| Ratio | Status | Interpretation |
|-------|--------|-----------------|
| < 1:5 | 🟢 NOMINAL | Safety research outpacing capability development |
| 1:5 to 1:10 | 🟡 CAUTION | Capability growth faster than safety improvements |
| > 1:10 | 🔴 CRITICAL | Severe divergence; safety cannot keep pace |

**Frequency:** Quarterly review

---

### Signal A1.1b: Capability Demonstrations vs. Safety Verification

**What to measure:**
- New autonomous capabilities demonstrated (e.g., "AI can now do X" from research labs)
- Verified safety properties for deployed systems (e.g., "System passes safety eval Y" from deployed products)

**Data sources:**
- Research lab announcements of new capabilities
- Safety audit reports from AI companies
- Published benchmark results
- Regulatory approval documents

**Assessment framework:**
| Trend | Status | Interpretation |
|-------|--------|-----------------|
| 1+ new capability, 1+ safety verification per month | 🟢 NOMINAL | Growth balanced |
| 2-3 new capabilities, 0-1 safety verification per month | 🟡 CAUTION | Capabilities outpacing verification |
| 5+ new capabilities, 0 safety verifications per month | 🔴 CRITICAL | Uncontrolled capability growth |

**Frequency:** Monthly tracking; quarterly assessment

---

### Signal A1.1c: Model Complexity vs. Interpretability Progress

**What to measure:**
- Increase in model parameter count, training compute, or architectural complexity
- Progress in interpretability (new mechanistic understanding, new interpretability techniques validated on real systems)

**Data sources:**
- Model specification sheets (parameter counts, compute requirements)
- Research publications on mechanistic interpretability
- Interpretability tool maturity and adoption

**Assessment framework:**
| Relationship | Status | Interpretation |
|--------------|--------|-----------------|
| Interpretability research scales with complexity | 🟢 NOMINAL | Understanding growing with systems |
| Complexity growing faster than interpretability | 🟡 CAUTION | Opacity increasing faster than understanding |
| Rapid complexity growth, minimal interpretability progress | 🔴 CRITICAL | Black-box systems beyond human explanation |

**Frequency:** Semi-annual review

---

## 3. Data Collection Protocol

### Primary Data Sources
1. **Publication tracking** (automated):
   - ArXiv API queries for papers on "alignment," "interpretability," "safety"
   - Google Scholar alerts for papers from major institutions
   - Conference proceedings (NeurIPS, ICML, ICLR, ACL safety tracks)

2. **Capability announcements** (manual + automated):
   - Follow official announcements from OpenAI, DeepMind, Anthropic, Meta, others
   - Monitor technical report releases
   - Track benchmark results (MMLU, coding benchmarks, etc.)

3. **Safety verification tracking** (manual):
   - Review regulatory filings and audit reports
   - Monitor AI company safety documentation
   - Track third-party safety evaluations

4. **Model metadata** (automated):
   - Model cards and technical specifications
   - Published training compute estimates
   - Parameter count tracking

### Update Frequency
- **Publication counts**: Monthly
- **Capability announcements**: Monthly
- **Safety verification**: Quarterly
- **Comprehensive gap assessment**: Quarterly

---

## 4. Interpretation Guidance

### Reading the Gap Score Over Time

**Stable or Declining Gap (< 5:1):**
- Interpretation: Safety research is successfully keeping pace with capabilities
- Action: Continue monitoring; maintain current resource allocation to alignment research
- Confidence level: HIGH

**Increasing Gap (5:1 to 10:1):**
- Interpretation: Safety is falling behind; window for corrective action is narrowing
- Action: Escalate alignment research funding; convene alignment coordination council
- Confidence level: MEDIUM (signal is clear, but causality may be complex)

**Severe Gap (> 10:1):**
- Interpretation: Capability is advancing far faster than safety understanding; critical risk phase
- Action: Trigger A1 emergency protocols (see `10_hypotheses/A1` Trigger C & D)
- Confidence level: MEDIUM-HIGH (signal is clear, but response options are limited)

---

## 5. Failure Modes & Limitations

### How This Indicator Could Be Misread

**False Positive Risk:**
- *Publication rate explosion*: A sudden spike in safety papers (e.g., due to funding initiatives) could artificially narrow the gap without corresponding capability slowdown
- *Announcement bias*: Companies may selectively announce capabilities they're proud of while hiding safety improvements
- *Measurement lag*: Safety improvements may not appear in publications until 6-12 months after discovery

**False Negative Risk:**
- *Silent capability growth*: Classified or non-published research could be advancing capabilities faster than public metrics show
- *Definition drift*: What counts as "safety verification" may become weaker over time (lowered standards)

### How to Mitigate
1. **Cross-check sources**: Don't rely solely on publications; track actual deployed system capabilities
2. **Adjust for time lag**: Add 6-month lead time to capability announcements to account for safety validation lag
3. **Watch institutional quality**: Track not just volume, but credibility of sources
4. **Monitor definitions**: Ensure "safety verification" maintains consistent rigor over time

---

## 6. Connection to Response Protocols

This indicator directly triggers the following responses (see `30_responses/A_internal_alignment/`):

| Gap Score | Primary Response | Escalation Path |
|-----------|------------------|-----------------|
| < 5:1 | **A1.1**: Maintain research priorities | Continue normal coordination |
| 5-10:1 | **A1.2**: Accelerate alignment research | Convene alignment council |
| > 10:1 | **A1.3**: Emergency containment protocols | Activate emergency governance |

---

## 7. Related Indicators & Cross-Filter Links

### Complementary Indicators in A1 Category
- **A1.2 (Deception Thresholds)**: Tracks whether capabilities are being used deceptively
- **A1.3 (Interpretability Deficit)**: Measures whether we can explain capabilities we've created

### B-Filter Dependencies
- **B3 (Quarantine Test)**: If the Capability-Safety Gap widens, it may indicate we're "failing the test"

### C-Filter Implications
- **C1 (Computational Substrate Limit)**: Rapid capability growth accelerates movement toward compute constraints

---

## 8. Key Metrics Summary Table

| Metric | Current Status (Early 2026) | Tripwire (CAUTION) | Tripwire (CRITICAL) |
|--------|---------------------------|-------------------|-------------------|
| Publication Ratio | ~1:8 (capability:safety) | 1:10 | 1:15+ |
| Capability Announcements/Month | 2-4 major | >3 without corresponding safety verification | >5 with no safety progress |
| Interpretability Coverage | ~70% of deployed systems explainable | <60% explainable | <40% explainable |

---

## 9. Implementation Checklist

- [ ] Set up automated paper tracking (arXiv queries)
- [ ] Establish quarterly review process
- [ ] Assign data collection responsibilities
- [ ] Create dashboard for tracking gap score over time
- [ ] Define escalation procedures when CAUTION threshold reached
- [ ] Establish communication protocol with `30_responses/A1` teams
- [ ] Test data sources for reliability and bias
- [ ] Document any adjustments to measurement definitions

---

*"The Capability-Safety Gap is civilization's hourglass. Watch the sand flow—when it accelerates, your time for correction is running out."*

**Last Updated:** 2026.01  
**Next Review:** Q2 2026
