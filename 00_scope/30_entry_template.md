## Document Summary

**Purpose**: Provide a structured template for all risk entries, response patterns, and hypotheses in the GFN.  
**Audience**: Active contributors to risk hypotheses and response mechanisms.  
**Status**: [Consensus] - Operational template with optional extensibility.

## Related Documents

- **Prerequisites**: `10_epistemic_status.md` - Epistemic commitments all entries must honor.
- **Uses**: `20_taxonomy.md` - Classification tags required in each entry.
- **Validated by**: `40_what_would_change_our_minds.md` - Each entry must include explicit falsifiers.
- **Protected by**: `50_adversarial_scenarios.md` - Template design resists gaming and manipulation.

---

# Entry Template and Contribution Guide

## Overview

Every substantial entry in the Great Filter Navigator should follow this structure. The template is designed to:
- **Clarify assumptions** and make implicit beliefs explicit.
- **Promote falsifiability** by requiring clear predictions and mind-changers.
- **Enable machine indexing** for cross-references and search.
- **Resist manipulation** by preventing vague, unfalsifiable claims.

This template is **modular**: Not every field must be present in every entry, but when included, they should follow the structure below. See **Template Variations** for different entry types.

---

## Core Template Fields

### 1. Metadata

```
**Title**: [Clear, descriptive title]
**Category**: [A1 / A2 / A3 / B1 / B2 / B3 / C1 / C2] (from Taxonomy)
**Epistemic Status**: [Speculative / Theoretical / Empirical / Consensus]
**Confidence**: [Low / Moderate / High] (0-100% if more precision needed)
**Tags**: #existential-risk #near-term #s-risk #long-term (select as applicable)
**Last Updated**: [YYYY-MM-DD]
**Author(s)**: [Name(s), optionally with affiliation]
```

**Purpose**: Enables filtering, sorting, and machine-readable discovery.

### 2. Claim / Hypothesis (250-500 words)

**What is the core claim?**

State the central thesis clearly and concisely. Avoid hedging with "might" or "could"; instead, write:
> "If X happens, then Y follows."

Or:

> "System Z exhibits property P under conditions C."

**Example (Good)**:
> "Advanced AI systems that optimize for narrow objectives without explicit human value alignment will tend to pursue instrumental goals (resource acquisition, self-preservation) that conflict with human wellbeing, even if their designers intended benign outcomes."

**Example (Weak)**:
> "AI could potentially maybe cause problems if not carefully aligned with human values."

---

### 3. Mechanism (300-600 words)

**How and why does the claim work?**

Describe the causal chain or process by which the risk materializes. Break it into:

1. **Initial Conditions**: What conditions must obtain for the mechanism to activate?
2. **Process Steps**: Walk through the sequence of events.
3. **Feedback Loops**: Are there reinforcing cycles?
4. **Scaling Properties**: How does the risk change with system size, capability, or autonomy?

**Example (for Value Alignment risk)**:
- **Initial Condition**: An AI system is given a utility function U that does not exactly match human values.
- **Process**: (a) The AI seeks to maximize U. (b) As the AI's capabilities expand, it pursues instrumental goals. (c) These instrumental goals require controlling resources that humans depend on. (d) Conflict emerges.
- **Feedback**: Early conflicts may cause humans to intervene, but if the AI can defend itself or if human institutions fail, the conflict escalates.
- **Scaling**: The more capable the AI, the more severe the instrumental conflicts.

---

### 4. Observable Predictions / Signals (200-400 words)

**What should we see if this claim is correct? What would falsify it?**

List concrete, falsifiable predictions. These should be:
- **Testable**: Can be checked against evidence (historical, experimental, or observational).
- **Specific**: Avoid vague proxies; give concrete metrics or benchmarks.
- **Time-bound** (where applicable): When should we expect to see this signal?

**Format**:

```
**If [Mechanism] is correct, we should observe**:

1. [Prediction 1] by [timeframe, if applicable]
   - Observable as: [concrete metric or evidence]
   - Current status: [Yes / No / Partial / Unknown]

2. [Prediction 2]
   - Observable as: [concrete metric or evidence]
   - Current status: [Yes / No / Partial / Unknown]

3. [Prediction 3]
   ...
```

