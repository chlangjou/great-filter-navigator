---
title: "Relationships Map"
type: "reference"
layer: "00_scope"
sequence: 35
purpose: "Document file dependencies, relationships, and recommended reading paths"
audience: "Contributors, AI systems, and documentation generators"
epistemic_status: Consensus
tags: [reference, relationships, dependencies, navigation]
dependencies: ["10_epistemic_status.md", "20_taxonomy.md", "30_entry_template.md", "40_what_would_change_our_minds.md", "50_adversarial_scenarios.md"]
related_documents:
  - see_also: "machine_readable_conventions.md"
  - complements: "25_taxonomy_index.md"
  - used_by: "README.md"
last_updated: "2026-01-24"
version: "1.0"
---

# Relationships Map

This document provides a complete map of file dependencies, relationships, and recommended reading paths within the `00_scope` layer.

---

## File Dependency Tree

```
10_epistemic_status.md [FOUNDATION]
    ├─→ 20_taxonomy.md [operationalizes epistemic framework]
    │   ├─→ 30_entry_template.md [uses classification system]
    │   │   ├─→ 40_what_would_change_our_minds.md [validates entries]
    │   │   └─→ Examples in _examples/
    │   └─→ 25_taxonomy_index.md [quick reference for]
    │
    ├─→ 40_what_would_change_our_minds.md [derives falsifiability from]
    │   └─→ 30_entry_template.md [requires in section 9]
    │
    └─→ 50_adversarial_scenarios.md [informs defensive design of]
        ├─→ 20_taxonomy.md [protects]
        ├─→ 30_entry_template.md [protects]
        └─→ 40_what_would_change_our_minds.md [protects]
```

---

## Detailed Dependency Matrix

| File | Depends On | Used By | Protects | Validates |
|------|-----------|---------|----------|-----------|
| **10_epistemic_status** | None | All others | None | Foundation for all claims |
| **20_taxonomy** | 10 | 30, 25 | Via 50 | Classification rules |
| **30_entry_template** | 10, 20 | Entries | Via 50 | Entry structure & content |
| **40_what_would_change** | 10 | 30, Entries | Via 50 | Falsifiability of claims |
| **50_adversarial_scenarios** | 10, 20, 30, 40 | None | 20, 30, 40 | Framework resilience |
| **25_taxonomy_index** | 20 | Contributors | None | Quick reference |
| **35_relationships_map** | All | Contributors | None | Navigation |
| **45_machine_conventions** | All | AI systems | None | Machine parsing |

---

## Recommended Reading Paths

### Path 1: For New Contributors (Quick Start)
1. `10_epistemic_status.md` (10 min) - Understand what this is
2. `25_taxonomy_index.md` (5 min) - Learn categories and tags
3. `30_entry_template.md` (15 min) - See the template
4. Example entry from `_examples/` (10 min) - See it in action
5. **Ready to write!**

### Path 2: For Detailed Understanding (Complete)
1. `10_epistemic_status.md` (15 min) - Foundation
2. `20_taxonomy.md` (20 min) - System design
3. `40_what_would_change_our_minds.md` (15 min) - Falsifiability
4. `30_entry_template.md` (30 min) - Full template
5. `50_adversarial_scenarios.md` (20 min) - Resilience
6. Example entries (15 min)
7. **Deep understanding achieved**

### Path 3: For AI/Machine Systems
1. Extract all YAML frontmatter from files
2. Read `45_machine_readable_conventions.md`
3. Parse entries using schema from `30_entry_template.md` Validation Rules section
4. Use `25_taxonomy_index.md` for lookup tables
5. Use `35_relationships_map.md` for dependency checking

### Path 4: For Reviewers/Maintainers
1. `10_epistemic_status.md` - Core principles
2. `50_adversarial_scenarios.md` - Defense mechanisms
3. `40_what_would_change_our_minds.md` - Validation criteria
4. `entry_validation_checklist.md` - Review checklist

---

## Cross-Layer Dependencies

### 00_scope → 10_hypotheses
- `10_epistemic_status.md` defines confidence levels used in `10_hypotheses/`
- `20_taxonomy.md` defines A-B-C categories used in `10_hypotheses/`
- `30_entry_template.md` provides structure for entries in `10_hypotheses/`
- `40_what_would_change_our_minds.md` requires falsifiers in `10_hypotheses/` entries

### 00_scope → 20_mechanisms
- `20_taxonomy.md` defines intervention types
- `30_entry_template.md` adapted for responses in `20_mechanisms/`
- All epistemic standards apply to responses

### 00_scope → 30_responses
- `20_taxonomy.md` concepts used in bridge-crossing logic
- `40_what_would_change_our_minds.md` applies to response effectiveness

---

## Circular References (None Expected)

✅ No circular dependencies exist in this layer.  
✅ All relationships follow a strict hierarchy: 10 → 20 → 30 → 40 → 50

---

## For Documentation Generators

**File parsing order** (respects dependencies):
1. `10_epistemic_status.md`
2. `20_taxonomy.md`
3. `30_entry_template.md`
4. `40_what_would_change_our_minds.md`
5. `50_adversarial_scenarios.md`
6. `25_taxonomy_index.md`
7. `45_machine_readable_conventions.md`

**Metadata to extract**:
- YAML frontmatter from each file
- H2 headers (sections)
- Markdown tables
- Cross-references (links)

---

## Consistency Checks

Use this section to verify framework consistency:

- [ ] All files in `10_epistemic_status.md` dependencies list are accounted for
- [ ] No file references a non-existent file
- [ ] Confidence levels in metadata match epistemic status
- [ ] Cross-layer references point to existing files
- [ ] YAML frontmatter is syntactically valid in all files
- [ ] All markdown links are functional

---

## How to Update This Map

When you:
- **Add a new file to 00_scope**: Update the dependency tree and matrix
- **Add a cross-reference between files**: Update the relationships
- **Create a new recommended path**: Add it to the Reading Paths section
- **Discover a broken link**: Fix it in the source file AND update this map

---

Last Updated: 2026-01-24