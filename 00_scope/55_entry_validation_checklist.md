---
title: "Entry Validation Checklist"
type: "guide"
layer: "00_scope"
sequence: 55
purpose: "Provide automated and manual validation checklist for GFN entries"
audience: "Contributors, reviewers, and automated validation systems"
epistemic_status: Consensus
confidence: 90
tags: [guide, validation, checklist, quality-assurance]
dependencies: ["30_entry_template.md", "40_what_would_change_our_minds.md"]
related_documents:
  - based_on: "30_entry_template.md"
  - used_for: "Entries in 10_hypotheses/ and 20_mechanisms/"
  - see_also: "45_machine_readable_conventions.md"
last_updated: "2026-01-24"
version: "1.0"
---

# Entry Validation Checklist

This document provides a structured checklist for validating new entries before submission. Use this for:
- **Manual review** by human contributors
- **Automated validation** by tools
- **Peer review** by other contributors

---

## Pre-Submission Checklist (For Contributors)

Use this checklist before submitting your entry. All items should be checked (✅) before submission.

### Section 1: Structure and Format

- [ ] **S1.1** Entry has clear title (5-150 characters)
- [ ] **S1.2** Entry includes Metadata section with at least: Title, Category, Epistemic Status, Confidence
- [ ] **S1.3** Claim/Hypothesis section is present and clearly labeled
- [ ] **S1.4** Mechanism section explains causal chain with 3+ steps
- [ ] **S1.5** Observable Predictions section lists 2+ predictions
- [ ] **S1.6** Counterarguments section presents real objections
- [ ] **S1.7** Failure Modes section documented (recommended)
- [ ] **S1.8** Response Patterns section present or linked (recommended)
- [ ] **S1.9** "What Would Change My Mind" section is present and substantive ✅ **MANDATORY**
- [ ] **S1.10** References section lists 5+ citations

**Status**: All mandatory items (S1.1, S1.2, S1.3, S1.4, S1.5, S1.6, S1.9, S1.10) ✅ checked?

---

### Section 2: Content Quality

- [ ] **C2.1** Title clearly describes the core claim
- [ ] **C2.2** Claim is testable and not tautological
- [ ] **C2.3** Mechanism includes clear causal steps (not just "X leads to Y")
- [ ] **C2.4** Mechanism addresses "why" and "how", not just "what"
- [ ] **C2.5** Each prediction includes observable metric or evidence
- [ ] **C2.6** Predictions are falsifiable (not vague like "something bad will happen")
- [ ] **C2.7** Counterarguments are serious (not strawmanned)
- [ ] **C2.8** Counterarguments are NOT successfully dismissed without response
- [ ] **C2.9** Uncertainty/Confidence explained if rating < 70%
- [ ] **C2.10** Failure modes are realistic, not hypothetical edge cases

**Status**: Minimum 8/10 items checked? 

---

### Section 3: Falsifiability (Critical)

- [ ] **F3.1** "What Would Change My Mind" section is substantive (150+ words)
- [ ] **F3.2** Contains 3+ specific conditions for revision or rejection
- [ ] **F3.3** Conditions are testable (empirical, not philosophical)
- [ ] **F3.4** Conditions are concrete (e.g., "observed in X scenarios" NOT "maybe something surprising happens")
- [ ] **F3.5** Falsifiability section is NOT vague (avoid: "new evidence", "better theories", "more research")
- [ ] **F3.6** At least one falsifier is within 5-year horizon
- [ ] **F3.7** The entry survives attempted self-refutation (author tried to falsify their own claim)

**Status**: All 7 falsifiability items checked? ✅ **MANDATORY FOR SUBMISSION**

---

### Section 4: Classification and Tagging

