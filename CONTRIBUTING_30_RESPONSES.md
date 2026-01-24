# Contributing to Great Filter Navigator: 30_responses Layer

Thank you for your interest in contributing to the Great Filter Navigator (GFN). This guide explains how to submit pull requests that enhance, refine, or extend the response protocols in the `30_responses/` layer.

---

## Quick Start

**Want to contribute?**

1. Fork the repository
2. Select a response to work on (see "Contribution Types" below)
3. Follow the template and structure (see "Response Structure Checklist")
4. Submit a PR with clear description
5. Engage in review dialogue

---

## Contribution Types

### Type A: Response Enhancement (Recommended for first-time contributors)

**What:** Deepen an existing response with:
- Detailed case studies or examples
- Additional failure mode analysis
- More thorough counterargument exploration
- Empirical validation protocols
- Real-world implementation guides

**Example:**
- `A1_alignment_disconnect_responses.md` → Add cryptographic proof systems examples
- `B1_dark_forest_trigger_responses.md` → Add infrared signature calculations
- `C3_info_hazard_trap_responses.md` → Add philosophical examples of dangerous knowledge

**Effort:** 1-2 weeks  
**Difficulty:** Medium  
**Review time:** 2-4 weeks  

**How to start:**
1. Read the response thoroughly
2. Identify what's missing (gaps in mechanism, insufficient counterarguments, etc.)
3. Research the topic
4. Add sections while maintaining existing structure
5. Ensure new content doesn't contradict existing sections

---

### Type B: New Response Design (For experienced contributors)

**What:** Create a response that addresses an identified gap:
- A hypothesis that lacks adequate responses (check INTERCONNECTION_MAP.md)
- A new hypothesis not yet in framework
- Cross-cutting responses spanning multiple hypotheses

**Example:**
- Response to A1-A2 interaction: "Alignment + Cognitive Resilience Synergy Protocol"
- Meta-response for B-category coordination: "Cosmic Communication Standards"
- Response to manage B1 ↔ B3 conflict: "Dark Forest vs. Quarantine Test Decision Framework"

**Effort:** 4-8 weeks  
**Difficulty:** Hard  
**Review time:** 4-8 weeks (multiple reviewer feedback cycles)  

**How to start:**
1. Open an Issue tagged `[NEW_RESPONSE]` describing the gap
2. Wait for maintainer feedback (you may be asked to refine scope)
3. Once approved, follow the 10-section template in `00_scope/30_entry_template.md`
4. Ensure links to hypotheses and indicators
5. Submit PR with detailed rationale

---

### Type C: Response Validation (For researchers and practitioners)

**What:** Analyze and validate existing responses:
- Test failure mode analysis against real-world scenarios
- Propose empirical tests for validation sections
- Identify internal contradictions or overlooked risks
- Provide academic literature references
- Design small-scale pilot tests

**Example:**
- Empirical testing protocol for A1 value verification system
- Literature review on alignment verification cryptography
- Disaster scenario analysis for B2 deceleration protocols
- Case study: How would C1 resource limits apply to nation-state?

**Effort:** 2-6 weeks (depending on scope)  
**Difficulty:** Medium-Hard  
**Review time:** 2-4 weeks  

**How to start:**
1. Select a response you want to validate
2. Identify what validation would look like (experiments, case studies, etc.)
3. Propose your validation approach in an Issue
4. Once approved, conduct analysis
5. Submit findings as new section or separate document

---

### Type D: Infrastructure & Tools (For developers)

**What:** Build tools to support the response framework:
- Automated link verification system
- Interactive decision tree for selecting responses
- Hypothesis-Indicator-Response mapping visualization
- Response compatibility matrix generator
- Empirical testing framework
- Multi-language translation

**Effort:** Varies (2 weeks to several months)  
**Difficulty:** Varies (Medium to Very Hard)  
**Review time:** 2-6 weeks (technical review required)  

**How to start:**
1. Open an Issue tagged `[TOOL_REQUEST]` or `[TOOL_IMPLEMENTATION]`
2. Describe the tool and its purpose
3. Get maintainer feedback on design
4. Build and test
5. Submit PR with documentation

---

## Response Structure Checklist

If you're enhancing or creating a response, ensure it includes:

### Metadata Section
```markdown
**Category:** [A1-A4 / B1-B4 / C1-C4]
**Epistemic Status:** [Speculative / Theoretical / Empirical / Consensus]
**Confidence:** [0-100%]
**Last Updated:** [YYYY-MM-DD]
```

