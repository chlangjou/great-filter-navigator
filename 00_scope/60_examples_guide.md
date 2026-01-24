---
title: "Examples Guide"
type: "guide"
layer: "00_scope"
sequence: 60
purpose: "Explain how to use the example entries and learn from them"
audience: "New contributors and learners"
epistemic_status: Consensus
confidence: 95
tags: [guide, examples, learning, best-practices]
dependencies: ["30_entry_template.md", "55_entry_validation_checklist.md"]
related_documents:
  - examples_in: "_examples/"
  - based_on: "30_entry_template.md"
  - complements: "55_entry_validation_checklist.md"
last_updated: "2026-01-24"
version: "1.0"
---

# Examples Guide

This document explains how to use the example entries in the `_examples/` directory and learn from them.

---

## What Are These Examples?

The `_examples/` directory contains **real-looking but pedagogical entries** designed to illustrate:
- ✅ What high-quality entries look like
- ❌ Common errors and how to avoid them
- 🔧 How to adapt templates for different risk types
- 📚 Best practices in reasoning and argumentation

**Important**: These are NOT actual GFN entries. They are teaching tools.

---

## The Four Example Files

### 1. `hypothesis_A1_good.md` - Exemplary Hypothesis Entry

**What it demonstrates**:
- ✅ Clear, testable claim
- ✅ Detailed causal mechanism with explicit steps
- ✅ Multiple observable predictions with current empirical status
- ✅ Real (not strawmanned) counterarguments
- ✅ Specific, testable falsification conditions
- ✅ Appropriate confidence calibration
- ✅ Diverse references (6+)

**How to use it**:
1. Read it as a complete example of what you should aim for
2. Compare its structure to the template in `30_entry_template.md`
3. Note how it addresses each template section
4. Use its tone and reasoning style as a model

**Length**: ~250 lines  
**Category**: A1 (Value Alignment)  
**Epistemic Status**: [Theoretical]  
**Time to read**: 15-20 minutes

---

### 2. `hypothesis_A1_bad.md` - Anti-Example with Errors Highlighted

**What it demonstrates**:
- ❌ Vague, untestable claims ("might happen")
- ❌ Insufficient mechanism explanation
- ❌ Unfalsifiable predictions ("unexpected ways")
- ❌ Strawmanned counterarguments
- ❌ **Missing "What Would Change My Mind" section** (disqualifying!)
- ❌ Too few references (2 vs. 5+ required)
- ❌ Unjustified confidence

**How to use it**:
1. Read it alongside the "good" example
2. Note which sections are problematic
3. For each error, understand WHY it's problematic
4. Compare to the good example to see corrections
5. Use as a checklist: "Am I making any of these mistakes?"

**Special Feature**: Each problematic section is annotated with:
- **What the error is**
- **Why it matters**
- **How to fix it**

**Length**: ~260 lines  
**Time to read**: 15 minutes (or 5 min for rapid review)

---

### 3. `response_technical_good.md` - Technical Solution Example

**What it demonstrates**:
- ✅ Structure for "response" entries (addressing risks)
- ✅ How to discuss mechanisms and trade-offs
- ✅ How to address limitations honestly
- ✅ Synergies with other response types
- ✅ Implementation pathways with milestones
- ✅ How to link to addressed risks (A1, A3, etc.)

**How to use it**:
1. Use as template if writing a technical response
2. Note how it differs from hypothesis entries (more solutions-focused)
3. See how it handles limitations and uncertainties
4. Use its implementation roadmap as model

**Length**: ~200 lines  
**Category**: Technical Response (Interpretability)  
**Addresses Risks**: A1, A3  
**Time to read**: 12-15 minutes

---

### 4. `response_institutional_good.md` - Institutional Solution Example

**What it demonstrates**:
- ✅ Structure for institutional/policy responses
- ✅ How to discuss complex social systems
- ✅ Game theory and coordination problems
- ✅ Historical precedents and lessons learned
- ✅ Multi-risk addressing (addresses 5 different risks)
- ✅ Implementation via coalition-building

