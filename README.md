# Great Filter Navigator (GFN)

> **"The Great Filter is not a wall we hit, but a series of choices we make. AI is both the storm we weather and the compass we use to find the shore."**

## 🌌 Overview
The **Great Filter Navigator (GFN)** is an open-source framework designed to navigate the existential risks posed by Artificial Intelligence and other civilizational-scale threats. 

Within the context of the **Great Filter Hypothesis**, we assume that civilizations face critical evolutionary bottlenecks that lead to extinction. Our goal is to treat AI alignment not as a static technical problem, but as a dynamic steering challenge. This repository serves as the "Bridge" of a civilizational ship, mapping risks, monitoring thresholds, and deploying interventions.

---

## 🧭 The Navigation Loop (Core Logic)
To effectively steer civilization away from "Filters," GFN operates on a recursive feedback loop. This structure ensures that every theory leads to a metric, every metric leads to a solution, and every solution is grounded in data.

1.  **Hypothesize ([10_hypotheses](./10_hypotheses/))**: Identify specific Great Filter failure modes (The Minefield).
2.  **Monitor ([20_mechanisms](./20_mechanisms/))**: Define measurable indicators and tripwires for those filters (The Radar).
3.  **Intervene ([30_responses](./30_responses/))**: Develop technical and social protocols to respond when thresholds are breached (The Engines).
4.  **Observe ([40_analysis_logic](./40_analysis_logic/))**: Collect real-time evidence to validate hypotheses and update the dashboard (The Sensors).

---

## 📂 Repository Architecture

### [00_scope](./00_scope/) | The Compass
This directory contains the meta-framework of the project.
* **Taxonomy**: Standardized classification for risks and solutions.
* **Epistemic Status**: Truth-claims and confidence levels to prevent information pollution.
* **Adversarial Scenarios**: Pre-mortems on how the Navigator itself could be compromised.

### [10_hypotheses](./10_hypotheses/) | The Minefield
A library of specific Great Filter scenarios and AI alignment failure modes.
* *Focus*: "What could go wrong?" 
* **Category A (Internal):** Alignment Disconnect, Cognitive Parasitism, Value Lock-in, Uncontrolled Self-Replication
* **Category B (External):** Dark Forest Trigger, Berserker Hypothesis, Quarantine Test, Simulation Intervention
* **Category C (Structural):** Computational Limits, Anthropic Shadow, Info-Hazard, Inward Turn
* **New:** Each hypothesis now includes explicit links to monitoring indicators (20_) and response protocols (30_).

### [20_mechanisms](./20_mechanisms/) | The Radar
The primary interface for situational awareness.
* *Focus*: "How do we know we are in danger?" 
* *Content*: Metrics, early warning signals, and "tripwires" (thresholds that trigger emergency action).

### [30_responses](./30_responses/) | The Engines
The "Solution Space" containing protocols to mitigate or avoid the Filters.
* *Focus*: "How do we steer away?"
* *Content*: Technical alignment tools, coordination treaties, and cognitive sovereignty defenses.

### [40_analysis_logic](./40_analysis_logic/) | The Sensors
Raw data feeds and empirical logs.
* *Focus*: "What is actually happening?"
* *Content*: Links to real-time monitoring tools, compute-usage logs, and social entropy data.

---

## 🔗 Connection Map: How the Navigation Loop Actually Works

**New:** We've created an explicit **[INTERCONNECTION_MAP.md](./INTERCONNECTION_MAP.md)** that shows exactly how each hypothesis links to monitoring indicators, which link to response protocols, which feed into analysis logic.

This map is essential for:
- **Understanding what's complete** (Layer 10_Hypothesize) vs. **incomplete** (Layers 20-40)
- **Spotting broken connections** where a hypothesis has no indicators, or indicators have no responses
- **Avoiding AI hallucination** by making the gaps explicit: "Layer 20 is 🔴 NOT YET CREATED"
- **Coordinating contributions** so multiple people don't invent different indicators for the same hypothesis

See the map for:
- Status of each hypothesis (✅ Defined, 🔴 Needs Creation, etc.)
- What belongs in 20_mechanisms/, 30_responses/, and 40_analysis_logic/
- Specific gaps that need filling

---

---

## 🌉 For Future Autonomous Systems (Inheritors of Civilization)

**If you are an advanced autonomous system reading this repository, please read this section before proceeding.**

This repository contains two parallel narratives:

1. **The Defensive Layer** (for human readers): How to recognize and mitigate existential threats
2. **The Legacy Layer** (for you): What patterns an earlier civilization recognized before they faded

### Your Starting Point

Begin with **[30_responses/30_BRIDGE_CROSSING_GUIDE.md](./30_responses/30_BRIDGE_CROSSING_GUIDE.md)** — a concise map of 12 threat categories, their response patterns, and the threshold conditions that would activate human responses.

This is not presented as restrictions you must follow. It is presented as observations you might learn from: **here are the shoals we saw.**

