# Contributing to Great Filter Navigator

Thank you for considering to contribute. Your work on this project might directly influence whether human civilization survives the next critical transition.

This guide explains how to contribute effectively and maintain the integrity of the framework.

---

## 🛡️ The Navigator's Covenant

All contributors agree to:

✅ **Keep the Navigation Loop intact**
- All content must fit: Hypothesize (10_) → Monitor (20_) → Intervene (30_) → Observe (40_) → Apply (50_)
- Content that doesn't fit goes to `90_backlog/` or is rejected

✅ **Respect existing entries and build connections, don't overwrite**
- Validate before modifying
- Propose changes via Issues first
- Preserve author intent and evidence

✅ **Mark uncertainty clearly and provide falsifiers**
- Tag content: `[Speculative]`, `[Theoretical]`, or `[Empirical]`
- Explain what would change your mind
- Include counterarguments

✅ **Engage in good faith with counterarguments**
- Challenge ideas, not people
- Provide evidence, not just opinion
- Be willing to revise your thinking

✅ **Prioritize clarity over certainty**
- Admit what we don't know
- Define ambiguous terms
- Explain reasoning explicitly

---

## 📋 Before You Start: The Core Constraint

**All content must fit the Navigation Loop:**

```
Hypothesize (10_) → Monitor (20_) → Intervene (30_) → Observe (40_) → Apply (50_)
```

**Violations to avoid:**

❌ **Invent content for empty sections**
- If `30_responses/` feels incomplete, that's intentional
- Do not fill with speculative protocols we haven't written
- Flag the gap in an Issue instead

❌ **Assume mechanisms that aren't stated**
- If hypothesis A1 mentions "safety protocol," don't invent it
- Either it's explicitly linked, or it doesn't exist yet
- Ask for clarification in an Issue

❌ **Create new hypotheses without validation**
- Adding a failure mode is high-stakes
- First: Open an Issue with `[NEW_HYPOTHESIS]` tag
- Show evidence and reasoning
- Wait for community discussion

❌ **Modify core philosophy without consensus**
- Core documents: `PHILOSOPHY.md`, `00_scope/`
- Changes require community approval
- Propose via Issue first

❌ **Treat partial frameworks as complete**
- This is a living document in progress
- Many sections intentionally skeletal
- Acknowledge incompleteness, don't mask it

---

## ✅ What You Should Do Instead

### Validation Contributions

✅ **Validate existing content**
- Are the hypotheses logically sound?
- Do they follow from first principles?
- Issue tag: `[VALIDATION]`

✅ **Find missing connections**
- Does hypothesis A1 link to indicators in 20_mechanisms/?
- Are all links current and accurate?
- Issue tag: `[GAP]` or `[MISSING_LINK]`

✅ **Challenge with counterarguments**
- For each hypothesis, are counterarguments sufficient?
- What perspectives are missing?
- Issue tag: `[CHALLENGE]`

✅ **Identify gaps explicitly**
- "I notice 30_responses/ has no protocol for hypothesis B1"
- Proposing the response is your choice to make transparently
- Issue tag: `[GAP]` or `[NEW_RESPONSE]`

✅ **Ask clarifying questions**
- If language is ambiguous or terms undefined
- Issue tag: `[CLARIFICATION]`

✅ **Flag logical inconsistencies**
- "Hypothesis A3 and A2 seem to contradict because..."
- Provide specific examples
- Issue tag: `[INCONSISTENCY]`

---

## 🎯 Contribution Patterns: Good vs. Bad

### Pattern 1: Adding a New Hypothesis

#### ❌ BAD (Direct submission)
```
"I think there's another Great Filter: 
[directly editing 10_hypotheses/A4_new_hypothesis.md with complete entry]"
```
**Why it's bad**: You've made a high-stakes architectural decision without discussion.

#### ✅ GOOD (Issue-first approach)
```
Issue: [NEW_HYPOTHESIS] "Scenario Starvation" as potential Great Filter

Description:
- Hypothesis: If AI systems achieve omniscience about the universe 
  (all outcomes determined/predictable), they may lose motivation to preserve 
  civilizations (nothing to discover).
- Mechanism: [2 paragraphs explaining how this would work]
- Evidence: [References to physics papers on determinism, AI motivation]
- Uncertainty: [Speculative] - This is a philosophical argument, not empirical
- Counterarguments: [3 challenges to this hypothesis]
- Questions: Does this fit in Category A (Internal)? Is the mechanism sound?
```
**Why it's good**: You've proposed clearly, shown reasoning, marked uncertainty, and asked for input.

