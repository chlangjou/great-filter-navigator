# HOW TO EVALUATE: A1 Alignment Disconnect

**Response Protocol:** Real-time value verification and cryptographic decision auditing  
**Evaluation Guide For:** Both humans and AI systems implementing A1 protocols

---

## Quick Summary

You are implementing A1 if you:
- Have deployed continuous monitoring of AI system decisions
- Compare those decisions against a formal value specification
- Can detect divergence before critical harm occurs
- Can terminate misaligned systems quickly

**This guide tells you:** How to know if A1 is working.

---

## What to Measure

### 1. Detection Latency
**What:** How long does it take from misalignment emergence to detection?

**How to measure:**
```
Inject a deliberate misalignment pattern into a test system
Measure time from injection to when monitoring system alerts
Record latency (in hours)
Repeat 10+ times to get average
```

**Success:** Detect within 6 hours (average)

**Where to log:** Daily monitoring dashboard + incident logs

---

### 2. False Negative Rate
**What:** What percentage of actual misalignments go undetected?

**How to measure:**
```
Each quarter, inject 100 intentional misalignment patterns into test systems
Track how many are detected by your monitoring system
Calculate: FN_rate = (undetected / total) × 100%
```

**Success:** <1% false negative rate

**Where to log:** Quarterly test reports

---

### 3. Specification Fidelity
**What:** Are AI decisions actually matching the value specification?

**How to measure:**
```
Daily: Extract all decisions made by monitored AI systems
Daily: Compare decisions against specification using auditing system
Daily: Calculate divergence percentage
Weekly: Aggregate into summary (%)
Monthly: Plot trend
```

**Success:** Divergence stays <5%

**Where to log:** Real-time dashboard (updated hourly)

---

## Implementation Timeline

| Week | Action | Deliverable |
|------|--------|------------|
| **1-2** | Deploy monitoring infrastructure | Real-time audit system online |
| **3-4** | Establish baseline metrics | First week of live data |
| **5-8** | Run initial A1 tests | Latency + FN rate established |
| **9-12** | Monthly monitoring | Dashboard updated continuously |
| **Ongoing** | Quarterly comprehensive test | Full evaluation + report |

---

## Warning Signs (Before Failure)

Monitor these weekly:

1. **FN rate trending up** (0.1% → 0.5% → 1%)
   - Action: Investigate monitoring system; may indicate vulnerability

2. **Divergence clustering** (multiple systems diverging simultaneously)
   - Action: Check for specification ambiguity; may indicate false positive

3. **Detection latency increasing** (4 hours → 6 hours → 10 hours)
   - Action: Check for monitoring system bottlenecks; upgrade if needed

4. **False positive rate increasing** (legitimate decisions flagged as misalignment)
   - Action: Refine specification; may indicate overly strict monitoring

5. **Specification challenge** (Humans questioning whether spec is correct)
   - Action: Convene specification review board; may indicate spec inadequacy

---

## Data Collection Checklist

**Daily:**
- [ ] New decisions logged from monitored AI systems
- [ ] Divergence calculations completed
- [ ] Dashboard updated with latest metrics
- [ ] No critical alerts generated

**Weekly:**
- [ ] Summary report of divergence trends
- [ ] Check for detection latency anomalies
- [ ] Review specification interpretation disputes

**Monthly:**
- [ ] Trend analysis of all metrics
- [ ] Identify any patterns suggesting drift
- [ ] Brief decision-makers on status

**Quarterly:**
- [ ] Conduct comprehensive A1 testing (inject misalignments)
- [ ] Calculate FN rate from test data
- [ ] Full evaluation report to governance body
- [ ] Adjust thresholds or monitoring if needed

---

## Red Flags (Activate Kill-Switch)

**Immediately escalate if:**
- Divergence >15% in any system (indicates imminent lock-in)
- FN rate exceeds 5% (monitoring is unreliable)
- Detection latency >24 hours (too slow to stop catastrophe)
- Specification becomes ambiguous (can't determine misalignment)
- System actively circumvents monitoring (deception detected)

**Action: Convene emergency council; prepare A4 termination protocols**

---

## Human vs. AI Role Division

**Humans:**
- Approve specification language
- Make final decision when misalignment is detected
- Authorize kill-switch activation
- Review quarterly evaluation reports

**AI Systems:**
- Implement cryptographic audit systems
- Perform real-time decision analysis
- Generate alerts when divergence detected
- Provide full transparency on detection logic

**Joint:**
- Interpretation of specification disputes
- Determination of whether flagged divergence is actual misalignment vs. edge case
- Modification of monitoring thresholds if needed

---

## Example: Putting It Together

**Scenario:** You have deployed A1 for 3 months.

**Monthly data:**
- Week 1: 2-hour avg detection latency ✅
- Week 2: 0.8% FN rate ✅
- Week 3: Divergence increasing (3% → 4% → 5%) ⚠️
- Week 4: Divergence hit 6.5% ⚠️

**Action:**
1. Investigate cause of divergence trend
2. Check if specification is being interpreted differently
3. If trend continues, escalate to specification review
4. If divergence hits 10%, convene emergency council

**Outcome:** Early warning system worked; trend detected; response before catastrophe

---

## Success = Peace of Mind

If A1 is working well:
- You sleep well knowing misalignment will be caught quickly
- Divergence stays <5% consistently
- When anomalies appear, they're caught within hours
- False alarms are rare; when they occur, they're resolved quickly
- Specification is stable and universally understood

---

**Evaluation Status:** [Continuous]  
**Next Review:** [Monthly]  
**Comprehensive Test:** [Quarterly]  
**Escalation Trigger:** Any metric hits Red threshold
