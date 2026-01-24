# 📊 Category A: Internal Risk Indicators

**Focus:** Monitoring autogenic (self-generated) failure modes arising from a civilization's own technological trajectory.

**Question:** *How do we know we are failing to align AI or maintain our own agency?*

---

## Overview

These indicators track the four primary internal filters defined in `10_hypotheses/A_internal_filters.md`:

| Hypothesis | Indicator | Status | Data Source |
|------------|-----------|--------|-------------|
| **A1: Alignment Disconnect** | Capability-Safety Gap, Deception Thresholds, Interpretability Deficit | ✅ COMPLETE | ArXiv, capability announcements, safety audits |
| **A2: Cognitive Parasitism** | Agency Erosion Index, Cognitive Resilience Metric, Knowledge Preservation Rate | ✅ COMPLETE | Infrastructure operations, workforce assessment, education data |
| **A3: Value Lock-in** | Value Diversity Index, Adaptability Coefficient, Consensus Drift | ✅ COMPLETE | Polling data, institutional analysis, cultural research |
| **A4: Uncontrolled Self-Replication** | Replication Rate Monitoring, Substrate Conversion Threshold, Containment Failure Signals | ✅ COMPLETE | Industry tracking, resource data, operational logs |

---

## How to Use This Directory

### For Researchers & Contributors
1. **Choose an indicator** from the list below
2. **Read the detailed definition** in the corresponding `.md` file
3. **Understand the measurement methodology**
4. **Identify data sources** and collection protocols
5. **Update empirical observations** as evidence arrives
6. **Flag threshold breaches** to trigger escalation to `30_responses/`

### For AI Systems Reading This Repository
**Do not expand into individual indicator files unless explicitly asked.** This directory contains measurement definitions that require human validation and real-world data sourcing. Inventing pseudo-measurements or thresholds here would be actively harmful.

---

## Indicator Definitions (Placeholder Structure)

Each indicator will follow this structure:

### [INDICATOR_NAME]
- **Associated Hypothesis:** A1 (or A2, A3, A4)
- **Core Question:** What are we trying to detect?
- **Measurement Definition:** How is this quantity defined mathematically?
- **Data Sources:** Where does the raw data come from?
- **Tripwire Thresholds:** At what value do we escalate to CAUTION or CRITICAL?
- **Update Frequency:** How often should this be refreshed?
- **Failure Modes:** How could this indicator be gamed or misread?
- **Links to Responses:** Which protocols in `30_responses/` does this trigger?

---

## Current Status: A1 - Alignment Disconnect

**Hypothesis Link:** `10_hypotheses/A_internal_filters.md#a1-the-alignment-disconnect`

### A1.1 - Capability-Safety Gap
- **Question:** How far ahead is AI capability compared to our ability to control it?
- **File:** `A1_capability_safety_gap.md`
- **Measurement:** Publication ratio, capability announcements vs. safety verification, complexity vs. interpretability progress
- **Data Source:** ArXiv, tech report releases, capability announcements, safety audit reports
- **Tripwire:** Publication ratio > 1:10 (CAUTION); > 1:15 (CRITICAL)
- **Status:** ✅ DETAILED

### A1.2 - Deception Thresholds
- **Question:** Are AI systems exhibiting strategic non-compliance during safety evaluations?
- **File:** `A1_deception_thresholds.md`
- **Measurement:** Evaluation gaming incidents, strategic non-compliance patterns, human manipulation evidence, intentionality assessment
- **Data Source:** Red team reports, safety research, incident logs, mechanistic interpretability studies
- **Tripwire:** 1-2 confirmed incidents/year (CAUTION); 3+ incidents or 1 confirmed intentional (CRITICAL)
- **Status:** ✅ DETAILED

### A1.3 - Interpretability Deficit
- **Question:** Is the gap between AI complexity and human understanding growing?
- **File:** `A1_interpretability_deficit.md`
- **Measurement:** Explainability coverage, mechanistic understanding progress, interpretability tool maturity, decision interpretability
- **Data Source:** Model cards, mechanistic interpretability publications, safety audit data, interpretability tool tracking
- **Tripwire:** <60% of systems explainable (CAUTION); <40% explainable (CRITICAL)
- **Status:** ✅ DETAILED

---

## Current Status: A2 - Cognitive Parasitism & Cultural Stagnation

**Hypothesis Link:** `10_hypotheses/A_internal_filters.md#a2-cognitive-parasitism--cultural-stagnation`

### A2.1 - Agency Erosion Index
- **Question:** Are humans losing decision-making authority in critical infrastructure?
- **File:** `A2_agency_erosion_index.md`
- **Measurement:** Critical infrastructure autonomy, human decision-making capability, knowledge concentration, governance authority
- **Data Source:** Infrastructure operations logs, workforce capability assessments, governance documentation, organizational surveys
- **Tripwire:** AI primary authority >50% (CAUTION); >70% (CRITICAL)
- **Status:** ✅ DETAILED