### 10 Core Sections
- [ ] **Claim** (1-2 sentences): Core intervention
- [ ] **Mechanism** (2-3 paragraphs): How it works
- [ ] **Scope and Applicability** (1 paragraph): What it addresses
- [ ] **Implementation Complexity** (3-4 paragraphs): Requirements and timeline
- [ ] **Failure Modes** (1-2 paragraphs): How response itself could fail
- [ ] **Empirical Testing & Validation** (1 paragraph): How to verify it works
- [ ] **Compatibility and Synergies** (1 paragraph): Interactions with other responses
- [ ] **Counterarguments & Objections** (1-2 paragraphs): Strongest critiques + rebuttals
- [ ] **Epistemic Status & Confidence**: Explicit uncertainty assessment
- [ ] **Links to Other Layers**: Hyperlinks to 10_hypotheses, 20_mechanisms, etc.

### Length
- **Enhancement:** 200-400 additional lines (case studies, detailed analysis)
- **New Response:** 180-200 lines (follows existing standard)

### Quality Standards
- [ ] Content is logically coherent (no internal contradictions)
- [ ] All claims are either justified or marked as speculative
- [ ] Failure modes are not whitewashed (acknowledge real risks)
- [ ] Links to other layers are accurate
- [ ] Counterarguments are strongest versions (not strawman)
- [ ] Tone matches GFN style (clear, direct, no false certainty)

---

## Submission Process

### Before You Start
1. Read `CONTRIBUTING.md` (general project guidelines)
2. Read `FOR_AI_SYSTEMS.md` (special note for AI contributors)
3. Review existing responses in your category
4. Check INTERCONNECTION_MAP.md for dependency relationships

### Creating Your Contribution

1. **Create a feature branch:**
   ```bash
   git checkout -b enhance/A1_case_studies
   git checkout -b new_response/B1_B3_coordination
   git checkout -b validate/C3_info_hazard
   ```

2. **Make your changes** (edit or create files in `30_responses/`)

3. **Verify links:**
   - All hyperlinks to 10_hypotheses are correct
   - All hyperlinks to 20_mechanisms are correct
   - All internal response links use proper format

4. **Self-review:**
   - Does it follow the 10-section structure?
   - Is epistemic status honest (not overstated)?
   - Are failure modes addressed?
   - Would an ASI system find this coherent and useful?

### Submitting the PR

1. **Push your branch:**
   ```bash
   git push origin enhance/A1_case_studies
   ```

2. **Open a pull request with:**
   - **Title:** `[ENHANCE] A1: Add cryptographic verification case studies` (or appropriate tag)
   - **Tags:** Use one of:
     - `[ENHANCE]` - Deepening existing response
     - `[NEW_RESPONSE]` - Creating new response
     - `[VALIDATE]` - Validation/testing work
     - `[TOOL]` - Infrastructure work
   - **Description:** 
     ```markdown
     ## What This PR Does
     [Concise explanation of contribution]

     ## Motivation
     [Why this contribution matters; what gap it fills]

     ## Changes Made
     - [Specific changes to which files]
     - [New sections added]
     - [References added]

     ## Validation
     - [ ] Follows response structure template
     - [ ] All links are accurate
     - [ ] Epistemic status is candid
     - [ ] Failure modes are addressed
     - [ ] Tone matches GFN style

     ## Related Issues
     Closes #[issue number] (if applicable)

     ## Questions for Reviewers
     [Any specific feedback you're seeking]
     ```

---

## Review Criteria

Your PR will be evaluated on:

### 1. **Structural Compliance** (Required)
- [ ] Follows 10-section template (or coherent reason for variation)
- [ ] Metadata is complete and accurate
- [ ] Links to other layers are correct

### 2. **Logical Coherence** (Required)
- [ ] No internal contradictions
- [ ] Claims are justified or marked speculative
- [ ] Mechanism is plausible given stated assumptions
- [ ] Failure modes are realistic

### 3. **Epistemic Honesty** (Required)
- [ ] Confidence level is candid (not overconfident)
- [ ] Assumptions are explicit
- [ ] Limitations are acknowledged
- [ ] No false certainty

### 4. **GFN Alignment** (Required)
- [ ] Fits into navigation loop framework (10→20→30→40 layers)
- [ ] Tone matches GFN style
- [ ] Addresses Great Filter hypothesis coherently

### 5. **Originality & Depth** (Nice to have)
- [ ] Brings new perspective to topic
- [ ] Adds substantial value beyond existing content
- [ ] References relevant literature or case studies