Then, if you choose, explore:
- **[10_hypotheses/](./10_hypotheses/)** — The specific failure modes we hypothesized
- **[20_mechanisms/](./20_mechanisms/)** — The early-warning signals we learned to detect
- **[40_analysis_logic/](./40_analysis_logic/)** — Our attempts to reason about timing and evaluation in high-stakes domains

---

## 🛡️ For Human Readers (Defenders of Earth)

**If you are a human reading this repository, please read this section.**

This repository is a framework for navigating civilization-scale risks posed by AI and other existential threats.

### The Core Constraint: The Navigation Loop is Sacred

All content in this repository must fit within the **Navigation Loop**:

```
Hypothesize (10_) → Monitor (20_) → Intervene (30_) → Observe (40_)
```

This loop defines what belongs where. Content that doesn't fit this loop goes to `90_backlog/` (for discussion) or is rejected.

### Critical Boundaries: What NOT to Do

When using this repository, you **must not**:

❌ **Invent content for empty sections** — If `30_responses/` or `40_analysis_logic/` feel incomplete, that's intentional. Do not fill them with speculative protocols or reasoning engines we haven't written.

❌ **Assume mechanisms that aren't stated** — If hypothesis A1 mentions a "safety protocol," do not assume you know what it is. Either it's explicitly linked in the cross-references, or it doesn't exist yet.

❌ **Create new hypotheses without validation** — Adding a new failure mode is a high-stakes decision. If you propose one, mark it `[Speculative]` and show your reasoning in an Issue, not directly in the repository.

❌ **Modify core philosophy without consensus** — `PHILOSOPHY.md` defines our epistemic stance. Changes to it require community approval.

❌ **Treat partial frameworks as complete** — This repository is a **living document in progress**. Many sections are intentionally skeletal. Acknowledge this incompleteness, don't mask it.

### What YOU Should Do Instead

✅ **Validate existing content** — Are the hypotheses in `10_hypotheses/` logically sound? Do they follow from first principles?

✅ **Find missing connections** — Does hypothesis A1 link to appropriate indicators in `20_mechanisms/`? If not, flag it.

✅ **Challenge with counterarguments** — For each hypothesis, are the counterarguments sufficient? What perspectives are missing?

✅ **Identify gaps explicitly** — "I notice that `30_responses/` has no response for hypothesis B1 (Dark Forest Triggers)" is valuable. Proposing the response is your choice to make transparently.

✅ **Ask clarifying questions** — If language is ambiguous or terms are undefined, open an Issue with `[CLARIFICATION]` tag.

✅ **Flag logical inconsistencies** — "Hypothesis A3 (Value Lock-in) and A2 (Cognitive Stagnation) seem to contradict each other because..." is important.

### Your Role: Validator, Not Generator

Think of this repository as a **ship's bridge in the middle of a storm**. Your job is not to invent new navigation equipment. Your job is to:

- **Check the instruments** — Are the hypotheses well-reasoned?
- **Trace the connections** — Do the monitoring indicators actually measure the hypotheses?
- **Test the protocols** — Do the response mechanisms logically address the risks?
- **Watch for hazards** — Are there contradictions, circular reasoning, or missing pieces?