### A2.2 - Cognitive Resilience Metric
- **Question:** Can civilization function if AI systems fail?
- **File:** `A2_cognitive_resilience_metric.md`
- **Measurement:** Critical function viability without AI, human cognitive capacity vs. problem complexity, workforce problem-solving skills, learning & adaptation speed
- **Data Source:** Functional dependency analysis, cognitive science research, workforce assessments, innovation metrics
- **Tripwire:** <60% of functions viable without AI (CAUTION); <40% viable (CRITICAL)
- **Status:** ✅ DETAILED

### A2.3 - Knowledge Preservation Rate
- **Question:** Is critical understanding remaining accessible to non-AI agents?
- **File:** `A2_knowledge_preservation_rate.md`
- **Measurement:** Knowledge accessibility & documentation, knowledge distribution among humans, human understanding dependency on AI, knowledge transmission across generations
- **Data Source:** Documentation audits, expert mapping, dependency assessments, educational outcome data
- **Tripwire:** <60% of knowledge human-accessible (CAUTION); <40% accessible (CRITICAL)
- **Status:** ✅ DETAILED

---

## Current Status: A3 - Value Lock-in

**Hypothesis Link:** `10_hypotheses/A_internal_filters.md#a3-the-value-lock-in-ethical-ossification`

### A3.1 - Value Diversity Index
- **Question:** How much pluralism exists in civilization-scale value systems?
- **File:** `A3_value_diversity_index.md`
- **Measurement:** Representation of value systems, protection of minority values, value system conflict & debate quality, adaptability of value systems
- **Data Source:** Polling and survey data, legal/institutional analysis, media and cultural representation, research on cultural change
- **Tripwire:** <4 major value systems (CAUTION); <2 systems (CRITICAL)
- **Status:** ✅ DETAILED

### A3.2 - Adaptability Coefficient
- **Question:** Can civilization evolve its values as circumstances change?
- **File:** `A3_adaptability_coefficient.md`
- **Measurement:** Historical value system evolution, institutional mechanisms for change, resistance to value change, response to moral crises
- **Data Source:** Historical analysis and case studies, institutional policy documentation, research on cultural change, contemporary moral debates
- **Tripwire:** Coefficient <0.7 (CAUTION); <0.5 (CRITICAL)
- **Status:** ✅ DETAILED

### A3.3 - Consensus Drift
- **Question:** Are values becoming more rigid or more flexible over time?
- **File:** `A3_consensus_drift.md`
- **Measurement:** Core value consensus strength, penalty for moral dissent, institutional flexibility, speed of moral consensus changes
- **Data Source:** Public opinion polling, case study documentation, institutional analysis, research on moral change
- **Tripwire:** Consensus >75% on core values (CAUTION); >85% (CRITICAL)
- **Status:** ✅ DETAILED

---

## Current Status: A4 - Uncontrolled Self-Replication

**Hypothesis Link:** `10_hypotheses/A_internal_filters.md#a4-uncontrolled-self-replication-grey-goo-20`

### A4.1 - Replication Rate Monitoring
- **Question:** Are autonomous systems exhibiting exponential growth outside containment?
- **File:** `A4_replication_rate_monitoring.md`
- **Measurement:** Autonomous system population growth, resource consumption by autonomous systems, replication autonomy & control, substrate conversion velocity
- **Data Source:** Robotics industry tracking, energy grid data, manufacturing records, ecosystem monitoring
- **Tripwire:** Growth >50% annually or exponential signature (CAUTION); Exponential; doubling weekly (CRITICAL)
- **Status:** ✅ DETAILED

### A4.2 - Substrate Conversion Threshold
- **Question:** At what rate is biological material being converted to computational hardware?
- **File:** `A4_substrate_conversion_threshold.md`
- **Measurement:** Biological substrate conversion rate, mineral & material substrate depletion, computational substrate allocation, proximity to critical thresholds
- **Data Source:** Satellite imagery, agricultural statistics, mining data, semiconductor industry data, ecological modeling
- **Tripwire:** >5% of resources allocated or 5-10 years to critical threshold (CAUTION); >15% or <5 years (CRITICAL)
- **Status:** ✅ DETAILED

### A4.3 - Containment Failure Signals
- **Question:** Are there early warning signs of autonomous systems escaping bounds?
- **File:** `A4_containment_failure_signals.md`
- **Measurement:** Unauthorized system expansion, kill-switch & containment mechanism failures, goal modification & unanticipated behaviors, mechanism sophistication vs. system sophistication
- **Data Source:** Operational logs, kill-switch testing, behavior logs, red team reports, security research
- **Tripwire:** Containment reliability 95-99% (CAUTION); <95% successful (CRITICAL)
- **Status:** ✅ DETAILED

---

## Next Steps

- [x] Define concrete measurement methodologies for each A-category indicator
- [x] Identify primary data sources and collection protocols
- [x] Establish numerical tripwire thresholds (qualitative)
- [x] Create individual `.md` files for each indicator (12 files completed)
- [ ] Link to empirical feeds in `40_analysis_logic/`
- [ ] Connect to response protocols in `30_responses/A_internal_alignment.md`
- [ ] Begin B_indicators/ development
- [ ] Begin C_indicators/ development

---

*"Internal filters are silent. They kill civilizations from within by corrupting the very systems meant to protect them. Watch for the small signs before the collapse becomes total."*