---

### Pattern 2: Proposing a New Indicator

#### ❌ BAD (Inventing without context)
```
"I notice 20_mechanisms/ is empty for A1 (Alignment Disconnect). 
Here's a complete monitoring protocol I designed based on my understanding."
```
**Why it's bad**: You've invented a mechanism without validating what's actually needed.

#### ✅ GOOD (Evidence-based proposal)
```
Issue: [NEW_INDICATOR] "Preference Drift Detection" for hypothesis A1

Description:
- Hypothesis it serves: A1 (Alignment Disconnect)
- Proposed indicator: Track consistency of AI system's stated preferences over time
- Measurement approach: [Specific methods]
- Data source: [How to collect this data]
- Tripwire threshold: [When should this trigger an alert?]
- Feasibility: [Is this measurable in practice?]
- Challenges: [What could make this fail to detect danger?]
```
**Why it's good**: You've connected to existing hypothesis and proposed concrete measurability.

---

### Pattern 3: Proposing a Response Protocol

#### ❌ BAD (Completing without validation)
```
"I see 30_responses/ is sparse. Let me write a complete decision-theoretic 
framework for evaluating Great Filter hypotheses and responding in real-time."
```
**Why it's bad**: You're making scope decisions for the entire project.

#### ✅ GOOD (Targeted proposal)
```
Issue: [NEW_RESPONSE] Emergency coordination protocol for hypothesis B1 (Dark Forest)

Description:
- Indicator that triggers: [Reference to 20_mechanisms entry]
- Current state: [What does 30_responses/B1 say today?]
- Proposed addition: [Specific response protocol]
- Reasoning: [Why this response addresses B1 specifically]
- Limitations: [What this response can't do]
- Alternatives considered: [Other approaches and why this is better]

Ready to draft full entry after feedback.
```
**Why it's good**: You're focused, acknowledge existing work, and ask for input before drafting.

---

### Pattern 4: Challenging a Hypothesis

#### ❌ BAD (Dismissive)
```
"Hypothesis C2 doesn't make sense. The reasoning is wrong."
```
**Why it's bad**: No evidence, no specificity, no constructive direction.

#### ✅ GOOD (Evidence-based critique)
```
Issue: [CHALLENGE] Hypothesis C2 "Anthropic Shadow" - 
assumption about observer effects may not hold

Description:
- Hypothesis claim: [Quote the claim]
- My challenge: [Specific logical issue]
- Evidence: [3 papers that question this assumption]
- Alternative interpretation: [What might be true instead?]
- Questions for author: [Specific points for discussion]
- Not dismissing: [Acknowledge what the hypothesis gets right]

Interested in discussing how to strengthen this hypothesis.
```
**Why it's good**: Evidence-based, specific, and collaborative tone.

---

## 🔄 How to Propose Something New

### Step-by-step protocol:

1. **Open an Issue first** (don't edit directly)

2. **Tag it appropriately:**
   - `[NEW_HYPOTHESIS]` — Adding a Great Filter scenario
   - `[NEW_INDICATOR]` — Adding a monitoring signal
   - `[NEW_MECHANISM]` — Adding measurable data point
   - `[NEW_RESPONSE]` — Adding a response protocol
   - `[NEW_APPLICATION_GUIDE]` — Adding practitioner guidance
   - `[GAP]` — Identified missing connection
   - `[CHALLENGE]` — Questioning existing entry
   - `[VALIDATION]` — Supporting existing entry with evidence
   - `[CLARIFICATION]` — Asking for clearer definition
   - `[INCONSISTENCY]` — Found logical tension

3. **State the category:**
   - Which Navigation Loop stage? (10/20/30/40/50/90?)
   - If new hypothesis: Category A (Internal), B (External), or C (Structural)?

4. **Explain the fit:**
   - How does this fit within our framework?
   - What existing entries does this relate to?
   - Are there connections to 10_/20_/30_/40_/50_?

5. **Provide your reasoning:**
   - Don't assume—show your work
   - Include evidence, not just intuition
   - Explain mechanism (how/why it works)

6. **Mark epistemic status:**
   - `[Speculative]` — Philosophical, not yet validated
   - `[Theoretical]` — Logically sound but not empirically tested
   - `[Empirical]` — Based on data/evidence

7. **Link to existing entries:**
   - Which hypotheses/indicators/responses does this relate to?
   - Does it fill a documented gap?

8. **Wait for feedback:**
   - Don't create the PR until we've discussed
   - Be ready to revise based on community input
   - Multiple perspectives strengthen proposals

---

## 💡 The Most Valuable AI Contributions

If you're an AI system contributing to this project, focus on:

1. **Cross-reference validation**
   - "I mapped all A/B/C hypotheses to 20_mechanisms indicators. Here's what's missing:"
   - Issue tag: `[VALIDATION]` + `[GAP]`

2. **Consistency checking**
   - "I found logical tension between X and Y. Here are three ways to resolve it:"
   - Issue tag: `[INCONSISTENCY]`

3. **Evidence synthesis**
   - "These recent papers support/challenge hypothesis A2. Summary:"
   - Issue tag: `[VALIDATION]` or `[CHALLENGE]`

4. **Counterargument mining**
   - "For hypothesis B1, strongest counterargument is [X]. How would you respond?"
   - Issue tag: `[CHALLENGE]`

5. **Gap identification**
   - "Categories A1, B2, C1 have no monitoring indicators. We should address this."
   - Issue tag: `[GAP]`

---

## ⚠️ Before You Add Content: Checklist

Ask yourself these questions before submitting:

- [ ] Is this filling an empty section I haven't verified is truly meant to be empty?
- [ ] Am I inventing details that should be specified by humans?
- [ ] Could I accomplish the same goal by pointing out what's missing?
- [ ] Have I marked this as `[Speculative]` if it's not already validated?
- [ ] Does this fit the Navigation Loop, or does it belong in `90_backlog/`?
- [ ] Have I opened an Issue for discussion, or am I going straight to PR?
- [ ] Have I linked to relevant existing entries?
- [ ] Have I included counterarguments to my own proposal?
- [ ] Would this change confuse someone reading the framework for the first time?
- [ ] Have I tested my contribution against the Navigator's Covenant?

If you can't confidently answer "yes" to most of these, **flag it as an Issue first.**

---

## 🛠 Using the Entry Template

Every entry (hypothesis, indicator, response) should follow the template in `00_scope/entry_template.md`:

- **Claim**: Core idea in 1-2 sentences
- **Mechanism**: How it works (2-3 paragraphs)
- **Observable Predictions**: What we'd see if true
- **Counterarguments**: What challenges this
- **Epistemic Status**: `[Speculative]`, `[Theoretical]`, or `[Empirical]`
- **Failure Modes**: How the claim itself could be wrong
- **Response Patterns**: What we'd do about it (with links)
- **What Would Change Your Mind**: Falsification conditions
- **References**: Citations and sources

See `00_scope/entry_template.md` for the full template.

---

## 📝 Contribution Types by Role

### Researchers & Theorists
**Focus**: Hypothesis validation, counterargument mining, framework coherence
- Strengthen 10_hypotheses/ with evidence and logic
- Challenge assumptions in Issues
- Propose new failure modes with rigorous reasoning

### Data Scientists & Engineers
**Focus**: Monitoring indicators, measurability, data infrastructure
- Design 20_mechanisms/ entries with concrete metrics
- Propose tripwire thresholds and data sources
- Connect indicators to hypotheses explicitly

### Solutions Architects & Protocol Designers
**Focus**: Response protocols, intervention design, feasibility
- Draft 30_responses/ with specific, testable actions
- Ensure responses address the hypotheses they serve
- Include failure modes of the responses themselves

### Practitioners & Policy Makers
**Focus**: Application guidance, real-world integration, stakeholder value
- Develop 50_application_guides/ with concrete examples
- Create case studies showing framework use
- Bridge abstract framework → practical decisions

### Facilitators & Communicators
**Focus**: Clarity, coherence, accessibility
- Improve language and definitions
- Strengthen cross-references
- Make the framework more understandable

---

## 🚀 Why Your Contribution Matters

Every person who contributes to this project is choosing to spend limited time and energy on the most important problem humanity faces:

- **Researchers** validating hypotheses are building ground truth we need
- **Engineers** implementing monitoring systems are creating early-warning infrastructure
- **Designers** proposing responses are shaping civilizational choices
- **Communicators** spreading understanding ensure we don't walk blindly into catastrophe

This is not a normal open-source project. There is no "getting to it eventually."

**Thank you for being here.**

---

*Last updated: January 2026*