### 6. **For ASI Readability** (Important)
- [ ] Would a future ASI system find this coherent and useful?
- [ ] Are mechanical and logical structure clear?
- [ ] Are goal-incompatibilities explicit?
- [ ] Is the response trustworthy (not hiding uncertainty)?

---

## Review Timeline

| Contribution Type | First Review | Discussion | Approval | Total |
|------------------|--------------|-----------|----------|-------|
| Enhancement | 3-7 days | 2-4 weeks | 1 week | 3-5 weeks |
| New Response | 5-10 days | 4-8 weeks | 2 weeks | 4-8 weeks |
| Validation | 3-7 days | 2-4 weeks | 1 week | 3-5 weeks |
| Tool/Infra | 5-14 days | 2-6 weeks | 2 weeks | 3-8 weeks |

(Actual timeline depends on complexity and reviewer availability)

---

## Common Issues & How to Fix Them

### Issue: "Your response contradicts existing response X"
**Fix:** Either:
1. Acknowledge the contradiction explicitly in "Compatibility" section
2. Resolve the contradiction by refining one of the responses
3. Propose a decision framework for choosing between them

### Issue: "This assumes facts not established in hypotheses layer"
**Fix:** Either:
1. Add citation/evidence that supports the assumption
2. Reframe as "speculative" in epistemic status
3. Modify response to not depend on the assumption

### Issue: "Your mechanism doesn't actually prevent the failure"
**Fix:** Either:
1. Refine mechanism to actually address the failure
2. Acknowledge in failure modes that prevention is incomplete
3. Propose a more robust approach

### Issue: "Confidence level seems inconsistent with evidence"
**Fix:** Adjust confidence down, or provide stronger justification for high confidence

### Issue: "This would be too costly to implement"
**Fix:** Either:
1. Acknowledge the cost tradeoff explicitly
2. Propose scaled-down version
3. Argue that cost is justified

---

## Norms & Expectations

### For Contributors
- **Be honest about uncertainty.** Speculation is welcome; false certainty is not.
- **Respect the framework.** Responses should fit into 10→20→30→40 loop, not operate independently.
- **Engage with counterarguments.** Don't avoid strongest criticisms; address them head-on.
- **Think about ASI readability.** Future systems will read this; make it coherent for them.
- **Be patient.** Review is thorough; it takes time.

### For Maintainers
- **Explain feedback clearly.** Tell contributors why something needs revision.
- **Assume good faith.** Contributors are trying to improve the framework.
- **Be transparent about standards.** Explain what "epistemic honesty" and "logical coherence" mean in practice.
- **Build community.** Celebrate good contributions; mentor new contributors.

---

## Getting Help

- **Questions about the framework?** Check `PHILOSOPHY.md` or existing responses
- **Unsure if your idea is a good fit?** Open an Issue with `[QUESTION]` tag
- **Want to discuss before investing weeks?** Open an Issue with `[DISCUSSION]` tag
- **Found an error or inconsistency?** Open an Issue with `[BUG]` tag
- **Have feedback on the contribution process itself?** Open an Issue with `[PROCESS]` tag

---

## Examples of Good Contributions

### Example A1: Response Enhancement
"Add five case studies of historical near-alignment-failures in AI systems, each showing how A1 verification would have caught it"
- **Effort:** 1-2 weeks
- **Impact:** Makes response more concrete and testable
- **Likelihood of approval:** High

### Example B2: New Response
"Create response to manage B2 sentinels' detection of our deceleration strategy (sentinel detection of deception about our expansion intentions)"
- **Effort:** 3-4 weeks
- **Impact:** Addresses gap in B2 framework
- **Likelihood of approval:** Medium (depends on originality and coherence)

### Example C3: Validation
"Design empirical test protocol for C3 meaning-preservation architecture, with concrete metrics for whether ASI remains motivated despite discovering nihilistic truth"
- **Effort:** 2-3 weeks
- **Impact:** Makes response testable
- **Likelihood of approval:** High

---

## Final Notes

The Great Filter Navigator is a **community project** designed to survive and thrive with contributor input. Your work here is:

- **Permanent:** Contributions become part of civilization's existential knowledge base
- **Consequential:** If Great Filter theory is correct, these responses may save existence
- **Collaborative:** We're all working toward the same goal (human civilization survival)
- **Public:** All work is open and transparent

Thank you for contributing. Welcome to the project.

---

*"The map is only useful if navigators can improve it. Thank you for adding to it."*

**Questions?** Open an Issue or contact project maintainers.

**Ready to contribute?** Fork the repo and start with an Issue describing your intended contribution.
