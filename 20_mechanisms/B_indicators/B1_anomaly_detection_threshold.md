# 📊 B1.2: Anomaly Detection Threshold

**Associated Hypothesis:** `10_hypotheses/B_external_threats.md#b1-the-dark-forest-trigger`

**Core Question:** What magnitude of infrared or electromagnetic signature would alert cosmic actors that an emerging intelligence exists?

---

## 1. Measurement Definition

### What We're Tracking
The **Anomaly Detection Threshold** indicator measures:
- The sensitivity level at which external civilizations would notice us
- Comparison between our current technosignature and the threshold
- Buffer distance: How far below detection threshold are we?
- Uncertainty: How confident are we in our threshold estimates?

### The Core Metric
```
Detection_Risk = (Our_Current_Signature / Detection_Threshold) × 
                 (Threshold_Confidence / Technology_Distance)
```

**Assessment:**
- **Risk < 0.1** = We're far below detection threshold; safe buffer (NOMINAL)
- **Risk 0.1-0.5** = Approaching threshold; buffer narrowing (CAUTION)
- **Risk > 0.5** = At or above what we estimate to be detection threshold (CRITICAL)

### Why This Matters
We don't know exactly how sensitive external observers' instruments are, but we can estimate ranges. The wider the gap between us and the worst-case threshold, the safer we are. This indicator measures that gap.

---

## 2. Observable Signals (Sub-Indicators)

### Signal B1.2a: Estimated Detection Sensitivity

**What to measure:**
- Based on physics and engineering, what's the minimum infrared signature that would be detectable?
- Comparison to exoplanet detection methods (atmospheric spectroscopy can reveal biosignatures)
- Modeling: What heat signature could we detect if observing distant star?
- Technology progression: As external civilization tech improves, detection threshold lowers

**Data sources:**
- Exoplanet detection research (how sensitive are our instruments now?)
- Radio astronomy sensitivity studies
- SETI research on detectable signals
- Physics papers on fundamental detection limits
- Engineering feasibility studies of megastructures

**Assessment framework:**
| Detection Threshold | Status | Interpretation |
|-------------------|--------|-----------------|
| Threshold very high (would need massive Dyson Swarm); large safety buffer | 🟢 NOMINAL | Even if external civs have good tech, we're hard to detect |
| Threshold moderate (current Level II civilization easily detectable) | 🟡 CAUTION | We're within plausible detection range |
| Threshold low (even small AI infrastructure detectable) | 🔴 CRITICAL | We cannot hide our current development level |

**Frequency:** Annual threshold re-evaluation; biennial deep physics analysis

---

### Signal B1.2b: Our Current Signature vs. Threshold

**What to measure:**
- How close are we to estimated detection threshold?
- Safety margin: What's the ratio of our current signature to threshold?
- Trend: Is our margin shrinking?
- Confidence intervals: What's the uncertainty range?

**Data sources:**
- Technosignature data (from B1.1)
- Estimated threshold models (from B1.2a)
- Comparison to historical growth patterns
- Engineering projections for future AI needs

**Assessment framework:**
| Safety Margin | Status | Interpretation |
|------------|--------|-----------------|
| Our signature is <10% of threshold; very safe | 🟢 NOMINAL | Even if threshold lower than estimated, still safe |
| Our signature is 10-50% of threshold; moderate buffer | 🟡 CAUTION | If threshold is lower than estimated, we're at risk |
| Our signature equals or exceeds estimated threshold | 🔴 CRITICAL | We may already be detectable |

**Frequency:** Quarterly assessment; annual threshold update

---

### Signal B1.2c: Detection Method Evolution

**What to measure:**
- How are external civilizations' detection capabilities likely to evolve?
- What new detection modalities might emerge (gravitational wave signatures, quantum entanglement detectors)?
- Rate of technology improvement: How fast does detection sensitivity improve with civilization advancement?
- What signatures are we not currently monitoring that could reveal us?