**How to use it**:
1. Use as template for policy/governance entries
2. See how to incorporate game theory and history
3. Note table for trade-offs analysis
4. Model for addressing multiple risks simultaneously

**Length**: ~240 lines  
**Category**: Institutional Response (Governance)  
**Addresses Risks**: A1, B1, B2, C1, C2  
**Time to read**: 15-18 minutes

---

## How to Use Examples: Three Learning Paths

### Path 1: Quick Learning (20 minutes)

1. Read: `hypothesis_A1_bad.md` - See common errors (5 min)
2. Read: `hypothesis_A1_good.md` - See correct approach (10 min)
3. Compare: Note specific differences (5 min)

**Result**: Understand what makes entries good vs. bad

---

### Path 2: Detailed Learning (45 minutes)

1. Read: `hypothesis_A1_good.md` (15 min)
2. Read: `30_entry_template.md` (15 min)
3. Map: Identify how good example fills each template section (10 min)
4. Read: `hypothesis_A1_bad.md` for anti-examples (10 min)

**Result**: Deep understanding of entry structure and quality

---

### Path 3: Specialized Learning (60+ minutes)

**For writing hypothesis entries**:
1. Read: `hypothesis_A1_good.md` + `hypothesis_A1_bad.md` (25 min)
2. Study: `30_entry_template.md` in detail (20 min)
3. Review: `55_entry_validation_checklist.md` (15 min)
4. Analyze: Why good example passes all checks, bad example fails (15+ min)

**For writing technical response entries**:
1. Read: `response_technical_good.md` (15 min)
2. Study: How it addresses limitations and trade-offs (15 min)
3. Note: Implementation pathway structure (10 min)
4. Draft: Your own technical response (20+ min)

**For writing institutional response entries**:
1. Read: `response_institutional_good.md` (15 min)
2. Note: How it uses history and game theory (15 min)
3. Study: Risk addressing framework (10 min)
4. Draft: Your own institutional response (20+ min)

---

## Adaptation Guide: Using Examples as Templates

### Adapting the Hypothesis Structure

**Step 1**: Use `hypothesis_A1_good.md` as structural template
**Step 2**: Replace content with your own
**Step 3**: Keep section headers and overall flow
**Step 4**: Maintain quality standards shown in example

Example sections to preserve:
- Metadata (title, category, status, confidence, tags)
- Claim (1-2 paragraphs, testable)
- Mechanism (4-7 paragraphs, with causal steps labeled)
- Predictions (2-3 observations, each with current status)
- Counterarguments (3-4, with substantive responses)
- Failure Modes (3-5 scenarios)
- **What Would Change My Mind** (3-5 specific conditions) ✅ **MANDATORY**
- References (7-10 citations)

### Adapting the Response Structure

**For Technical Responses**, use `response_technical_good.md`:
- How This Strategy Works (mechanism)
- Synergies with Other Responses (complementarities)
- Limitations and Risks (honest assessment)
- What Would Change My Mind (falsifiers)
- Implementation Pathway (phases and timeline)
- References (5-7 citations)

**For Institutional Responses**, use `response_institutional_good.md`:
- How This Strategy Works (mechanism)
- Synergies with Other Responses
- Limitations and Risks (including game-theoretic analysis)
- What Would Change My Mind
- Relationship to Risk Hypotheses (which risks does it address?)
- Implementation Pathway (coalition-building, negotiation, enforcement)
- Historical Precedents (learn from similar cases)
- References (7-10 citations)

---

## Common Questions About Examples

### Q1: Can I copy the examples directly?

**Short answer**: No.

These are pedagogical. If you copy them:
- Your entry won't be original
- Reviewers will recognize duplicated content
- You'll waste effort (should be custom-written)

**What you should do**:
- Use them as structure and style guides
- Write your own content
- Model your reasoning after examples
- Cite and reference appropriately

