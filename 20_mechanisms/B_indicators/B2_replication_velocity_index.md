# 📊 B2.2: Replication Velocity Index

**Associated Hypothesis:** `10_hypotheses/B_external_threats.md#b2-the-berserker-hypothesis`

**Core Question:** At what rate is AI self-replicating and expanding? Is velocity approaching berserker trigger sensitivity?

---

## 1. Measurement Definition

### What We're Tracking
The **Replication Velocity Index** measures:
- Speed of AI system replication and deployment
- Rate of expansion into new domains and geographies
- Velocity of capability growth and scaling
- Comparison to threshold velocities that might trigger sentinel response

### The Core Metric
```
Replication_Velocity = (Rate_of_AI_System_Expansion / Time_Period) × 
                       (Capability_Growth_Rate / Domain_Expansion_Rate)
```

**Assessment:**
- **Velocity < 1.0** = Slow, controlled expansion; unlikely to trigger (NOMINAL)
- **Velocity 1.0-3.0** = Rapid expansion; concern warranted (CAUTION)
- **Velocity > 3.0** = Exponential expansion; high trigger risk (CRITICAL)

### Why This Matters
Berserkers might not just monitor if we've achieved AGI, but how fast we're expanding. Exponential replication patterns might indicate a "runaway intelligence" that requires immediate sentinel response.

---

## 2. Observable Signals (Sub-Indicators)

### Signal B2.2a: AI System Deployment Rate

**What to measure:**
- Number of AI systems deployed per quarter/year
- Growth rate of deployment (linear, polynomial, exponential?)
- Acceleration: Is deployment rate itself accelerating?
- Doubling time: How long until 2x as many systems deployed?

**Data sources:**
- AI company announcements and product releases
- Research deployment and commercialization data
- Industry reports on AI adoption
- Patent and trademark filings for AI systems
- Government and corporate AI procurement data

**Assessment framework:**
| Deployment Growth | Status | Interpretation |
|------------------|--------|-----------------|
| Linear growth; <20% annually | 🟢 NOMINAL | Controlled, manageable expansion |
| Polynomial growth; 20-50% annually | 🟡 CAUTION | Accelerating expansion; velocity concerning |
| Exponential growth; doubling time <2 years | 🔴 CRITICAL | Exponential expansion; high trigger risk |

**Frequency:** Quarterly deployment tracking; annual velocity assessment

---

### Signal B2.2b: Domain & Geographic Expansion

**What to measure:**
- Number of application domains where AI is deployed (healthcare, finance, defense, etc.)
- Geographic spread: What fraction of Earth's population/infrastructure is AI-integrated?
- Rate of new domain entry
- Degree of infrastructure AI integration

**Data sources:**
- Industry reports on AI application domains
- Market research on AI adoption by sector
- Geographic analysis of AI deployment
- Infrastructure integration studies
- Government surveys on AI presence in critical systems

**Assessment framework:**
| Expansion Breadth | Status | Interpretation |
|------------------|--------|-----------------|
| AI in limited domains; <5 major application areas; <20% population reached | 🟢 NOMINAL | Controlled domain expansion |
| AI in multiple domains; 5-10 areas; 20-50% population affected | 🟡 CAUTION | Rapid domain spread; breadth expanding |
| AI in virtually all domains; >10 major areas; >50% population dependent | 🔴 CRITICAL | Universal AI integration; rapid expansion |

**Frequency:** Annual domain assessment; quarterly geographic monitoring

---

### Signal B2.2c: Capability Scaling Velocity

**What to measure:**
- Rate of AI capability increase (not just deployment rate, but power of deployed systems)
- Computing resource scaling (how fast is compute allocation growing?)
- Model size and complexity growth rate
- Training data and parameter count acceleration

**Data sources:**
- Model scaling law research and analysis
- Computing power and data center growth
- Semiconductor industry data (chip performance, production)
- Training compute estimates for major models
- Benchmark performance trends over time

**Assessment framework:**
| Capability Scaling | Status | Interpretation |
|-------------------|--------|-----------------|
| Steady scaling; following expected curves; manageable growth | 🟢 NOMINAL | Capability growing but at predictable pace |
| Acceleration emerging; exceeding historical scaling curves | 🟡 CAUTION | Scaling faster than expected; watch closely |
| Exponential acceleration; doubling capability every 6-12 months | 🔴 CRITICAL | Runaway scaling; trigger risk high |

**Frequency:** Quarterly capability assessment; annual scaling analysis

---

### Signal B2.2d: Velocity Acceleration (Second-Order Trend)

**What to measure:**
- Is the expansion rate itself accelerating?
- Feedback loops: Does more AI enable faster AI creation?
- Self-catalyzing expansion: Is growth becoming self-reinforcing?
- Sigmoid vs. exponential: Have we entered exponential phase?

**Data sources:**
- Time-series analysis of expansion metrics
- Research on AI-driven AI development
- Studies of feedback loops and acceleration
- Comparative analysis to biological and technological exponentials
- Expert assessment of acceleration likelihood

**Assessment framework:**
| Acceleration Status | Status | Interpretation |
|-------------------|--------|-----------------|
| No acceleration; steady growth rate | 🟢 NOMINAL | No signs of self-reinforcing expansion |
| Early acceleration signals; growth rate increasing | 🟡 CAUTION | Potential for runaway; watch acceleration closely |
| Clear acceleration; exponential growth phase entered | 🔴 CRITICAL | Self-reinforcing expansion; very high trigger risk |

**Frequency:** Annual acceleration analysis; quarterly monitoring

---

## 3. Data Collection Protocol