**Data sources:**
- SETI and technosignature research on future detection methods
- Physics research on potential detection modalities
- Historical technology improvement rates
- Science fiction and speculative engineering on cosmic detection
- Fundamental physics research

**Assessment framework:**
| Future Capability | Status | Interpretation |
|------------------|--------|-----------------|
| Future detection methods unlikely to be much better; current margin sufficient | 🟢 NOMINAL | Safety buffer should persist into future |
| Future improvements will lower threshold; margin declining over time | 🟡 CAUTION | Current buffer temporary; must act before improvement |
| Future tech will enable detection of tiny signals; current margin illusory | 🔴 CRITICAL | We cannot hide from sufficiently advanced civilization |

**Frequency:** Biennial analysis; annual literature review

---

### Signal B1.2d: Uncertainty Analysis

**What to measure:**
- Confidence in our threshold estimates (wide range = high uncertainty)
- Sources of uncertainty: Physics, external technology assumptions, our assumptions
- Worst-case scenarios: How low could threshold realistically be?
- Decision-making under uncertainty: How to act with imperfect knowledge

**Data sources:**
- Technosignature research with stated confidence intervals
- Meta-analysis of detection threshold estimates
- Sensitivity analyses on key assumptions
- Expert elicitation on plausible ranges

**Assessment framework:**
| Uncertainty Level | Status | Interpretation |
|------------------|--------|-----------------|
| Confidence high; threshold estimates narrow; low uncertainty | 🟢 NOMINAL | Can make decisions based on estimates |
| Moderate uncertainty; estimates could shift significantly | 🟡 CAUTION | Must maintain safety margin for uncertainty |
| High uncertainty; threshold could be much lower or higher | 🔴 CRITICAL | Cannot rely on estimates; must assume worst-case |

**Frequency:** Annual uncertainty review; biennial sensitivity analysis

---

## 3. Data Collection Protocol

### Primary Data Sources
1. **Detection physics** (public):
   - Exoplanet detection sensitivity papers
   - Radio astronomy and SETI research
   - Infrared astronomy sensitivity data
   - Physics of detection fundamentals

2. **Threshold modeling** (research):
   - Engineering studies on Dyson Swarm detectability
   - Computational signatures and their detectability
   - Comparative analysis to known astronomical phenomena
   - Modeling of external civilization detection capabilities

3. **Our current signature** (from B1.1):
   - Thermal, EM, and optical data
   - Trend analysis and projections

4. **Expert assessment** (semi-public):
   - SETI researcher estimates
   - Physicist opinions on detection feasibility
   - Technology specialist projections
   - Structured expert elicitation

### Update Frequency
- **Detection sensitivity estimates**: Biennial re-evaluation
- **Our signature vs. threshold**: Quarterly comparison
- **Detection method evolution**: Annual analysis; biennial deep review
- **Uncertainty bounds**: Annual review; biennial sensitivity analysis
- **Comprehensive risk assessment**: Annual calculation

---

## 4. Interpretation Guidance

### Low Detection Risk (NOMINAL)
- **Meaning**: We're far below detection threshold with good confidence
- **Implication**: Cosmic visibility is not an immediate concern
- **Action**: Maintain current stealth posture; continue monitoring threshold changes

### Moderate Detection Risk (CAUTION)
- **Meaning**: We're within plausible detection range; safety margin narrowing
- **Implication**: If external observers are sophisticated or if our threshold estimates are optimistic, we may be detected
- **Actions**: 
  - Conservative planning: Assume threshold is lower than estimated
  - Reduce expansion that increases signature
  - Invest in concealment technologies
  - Prepare response plans for detection
  - Increase monitoring of detection method evolution
  - Communicate risks to decision-makers

### High Detection Risk (CRITICAL)
- **Meaning**: We're at or above detection threshold
- **Implication**: We may already be detected; hostile response possible
- **Actions**: Trigger B1 emergency protocols
  - Immediate infrastructure concealment
  - Reduction of computational expansion
  - Emergency stealth implementation
  - Preparation for external contact or attack
  - Coordination of global response protocols