### Q2: What if my topic is in A2 or B1, not A1?

**Answer**: Use the structure from `hypothesis_A1_good.md` but:
- Change the **Claim** to address A2 or B1 risks
- Keep all section headers
- Adapt **Mechanism** to the specific risk
- Update **Predictions** to fit your mechanism
- Adjust **References** to your topic

The template structure works for any category A1-C2.

### Q3: Can I just do hypothesis entries, or should I also write responses?

**Answer**: Both are valuable, but different:
- **Hypothesis entries** map risks/problems
- **Response entries** propose solutions

Start with what you understand best. If you understand a risk well, write a hypothesis. If you understand a potential solution, write a response.

### Q4: How detailed should my mechanism be?

**Answer**: Compare to examples:
- `hypothesis_A1_good.md`: Mechanism has 5 numbered steps + explanation = ~600 words
- Your mechanism should similarly explicit

Minimum: 300 words (multiple paragraphs, clear steps)  
Target: 400-600 words  
Maximum: Avoid > 1000 words unless truly complex

### Q5: How many counterarguments do I need?

**Answer**: Minimum 2-3, target 3-4 (like examples).

For each:
- State the objection clearly
- Respond substantively (not dismissively)
- Show why it doesn't invalidate your claim

### Q6: What if I disagree with one of the examples?

**Answer**: That's great! Write a response entry:
- Title: "Critique: [Example Title]"
- Explain what you think is wrong
- Provide alternative hypothesis
- Reference the original example

This is intellectual engagement, not attack.

---

## Quality Checklist: Is Your Entry Ready?

Use this checklist against your own entry:

**Structural Comparison** (vs. examples):
- [ ] Do I have all major sections like the good example?
- [ ] Is my mechanism as detailed as the example's?
- [ ] Do my predictions have observable metrics like the example's?
- [ ] Are my counterarguments substantive like the example's?

**Content Quality**:
- [ ] Is my claim as clear and testable as in good example?
- [ ] Are my causal steps explicit?
- [ ] Are my predictions specific (not vague like bad example)?
- [ ] Do I address counterarguments without strawmanning?

**Critical Elements** (required):
- [ ] Do I have "What Would Change My Mind" section? ✅
- [ ] Are my falsification conditions specific? ✅
- [ ] Do I have 5+ references? ✅
- [ ] Is my confidence calibrated to epistemic status? ✅

**Advanced** (optional but recommended):
- [ ] Do I discuss limitations honestly?
- [ ] Do I link to related entries or risks?
- [ ] Do I explain any key assumptions?
- [ ] Is my tone appropriately cautious?

---

## Next Steps After Learning From Examples

1. **Pick a risk or response** you care about
2. **Draft an entry** using examples as structure
3. **Self-review** using `55_entry_validation_checklist.md`
4. **Peer review** (share with 1-2 others)
5. **Submit** for community feedback
6. **Iterate** based on feedback

---

## Additional Resources

| Resource | Purpose | When to Use |
|----------|---------|------------|
| `30_entry_template.md` | Detailed template instructions | Writing your entry |
| `55_entry_validation_checklist.md` | Validation criteria | Before submission |
| `45_machine_readable_conventions.md` | Technical specs | If writing for automation |
| `25_taxonomy_index.md` | Category/tag reference | Choosing categories |
| `README.md` | Overview and navigation | New to 00_scope |

---

## Contributing Better Examples

If you write an entry that's exceptionally clear or provides good contrast with existing examples:
- Consider submitting it as an example
- It will help future contributors
- Examples are tagged and maintained separately

Criteria for example-worthy entries:
- ✅ Well-reasoned and substantive
- ✅ Illustrates important principles
- ✅ Good contrast with existing examples
- ✅ Accessible to learners
- ✅ Properly citations and sourced

---

**Last Updated**: 2026-01-24  
**Status**: Active guide for examples in `_examples/` directory  
**Feedback**: Suggest improvements via issue tracker or pull request