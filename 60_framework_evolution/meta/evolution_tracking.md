# Framework Evolution Tracking

**Central dashboard for all framework upgrade proposals and their status**

---

## 📊 Proposal Status Dashboard

| ID | Name | Status | Submitted | Review End | Decision | Adopter Decision |
|---|---|---|---|---|---|---|
| **2601** | Bionic Immunity & Intent Sandboxing (BIIS) | 🔵 Under Review | 2026-01-24 | 2026-02-07 | 2026-02-14 | Pending |
| **2602** | [Open for proposals] | ⚪ Not Proposed | - | - | - | - |
| **2603** | [Open for proposals] | ⚪ Not Proposed | - | - | - | - |

**Status Meanings:**
- 🔵 **Under Review** - Community feedback period active
- 🟡 **In Decision** - Core team making final decision
- 🟢 **Adopted** - Approved for implementation
- 🔴 **Rejected** - Not approved for implementation
- ⏸️ **Deferred** - Postponed for future consideration
- ⚪ **Not Proposed** - Slot available for new proposals

---

## 2601: BIIS (Bionic Immunity & Intent Sandboxing)

**Full Name:** Bionic Immunity & Intent Sandboxing Framework  
**Proposer:** Academic peer / red team  
**Submitted:** 2026-01-24  
**Scope:** Framework-wide v1.0 → v2.0 redesign  

### Timeline

| Phase | Start | End | Status |
|-------|-------|-----|--------|
| Community Review | 2026-01-24 | 2026-02-07 | 🔵 Active |
| Core Team Evaluation | 2026-02-07 | 2026-02-14 | ⚪ Pending |
| Decision Announcement | 2026-02-14 | 2026-02-14 | ⚪ Pending |
| Implementation (if approved) | 2026-02-21 | 2026-04-XX | ⚪ Pending |

### Review Discussion

**Discussion Location:** [GitHub Issues tagged #2601-biis]

**Community Sentiment (preliminary):** TBD after review period

**Key Questions Raised:** [Will be tracked in GitHub issues]

### Core Team Assessment

**Evaluation Date:** Pending (2026-02-14)

**Team Members Assessing:**
- [ ] Framework lead
- [ ] Technical lead
- [ ] Community representative
- [ ] AI safety expert

**Preliminary Assessment:** TBD

### Decision Rationale

[Will be filled in after decision is made on 2026-02-14]

---

## Decision Framework

### Adoption Criteria

**A proposal is ADOPTED if:**
- ✅ Solves 2+ major framework problems (demonstrated)
- ✅ Community consensus exists (70%+ support in review discussion)
- ✅ Clear implementation plan with phases and timelines
- ✅ Resources available for execution
- ✅ Backward compatibility with existing layers 10-50 preserved

**A proposal is DEFERRED if:**
- ⏸️ Needs more community input (insufficient feedback)
- ⏸️ Implementation plan needs clarification
- ⏸️ Resource constraints prevent current implementation
- ⏸️ Timing not optimal (better to revisit later)

**A proposal is REJECTED if:**
- ❌ Doesn't solve real framework problems
- ❌ Community opposes (30%+ significant concerns not addressed)
- ❌ Breaks backward compatibility without compelling justification
- ❌ Core team consensus against adoption

### 2601 BIIS Evaluation

**Does it solve real problems?**
- ✅ Addresses Goodhart's Law vulnerability (metric gaming)
- ✅ Addresses safe corridor paradox (over-specification)
- ✅ Addresses transparency vulnerability (attack surface)

**Is there community consensus?**
- Status: Under review (feedback being collected)
- Target: 70%+ support

**Is implementation plan clear?**
- ✅ 5 phases defined with token estimates
- ✅ Timeline: 8+ weeks to completion
- ✅ Integration points with existing layers specified

**Are resources available?**
- Status: To be determined based on adoption decision
- Estimated budget: 2,500-3,500 tokens
- Remaining available: ~25,000 tokens

**Is backward compatibility preserved?**
- ✅ Layers 10-50 logic preserved
- ✅ New layer 51_vitality_layer added
- ✅ Reframes 40_analysis_logic philosophy (justified by critique)
- ⚠️ Significant rewrite of 40_analysis_logic success criteria

---

## Historical Decisions

### GFN Framework Evolution History

**2026-01-24 - Initial Framework (v1.0)**
- Specification-based safety model
- Layers 10-50 fully developed
- Status: Deployed

**2026-01-24 - Red Team Critique**
- Three critical vulnerabilities identified
- BIIS proposal submitted as response
- Status: Under review

**2026-02-14 (Expected) - First Major Decision**
- Adopt BIIS → GFN v2.0 begins development
- Defer BIIS → Continue v1.0 with modifications
- Reject BIIS → Continue v1.0 unchanged
- Status: Pending decision

---

## Lessons from Framework Evolution

*[To be filled in as experience accumulates]*

### What We've Learned

1. **Framework maturation requires external critique**
   - Specification-based approaches have fundamental limits (Goodhart's Law)
   - Immune system metaphor more biologically plausible
   - Entropy-based monitoring harder to game than explicit metrics

2. **Community input is essential**
   - Red team identified problems we missed internally
   - Multiple expert perspectives strengthen proposals
   - Transparent evaluation builds trust

3. **Upgrade proposals need structured format**
   - 260X numbering enables version tracking
   - 01-04 subdirectories organize different aspects
   - Clear adoption criteria prevent arbitrary changes

---

## How to Monitor Progress

**Want to track 2601 BIIS progress?**
- Check GitHub issues tagged [#2601-biis]
- Read [2601_biis_proposal/](../2601_biis_proposal/) for latest details
- Check this file for status updates

**Want to propose a competing framework upgrade?**
- Follow [proposal_template.md](./proposal_template.md)
- Create 260X_[name]/ directory
- Launch for community review

**Want to see decision rationale?**
- Check back here after 2026-02-14 for core team decision
- See [decision_log.md](./decision_log.md) for detailed rationale

---

**Framework excellence requires transparency about evolution and improvement.** 🧬

Last updated: 2026-01-24