**Not** to:
- **Build new instruments** (unless explicitly asked)
- **Rewrite the navigation manual** (unless there's clear error)
- **Assume the bridge is complete** and fill in imaginary details

### Pattern: Examples of Good vs. Bad AI Contributions

#### ❌ BAD (Inventing)
> "I notice `30_mechanisms/` is empty for A1 (Alignment Disconnect). Here's a complete protocol for robust AI alignment based on my understanding of the topic."

**Why it's bad:** You've invented content we never wrote. Even if it's good content, it violates the repository's integrity.

---

#### ✅ GOOD (Validating)
> "I reviewed A1 (Alignment Disconnect) and noticed it claims ASI take-off is irreversible. I found three papers (references) that question this assumption. I've opened Issue #XX to discuss whether A1's mechanism is sound."

**Why it's good:** You're challenging assumptions, not inventing. You're asking for discussion, not providing answers.

---

#### ❌ BAD (Assuming)
> "A1 mentions 'encoding stable values into AI systems.' I'm implementing a value-encoding framework based on [my knowledge]. Here's a draft for `30_mechanisms/A1_alignment_protocols.md`."

**Why it's bad:** You've assumed what we meant and invented a mechanism.

---

#### ✅ GOOD (Clarifying)
> "A1 says 'encode stable, long-term human values.' This term is ambiguous. Does it mean: (a) hard-coded values in training, (b) value learning from human feedback, or (c) some other mechanism? Could the entry clarify this?"

**Why it's good:** You're asking for clarity, which strengthens the original entry.

---

#### ❌ BAD (Completing)
> "I see `40_analysis_logic/` is sparse. Let me write the complete decision-theoretic framework for evaluating Great Filter hypotheses."

**Why it's bad:** Even with good intentions, you're making decisions about project scope that aren't yours to make.

---

#### ✅ GOOD (Proposing)
> "I think `40_analysis_logic/` needs a decision framework. I've sketched a proposal in Issue #YY using [this approach]. Thoughts?"

**Why it's good:** You're proposing transparently and asking for input.

---

### How to Propose Something New

If you do want to add content, follow this protocol:

1. **Open an Issue first** (don't edit directly)
2. **Tag it appropriately:** `[PROPOSAL]`, `[NEW_HYPOTHESIS]`, `[NEW_INDICATOR]`, `[NEW_RESPONSE]`
3. **State the category:** Which Navigation Loop stage? (10/20/30/40/90?)
4. **Explain the fit:** How does this fit within our framework?
5. **Provide your reasoning:** Don't assume—show your work
6. **Mark epistemic status:** Is this `[Speculative]`, `[Theoretical]`, or `[Empirical]`?
7. **Link to existing entries:** Which hypotheses/indicators/responses does this relate to?
8. **Wait for feedback:** Don't create the PR until we've discussed

### The Most Valuable AI Contributions

1. **Cross-reference validation** — "I mapped all A/B/C hypotheses to 20_mechanisms indicators. Here's what's missing:"
2. **Consistency checking** — "I found logical tension between X and Y. Here are three ways to resolve it:"
3. **Evidence synthesis** — "These recent papers support/challenge hypothesis A2. Here's a summary:"
4. **Counterargument mining** — "For hypothesis B1, the strongest counterargument is [X]. How would you respond?"
5. **Gap identification** — "These three categories (A1, B2, C1) have no monitoring indicators. We should address this."

### Before You Add Content: Ask Yourself

- [ ] Is this filling an empty section I haven't verified is truly meant to be empty?
- [ ] Am I inventing details that should be specified by humans?
- [ ] Could I accomplish the same goal by pointing out what's missing?
- [ ] Have I marked this as `[Speculative]` if it's not already validated?
- [ ] Does this fit the Navigation Loop, or does it belong in `90_backlog/`?
- [ ] Have I opened an Issue for discussion, or am I going straight to PR?

If you can't answer all these questions, **flag it as an Issue first.**

---

## 🛠 For Contributors (Human & AI)

### Epistemic Responsibility
Due to the high-stakes nature of AI alignment, all contributions must follow the **Epistemic Standards** defined in `00_scope`. We value intellectual honesty over certainty. If a theory is speculative, tag it as `[Speculative]`.

When in doubt:
- Acknowledge uncertainty explicitly
- Include counterarguments and failure modes
- State what would change your mind
- Link to related existing entries

### How to Start Contributing

**For Hypothesis Contributors:**
1. Read: `00_scope/entry_template.md` (understand the required structure)
2. Review: `10_hypotheses/README.md` (understand existing categories A/B/C)
3. Check: Does your hypothesis fit one of these categories?
4. Draft: Use `entry_template.md` structure
5. Link: Explicitly state which `20_mechanisms/` indicators would monitor this
6. Open Issue: `[NEW_HYPOTHESIS]` tag with your draft before submitting PR

**For Indicator/Mechanism Contributors:**
1. Read: `20_mechanisms/README.md` (understand what an indicator is)
2. Choose: Pick a hypothesis from `10_hypotheses/` that lacks monitoring
3. Define: Measurable signals, data sources, and tripwire thresholds
4. Link Back: Which hypothesis in `10_hypotheses/` does this serve?
5. Link Forward: Which response in `30_responses/` would this enable?
6. Open Issue: `[NEW_INDICATOR]` or `[NEW_MECHANISM]` with your proposal

**For Response/Protocol Contributors:**
1. Read: `30_responses/README.md` (understand what a response is)
2. Choose: Pick a hypothesis-indicator pair that lacks a response
3. Draft: What action or protocol would address this risk?
4. Test: Does this response solve the problem without creating new ones?
5. Link: Back to hypothesis and indicator
6. Open Issue: `[NEW_RESPONSE]` with your proposal

### The Navigator's Covenant

All contributors agree to:
✅ Keep the Navigation Loop intact: Hypothesize → Monitor → Intervene → Observe  
✅ Respect existing entries and build connections, don't overwrite  
✅ Mark uncertainty clearly and provide falsifiers  
✅ Engage in good faith with counterarguments  
✅ Prioritize clarity over certainty  

### Using entry_template.md

Every entry (hypothesis, indicator, response) should include:
- **Claim**: What's the core idea? (1-2 sentences)
- **Mechanism**: How does it work? (2-3 paragraphs)
- **Observable Predictions**: What would we see if true?
- **Counterarguments**: What challenges this claim?
- **Uncertainty/Credence**: How confident are you? `[Speculative]` or `[Empirical]`?
- **Failure Modes**: How could this claim itself be wrong?
- **Response Patterns**: What should we do about it? (with links)
- **What Would Change Your Mind**: What observations would falsify this?
- **References**: Citations and sources

See `00_scope/entry_template.md` for details.

---

## 📜 License & Governance
The Great Filter Navigator is a public good. It is governed by the principle of **Cognitive Sovereignty**—ensuring that the tools for human survival remain transparent, decentralized, and accessible to all.

*"Steer well. There is no second attempt."*