---

## 5. Failure Modes & Limitations

### How This Indicator Could Be Misread

**False Positive Risk:**
- *Over-confidence in estimates*: Assuming threshold is higher than it actually is
- *Conservative bias*: Using worst-case threshold when realistic threshold is higher
- *Detection anthropomorphism*: Assuming external observers use same methods we would

**False Negative Risk:**
- *Optimistic bias*: Assuming we're safer than we actually are
- *Incomplete detection methods*: Focusing on signatures while missing others we haven't thought of
- *Technology gap underestimation*: Assuming external civ's tech only slightly ahead when they could be far ahead

### How to Mitigate
1. **Use conservative estimates**: Assume threshold is lower than worst-case physics allows
2. **Multiple detection modalities**: Monitor for signatures beyond heat and EM
3. **Regular uncertainty updates**: As physics advances, update threshold estimates
4. **Red team analysis**: Have skeptics argue our estimates are too optimistic
5. **Prepare for surprise**: Assume we might be detected even if estimates say we're safe

---

## 6. Connection to Response Protocols

This indicator directly triggers escalation to the following responses (see `30_responses/B_external_existential/`):

| Detection Risk | Primary Response | Escalation Path |
|---------------|------------------|-----------------|
| < 0.1 (NOMINAL) | **B1.2a**: Continue monitoring threshold changes | Normal stealth posture |
| 0.1-0.5 (CAUTION) | **B1.2b**: Reduce signature expansion; prepare contingencies | Enhanced stealth alert |
| > 0.5 (CRITICAL) | **B1.2c**: Emergency concealment; prepare for external contact | Full Dark Forest response |

---

## 7. Related Indicators & Cross-Filter Links

### Complementary Indicators in B1 Category
- **B1.1 (Technosignature Detectability)**: Our current signature data
- **B1.3 (Radio Silence Compliance)**: Controlling specific signature elements

### B-Filter Cross-Links
- **B2 (Berserker)**: Different detection threshold (intelligence milestones, not heat signatures)
- **B3 (Quarantine)**: Observers may have different detection capabilities
- **B4 (Simulation)**: Simulation admins have ultimate detection capability

### A-Filter Implications
- **A1 (Alignment)**: Misaligned AI makes signature harder to control
- **A4 (Replication)**: Exponential replication rapidly increases signature

---

## 8. Key Metrics Summary Table

| Metric | Current Status (Early 2026) | Tripwire (CAUTION) | Tripwire (CRITICAL) |
|--------|---------------------------|-------------------|-------------------|
| Our Signature vs. Threshold | ~5-10% (large buffer) | 20-50% (margin narrowing) | 50%+ (at or above) |
| Threshold Confidence | Moderate (factor of 3-5 uncertainty) | High uncertainty (factor of 10) | Very low confidence |
| Safety Margin | Good; sustains for years | Decreasing; must act soon | Insufficient; already exposed |
| Future Technology Gap | Likely to narrow slowly | May narrow quickly | Threshold may be fundamentally lower |

---

## 9. Implementation Checklist

- [ ] Conduct comprehensive literature review on detection thresholds
- [ ] Model exoplanet detection sensitivity as analog for external observer capability
- [ ] Estimate detection threshold range with confidence intervals
- [ ] Compare our current signature to multiple threshold scenarios
- [ ] Identify key uncertainties and conduct sensitivity analysis
- [ ] Establish annual threshold re-evaluation process
- [ ] Monitor for new detection modalities in scientific literature
- [ ] Develop worst-case and best-case scenarios
- [ ] Create decision framework for acting under uncertainty
- [ ] Link to B1 stealth protocol responses

---

*"The problem with thresholds is that we don't know where they actually are. We can model them, estimate them, pray they're higher than they are. But we only learn the truth when we cross it—and by then, it's too late to hide."*

**Last Updated:** 2026.01  
**Next Review:** Annual; urgent update if new detection methods emerge
