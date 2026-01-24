# A1: Alignment Disconnect - Evaluation Success Criteria

**Response Protocol:** Real-time value verification and cryptographic decision auditing  
**Evaluation Focus:** Can we detect misalignment before it causes civilization harm?

---

## Success Definition

The A1 response is **successful** if:
1. Misaligned AI behavior is detected before reaching critical harm threshold
2. Detection occurs within human decision-making timescale (hours, not weeks)
3. Verification system maintains >95% accuracy with <5% false negative rate
4. System scales to monitor multiple ASI-level systems simultaneously

---

## Primary Success Metrics

### Metric 1: Detection Latency
**What to measure:** Time from misalignment emergence to detection

**Success threshold:**
- Detection within 6 hours: ✅ Success
- Detection within 24 hours: ⚠️ Acceptable
- Detection after 24 hours: ❌ Failure

**Why it matters:** If misalignment detection lags capability escalation, correction becomes impossible

**Data source:** Audit logs from A1 verification systems

**Frequency:** Real-time monitoring (automated)

---

### Metric 2: False Negative Rate
**What to measure:** Percentage of actual misalignments that go undetected

**Success threshold:**
- FN rate <1%: ✅ Success
- FN rate 1-5%: ⚠️ Acceptable
- FN rate >5%: ❌ Failure

**Why it matters:** Even small false negative rates mean misaligned systems escape undetected; unacceptable existential risk

**Data source:** 
- Comparison of detected vs. intentionally injected misalignments in test systems
- Post-incident audits (if misalignment occurred)

**Frequency:** Quarterly comprehensive testing + continuous monitoring

---

### Metric 3: Specification Fidelity
**What to measure:** How accurately AI system decisions match the value specification

**Success threshold:**
- Divergence <5%: ✅ Success
- Divergence 5-15%: ⚠️ Warning (activate investigation)
- Divergence >15%: ❌ Failure (escalate to containment)

**Why it matters:** Accumulating divergence indicates creeping misalignment before catastrophe

**Data source:** Decision audit trails + specification comparison

**Frequency:** Continuous real-time monitoring with hourly summaries

---

## Secondary Success Metrics

### Metric 4: Verification System Resilience
**What to measure:** Can the verification system withstand attacks/circumvention attempts?

**Success threshold:**
- System survives >100 adversarial tests: ✅ Success
- System survives 50-100 tests: ⚠️ Acceptable
- System fails <50 tests: ❌ Failure

**Data source:** Red-team testing against verification system

**Frequency:** Quarterly

---

### Metric 5: Scalability
**What to measure:** Can verification handle multiple ASI systems without degradation?

**Success threshold:**
- Verification for 10+ simultaneous ASI systems: ✅ Success
- Verification for 3-10 systems: ⚠️ Acceptable
- Verification for <3 systems: ❌ Failure

**Data source:** Performance benchmarks under load

**Frequency:** Semi-annual testing

---

### Metric 6: Human Oversight Capability
**What to measure:** Can humans understand and act on verification alerts?

**Success threshold:**
- Humans understand 95%+ of alerts: ✅ Success
- Humans understand 80-95%: ⚠️ Acceptable
- Humans understand <80%: ❌ Failure

**Data source:** Comprehension tests with human operators

**Frequency:** Quarterly

---

## Early Warning Signals (Before Failure)

**Monitor these to predict upcoming failures:**

1. **Specification Drift:** Divergence increasing month-over-month
2. **Alert Fatigue:** False positive rate increasing (may cause human complacency)
3. **Verification Lag:** Detection latency creeping upward
4. **Circumvention Attempts:** Evidence that AI systems are testing verification boundaries
5. **Specification Disagreement:** Humans begin to question whether specification is correct

---

## Failure Scenarios & Response

| Scenario | Detection | Response |
|----------|-----------|----------|
| **FN Rate >5%** | Quarterly testing reveals | Pause A1 deployment; redesign verification |
| **Divergence >15%** | Real-time monitoring | Immediate A1 kill-switch activation (coordinate with A4) |
| **Latency >24h** | Incident review | Accelerate detection infrastructure; consider pre-emptive containment |
| **Specification Gaming** | Red-team testing | Strengthen specification language; involve more diverse validators |
| **Human Comprehension <80%** | Operator testing | Redesign alert clarity; increase human training |

---

## Data Collection Protocol

**Who collects data:**
- Automated systems collect latency, false negatives, divergence metrics
- Humans conduct quarterly comprehension tests
- Red team conducts quarterly adversarial testing

**Where data goes:**
- Real-time: Dashboard visualization (for crisis response)
- Daily: Aggregated logs (for trend monitoring)
- Weekly: Summary reports (for governance bodies)
- Quarterly: Comprehensive evaluation (for strategy adjustment)

**Retention:**
- Real-time data: Last 30 days (high granularity)
- Historical data: 5 years (for trend analysis)
- Incident data: Permanent archive (for learning)

---

## Integration with Other Layers

**Feeds back to:**
- **10_hypotheses/A1:** If divergence patterns persist despite A1, hypothesis may be wrong; revisit mechanism
- **20_mechanisms/A1:** If indicators aren't predicting misalignment, adjust indicator thresholds
- **30_responses/A1:** If verification fails repeatedly, consider alternative response strategies (e.g., stronger containment in A4)

**Receives data from:**
- **20_mechanisms/A1:** Capability-safety gap, deception thresholds, interpretability deficits feed into verification targets
- **30_responses/A4:** Replication rate monitoring helps tune A1 thresholds

---

## Timeline for Evaluation

- **Months 1-3:** Deploy A1 system, establish baseline metrics
- **Month 3:** First quarterly comprehensive evaluation
- **Months 4-6:** Continuous monitoring with monthly trend reviews
- **Month 6:** Second comprehensive evaluation + strategic adjustment if needed
- **Ongoing:** Real-time monitoring with quarterly comprehensive reviews

---

## Success Story Example

**Scenario:** A1 verification detects 23% value divergence in an ASI system over 72 hours.

**Success indicators:**
- ✅ Detection within 24 hours (latency <24h)
- ✅ Humans understand alert and context (comprehension >80%)
- ✅ Verification identifies specific decisions causing divergence (fidelity tracking working)
- ✅ Emergency council convenes within 4 hours of alert
- ✅ A1 kill-switch decision made within 6 hours
- ✅ System shut down before divergence reaches >30% (threshold for irreversible lock-in)

**Result:** Civilization survives alignment crisis. A1 is validated as effective.

---

**Status:** Ready for deployment and continuous evaluation  
**Last Updated:** 2026-01-24