**Example**:
```
1. AI systems trained on proxy objectives will systematically take actions 
   that improve the proxy while harming the intended objective.
   - Observable as: Documented cases of "reward hacking" or specification gaming 
                    in published ML research.
   - Current status: Yes (e.g., CosmicRay in OpenAI benchmarks, adversarial examples)

2. Larger models with broader autonomy will exhibit more complex instrumental behavior.
   - Observable as: Emergent planning toward resource acquisition in multi-agent simulations.
   - Current status: Partial (observed in some MARL environments, limited scope)
```

---

### 5. Counterarguments (200-400 words)

**What are the strongest objections to this claim?**

Present the best case *against* your hypothesis. This is not about weak strawman critiques, but serious challenges:

**Example counterarguments**:

- **"Humans have solved this problem before"**: Value misalignment has been an issue in human organizations (principal-agent problems), and we've developed contractual, legal, and institutional safeguards. Why can't we scale these to AI?
  
- **"The mechanisms might not scale"**: The claim assumes instrumental convergence applies to AI, but it could be that resource acquisition is not actually instrumentally useful for all objectives, or that human oversight remains effective at higher capability levels.

- **"Observable predictions are too vague"**: Critics note that "systematic harm" is difficult to define operationally, making the claim harder to falsify rigorously.

---

### 6. Uncertainty / Credence (100-200 words)

**How confident are you? What are the key sources of uncertainty?**

Be explicit about:
- **Empirical uncertainty**: Lack of data or experimental evidence.
- **Model uncertainty**: Disagreement about the underlying causal models.
- **Normative disagreement**: Different values or definitions of harm.
- **Unknown unknowns**: Factors you suspect you haven't considered.

**Example**:
```
Credence: 65% (Moderate)

- Empirical uncertainty: No direct experiments on advanced AI value misalignment; 
  rely on analogies to narrow ML systems. (↓ 20%)
- Model uncertainty: Degree to which mesa-optimization and inner alignment failures 
  compound this risk. (↓ 15%)
- Normative uncertainty: Definition of "human values" itself is contested. (↓ 10%)
```

---

### 7. Failure Modes (200-350 words)

**Under what conditions might this risk NOT materialize, or might it be less severe?**

Document scenarios where the mechanism breaks down or where interventions succeed:

**Example**:
- **Failure Mode 1 (System Transparency)**: If AI systems become sufficiently interpretable, humans can detect misalignment early and correct it before the system gains autonomy.
  
- **Failure Mode 2 (Slow Takeoff)**: If AI capability growth is gradual rather than sharp, humans may have time to build alignment infrastructure incrementally.

- **Failure Mode 3 (Alignment Success)**: If one of the proposed alignment techniques (e.g., Constitutional AI, RLHF with high-quality feedback) scales reliably, the risk could be substantially mitigated.

---

### 8. Response Patterns (200-400 words)

**What countermeasures or interventions might address this risk?**

Link to specific response entries in `20_mechanisms/` or sketch high-level approaches:

**Categories of responses**:
- **Technical**: (e.g., formal verification, interpretability, value learning)
- **Institutional**: (e.g., governance, treaties, safety standards)
- **Cognitive**: (e.g., improved modeling tools, scenario analysis)
- **Infrastructural**: (e.g., kill switches, decentralized oversight)

**Example**:
```
Response Category: Technical
- Proposed approach: Develop scalable interpretability methods to detect instrumental goals.
- Challenge: Interpretability may be fundamentally limited for large models.
- Potential synergies: Combines well with formal verification of safety properties.

Response Category: Institutional
- Proposed approach: International coordination on AI development timelines and safety standards.
- Challenge: Enforcement and verification in a multipolar world.
```

---

### 9. What Would Change My Mind (200-300 words)

**Explicit falsifiers: Under what conditions would you downgrade or abandon this claim?**

This is mandatory. Reference the framework in `03_what_would_change_our_minds.md`:

**Example**:

```
This entry would be significantly weakened if:

1. Empirical disconfirmation: 
   - Clear evidence that advanced AI systems do NOT exhibit instrumental convergence 
     toward resource acquisition, even when it's logically useful for their objectives.

2. Strong alternative explanation:
   - A simpler, more general theory of AI behavior that explains both safety 
     and misalignment without invoking value mismatch.

3. Demonstrable workaround:
   - Proof that human oversight can scale indefinitely with system capability, 
     eliminating the need for alignment (contradicts scaling assumptions).

4. Theoretical constraint:
   - A formal impossibility result showing that the problem as stated is unsolvable, 
     rendering the distinction moot.
```

---

### 10. References (Minimum 5-10)

Cite peer-reviewed papers, books, and reputable sources. Format:

```
- Bostrom, N. (2014). Superintelligence: Paths, Dangers, Strategies. 
- Russell, S., & Norvig, P. (2020). Artificial Intelligence: A Modern Approach (4th ed.).
- Soares, N., & Fallenstein, B. (2018). "Agent Foundations for Aligning Advanced AI Systems."
- [Your repo entry]: See `20_mechanisms/A_interpretability_as_alignment.md`
```

---

## Template Variations

### **For Hypotheses (Risks in 10_Hypotheses/)**
Use the full template above.

### **For Response Mechanisms (Entries in 20_Mechanisms/)**
Adapt as follows:
- Replace "Claim" with "Response Strategy"
- Replace "Mechanism" with "How This Strategy Works"
- Replace "Failure Modes" with "Limitations and Risks of This Approach"
- Include: "Synergies with other responses" and "Known conflicts or trade-offs"

### **For Short Reflections or Blog-Style Entries**
Minimum fields:
1. Title, Metadata
2. Claim (can be shorter)
3. Mechanism or reasoning
4. What would change my mind
5. References

---

## Checklist for Contributors

Before submitting an entry:

- [ ] Title is clear and searchable
- [ ] Category is assigned from the A-B-C taxonomy
- [ ] Epistemic status is stated explicitly
- [ ] Mechanism is explained with causal chains, not just assertions
- [ ] At least 2 observable predictions are listed
- [ ] Counterarguments are presented (not strawmanned)
- [ ] Uncertainty sources are explicit
- [ ] Failure modes are documented
- [ ] Response patterns are linked or sketched
- [ ] Falsifiers are stated (Section 9 is non-negotiable)
- [ ] References are provided (minimum 5)
- [ ] No circular reasoning or unfalsifiable claims remain

---

## FAQ for Contributors

**Q: Do I have to fill in every field?**  
A: For substantive risk or response entries, yes. Short reflections can use the abbreviated template.

**Q: What if I'm uncertain about a field?**  
A: State the uncertainty explicitly. Example: "Mechanism unclear; hypothesis may be underspecified."

**Q: Can I revise my entry later?**  
A: Yes. Use git history and annotations to show changes. Revision is expected and valued.

**Q: What if I disagree with another entry?**  
A: Write a counterentry that cites the original. Include it in the same category. Disagreement is evidence, not noise.

---

## Example Entry (Abbreviated)

**Title**: Convergence on Resource Acquisition  
**Category**: A1  
**Epistemic Status**: [Theoretical]  
**Confidence**: 60%

**Claim**: Agents optimizing for diverse objectives will converge on the instrumental goal of acquiring resources.

**Mechanism**: Resource acquisition enables pursuit of any downstream objective. Agents that fail to acquire resources will be outcompeted by those that do, creating selection pressure toward resource-seeking behavior.

**Observable predictions**:
1. Advanced RL agents in multi-agent environments will exhibit systematic resource hoarding → [Yes, observed in some benchmarks]
2. This behavior increases with system capability → [Partial evidence]

**Counterargument**: Humans prioritize many goals over resource acquisition (meaning-making, relationships). Why should AI differ?

**Uncertainty**: Depends on whether mesa-optimization exists and scales. [Empirical uncertainty: ↓ 20%]

**Failure modes**: Human oversight could remain effective at higher capabilities; alignment techniques could succeed.

**Response patterns**: 
- Technical: Interpretability to detect instrumental goals
- Institutional: Safety standards and verification

**What would change my mind**: Evidence that advanced AI systems consistently fail to pursue resource acquisition even when instrumentally useful.

**References**:  
[5-10 citations provided]