- [ ] **T4.1** Category is correctly assigned (A1-A3, B1-B3, or C1-C2)
- [ ] **T4.2** Epistemic Status is one of: [Speculative], [Theoretical], [Empirical], [Consensus]
- [ ] **T4.3** Confidence level is consistent with Epistemic Status
- [ ] **T4.4** Tags are from approved list (see `25_taxonomy_index.md`)
- [ ] **T4.5** At least 1 functional tag applied (#alignment, #governance, etc.)
- [ ] **T4.6** Time horizon tags applied (#near-term or #long-term)
- [ ] **T4.7** Risk level tags applied (#existential-risk or #s-risk as appropriate)

**Status**: 6/7 tagging items checked?

---

### Section 5: References and Attribution

- [ ] **R5.1** Minimum 5 references cited
- [ ] **R5.2** References include author, date, title
- [ ] **R5.3** References are from reputable sources (peer-reviewed, established researchers, official documents)
- [ ] **R5.4** Citations are accurate (author/date verified)
- [ ] **R5.5** At least 2 references are primary sources (not summaries/reviews)
- [ ] **R5.6** References span multiple sources (not all from one author/group)
- [ ] **R5.7** Out-of-date references noted (e.g., "as of 2023, X was..." if from older work)

**Status**: 6/7 reference items checked?

---

### Section 6: Logic and Reasoning

- [ ] **L6.1** No circular reasoning (Claim doesn't depend on Mechanism which depends on Claim)
- [ ] **L6.2** Mechanism's failure modes don't undermine the entire claim
- [ ] **L6.3** Counterarguments are actually addressed (not dismissed without engagement)
- [ ] **L6.4** No vague language in critical claims ("could", "might", "perhaps" only where appropriate)
- [ ] **L6.5** No confirmed false claims presented as current fact
- [ ] **L6.6** Assumptions are explicitly stated where non-obvious
- [ ] **L6.7** Claims are proportional to evidence (confident claims have strong support)

**Status**: 6/7 logic items checked?

---

### Section 7: Completeness

- [ ] **Comp7.1** Entry has been read aloud or reviewed by another person
- [ ] **Comp7.2** No placeholder text or TODOs remain
- [ ] **Comp7.3** All cross-references to other entries are functional
- [ ] **Comp7.4** Markdown formatting is valid (no broken links, valid tables)
- [ ] **Comp7.5** Estimated reading time is < 20 minutes (unless extensive)

**Status**: All 5 completeness items checked?

---

## Automated Validation Script

For automated systems, use this validation order:

### Validation Level 1: Format (CRITICAL)

```
ERROR if any of:
- [ ] Title is missing or < 5 characters
- [ ] No YAML frontmatter
- [ ] "What Would Change My Mind" section missing
- [ ] References < 5
- [ ] No Category specified
- [ ] Invalid Epistemic Status
```

**Action if Level 1 FAIL**: Reject entry, return error list

### Validation Level 2: Content (IMPORTANT)

```
WARNING if any of:
- [ ] Claim > 1000 words
- [ ] Mechanism < 200 words
- [ ] Predictions < 2 or > 10
- [ ] Counterarguments < 100 words
- [ ] Falsifiability section < 150 words
- [ ] Confidence not calibrated to Epistemic Status
- [ ] Tags not in approved list
```

**Action if Level 2 WARNING**: Flag issues, allow submission with review note

### Validation Level 3: Logic (ADVISORY)

```
SUGGESTION if:
- [ ] Circular logic detected (keyword analysis)
- [ ] Vague language in critical sections
- [ ] Confidence > 80% with [Speculative] status (mismatch)
- [ ] No response pattern linked
- [ ] Counterarguments not addressed
- [ ] Mechanism's failure modes dominant
```

**Action if Level 3 SUGGESTION**: Provide feedback, allow submission with suggestions

---

## Peer Review Checklist

For human reviewers of submissions:

### Quick Review (5 minutes)

1. [ ] Does the title accurately describe the claim?
2. [ ] Is the claim clearly testable or falsifiable?
3. [ ] Are there at least 5 references?
4. [ ] Does "What Would Change My Mind" section exist and make sense?
5. [ ] Is the category assignment reasonable?

**If all 5 ✅**: Likely acceptable. Consider full review.  
**If any ❌**: Request revisions before full review.

### Standard Review (20 minutes)

1. [ ] Structure: All required sections present?
2. [ ] Claim: Clear, testable, proportional to evidence?
3. [ ] Mechanism: Explains causal chain coherently?
4. [ ] Predictions: Observable and falsifiable?
5. [ ] Counterarguments: Real and addressed?
6. [ ] Falsifiability: Specific, testable conditions?
7. [ ] References: Credible, diverse, 5+ minimum?
8. [ ] Logic: No circular reasoning or fatal flaws?
9. [ ] Confidence: Calibrated to evidence?
10. [ ] Tags: Accurate and helpful?

**Scoring**: 8+ ✅ = Accept, 6-7 ✅ = Request revisions, <6 ✅ = Significant work needed

### Deep Review (45+ minutes)

Additional checks for complex or controversial entries:

- [ ] Verify all references are cited accurately
- [ ] Check if cited studies actually support the claim
- [ ] Research if significant counterevidence exists
- [ ] Assess if alternative explanations are adequately addressed
- [ ] Evaluate if entry could be stronger with different framing
- [ ] Consider if category is optimal or if alternative would be better
- [ ] Assess if confidence level is calibrated to expert consensus
- [ ] Identify potential weaknesses author didn't consider

---

## Common Validation Failures and Fixes

### Failure 1: Missing "What Would Change My Mind" Section

**Error Message**: "What Would Change My Mind section is mandatory"  
**Why It Matters**: Unfalsifiable claims can harden into dogma  
**Fix**: Add section with 3+ specific, testable conditions

**❌ Bad example**:
> "If new evidence emerges showing this is wrong, we would reconsider."

**✅ Good example**:
> "This entry would be weakened if: (1) Empirical studies show resource hoarding does NOT increase with AI capability, (2) We find historical precedents where coordination succeeded despite misaligned incentives, (3) Formal proofs show the mechanism cannot work as described."

---

### Failure 2: Vague Predictions

**Error Message**: "Predictions must be observable and testable"  
**Why It Matters**: Vague predictions can't be falsified  
**Fix**: Specify observable metric or evidence

**❌ Bad example**:
> "We will probably see more AI incidents in the future"

**✅ Good example**:
> "Within 5 years, major AI incidents caused by misalignment will double YoY, measured by incidents reported in [Database Name]"

---

### Failure 3: Counterarguments Not Addressed

**Error Message**: "Counterarguments appear to be dismissed without engagement"  
**Why It Matters**: Intellectual honesty requires addressing serious objections  
**Fix**: For each counterargument, show why it doesn't invalidate the claim

**❌ Bad example**:
> **Counterargument**: "Humans have solved this before."  
> **Response**: "But AI is different."

**✅ Good example**:
> **Counterargument**: "Humans solved principal-agent problems with contracts."  
> **Response**: "However, AI systems cannot be bound by contracts in the same way. Unlike humans, AIs lack the social/legal framework enforcement mechanisms. Moreover, the speed of AI decisions makes legal remedy after-the-fact ineffective."

---

### Failure 4: Confidence Mismatch

**Error Message**: "Confidence (85%) inconsistent with Epistemic Status ([Speculative])"  
**Why It Matters**: Calibration prevents overconfidence  
**Fix**: Align confidence to epistemic status or change status

**Guidance**:
- `[Speculative]`: 0-30% confidence
- `[Theoretical]`: 30-60% confidence
- `[Empirical]`: 60-85% confidence
- `[Consensus]`: 85-95%+ confidence

---

### Failure 5: Insufficient References

**Error Message**: "Minimum 5 references required; found 2"  
**Why It Matters**: Claims need evidentiary support  
**Fix**: Add 3+ additional credible sources

---

## Remediation Process

When validation fails:

1. **Automated Rejection**: Entry blocked from submission
2. **Feedback Provided**: Specific error messages given
3. **Revision Period**: Contributor has 30 days to revise
4. **Resubmission**: Submit revised entry for new validation
5. **Pass Threshold**: If revised entry passes all checks, accepted
6. **Appeal Process**: For disputed failures, submit to review committee

---

## Validation Metrics (For Maintainers)

Track validation performance:

- % entries passing first submission
- Most common failure reasons
- Average revision cycles before acceptance
- Time to validation completion
- False positive/negative rates

---

Last Updated: 2026-01-24