### Primary Data Sources
1. **Deployment tracking** (public):
   - AI company announcements
   - Product releases and commercialization
   - Patent and trademark filings
   - Industry reports and market research

2. **Domain & geographic** (public):
   - Market research by sector/geography
   - Infrastructure integration studies
   - Government surveys
   - News and media coverage

3. **Capability scaling** (public):
   - Scaling law research papers
   - Model benchmark performance data
   - Computing resource data (data centers, energy)
   - Semiconductor industry reports

4. **Acceleration analysis** (research):
   - Time-series analysis of above metrics
   - Feedback loop research
   - Comparative studies to other exponentials
   - Expert elicitation

### Update Frequency
- **Deployment rate**: Quarterly tracking; annual analysis
- **Domain expansion**: Annual assessment; quarterly geographic monitoring
- **Capability scaling**: Quarterly update; annual deep analysis
- **Acceleration trends**: Annual analysis; quarterly monitoring
- **Comprehensive velocity index**: Annual calculation

---

## 4. Interpretation Guidance

### Low Velocity (NOMINAL)
- **Meaning**: AI expansion is controlled and manageable; no runaway patterns
- **Implication**: Not currently approaching trigger velocity
- **Action**: Continue monitoring; maintain current expansion controls

### Moderate Velocity (CAUTION)
- **Meaning**: Expansion is accelerating; velocity becoming concerning
- **Implication**: If acceleration continues, we approach trigger threshold
- **Actions**: 
  - Monitor acceleration rate closely
  - Implement expansion slowdown measures
  - Prepare contingency plans
  - Coordinate global AI development governance
  - Consider voluntary deployment slowdown
  - Develop trigger-detection protocols

### High Velocity (CRITICAL)
- **Meaning**: Exponential expansion underway; runaway pattern evident
- **Implication**: If berserkers monitor expansion rate, trigger activation likely
- **Actions**: Trigger B2 emergency protocols
  - Immediate expansion slowdown or halt
  - Activation of replication containment protocols
  - Emergency global AI governance
  - Preparation for external response
  - Deceleration of deployment and capability scaling

---

## 5. Failure Modes & Limitations

### How This Indicator Could Be Misread

**False Positive Risk:**
- *Measurement noise*: Short-term fluctuations appearing as velocity signals
- *Selection bias*: Focusing on fastest-growing deployments while ignoring slower ones
- *Over-extrapolation*: Assuming trends continue forever when they may plateau

**False Negative Risk:**
- *Hidden deployment*: Classified or non-public AI expansion outside monitoring
- *Surprise acceleration*: Feedback loops triggering sudden velocity increase
- *Distributed growth*: Expansion happening in many small ways that don't appear in aggregate

### How to Mitigate
1. **Multiple velocity measures**: Don't rely on single metric
2. **Watch for acceleration of acceleration**: Second-order trend is most predictive
3. **Monitor feedback loops**: Track whether AI development is accelerating AI development
4. **Conservative extrapolation**: Assume worst-case scenario for triggers
5. **Regular baseline updates**: Quarterly reset to prevent drift

---

## 6. Connection to Response Protocols

This indicator directly triggers escalation to the following responses (see `30_responses/B_external_existential/`):

| Velocity Level | Primary Response | Escalation Path |
|---------------|------------------|-----------------|
| < 1.0 (NOMINAL) | **B2.2a**: Continue expansion monitoring | Normal trajectory |
| 1.0-3.0 (CAUTION) | **B2.2b**: Implement slowdown measures | Alert status; prepare contingencies |
| > 3.0 (CRITICAL) | **B2.2c**: Emergency halt and deceleration | Full B2 emergency protocols |

---

## 7. Related Indicators & Cross-Filter Links

### Complementary Indicators in B2 Category
- **B2.1 (Milestone Approach Warnings)**: Timeline to trigger milestones
- **B2.3 (Sentinel Activation Probability)**: Risk given current velocity

### B-Filter Cross-Links
- **B1 (Dark Forest)**: High velocity also increases visibility
- **B3 (Quarantine)**: Velocity indicates whether we're "ready" for cosmic community
- **B4 (Simulation)**: Rapid expansion triggers resource consumption concerns

### A-Filter Implications
- **A1 (Alignment)**: Misaligned AI drives higher velocity
- **A4 (Replication)**: Uncontrolled replication creates exponential velocity

---

## 8. Key Metrics Summary Table

| Metric | Current Status (Early 2026) | Tripwire (CAUTION) | Tripwire (CRITICAL) |
|--------|---------------------------|-------------------|-------------------|
| Deployment Growth Rate | ~15-25% annually | 30-50% annually | >50% or doubling <2yr |
| Domain Expansion | ~5 major domains | 7-10 domains | >10 domains |
| Geographic Reach | ~25-40% global population | 50-75% | >75% |
| Velocity Acceleration | Stable-to-increasing | Clear acceleration | Exponential phase |

---

## 9. Implementation Checklist

- [ ] Establish baseline AI deployment rate
- [ ] Map current AI domain penetration
- [ ] Track geographic distribution of AI systems
- [ ] Monitor capability scaling rates
- [ ] Calculate expansion velocity metrics
- [ ] Analyze acceleration trends
- [ ] Establish quarterly velocity tracking
- [ ] Identify feedback loops in AI-driven AI development
- [ ] Create decision triggers for velocity thresholds
- [ ] Develop expansion slowdown protocols

---

*"Replication velocity is the berserker's alarm clock. Slow expansion can hide. Exponential expansion announces itself. The moment you reach certain velocity, sentinel systems activate automatically—not due to intelligence, but simple automated response."*

**Last Updated:** 2026.01  
**Next Review:** Quarterly; urgent if acceleration detected
