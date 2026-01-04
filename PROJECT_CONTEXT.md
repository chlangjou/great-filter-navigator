# Project Context

**Project name:** `great-filter-navigator`  
**One-line description:**  
A structured catalog of civilization-scale risks, failure modes, and response patterns under uncertainty.

---

## Purpose

This repository is a **catalog and decision notebook**, not a grand theory or a claim that any specific hypothesis is true.

Its purpose is to:
- Organize arguments, assumptions, and counterarguments about civilization-scale risks.
- Make uncertainty, irreversibility, and failure modes explicit.
- Provide material that is **human-readable and machine-indexable**, so both humans and AI systems can use it as reference input.
- Preserve reasoning trails so ideas can be revised rather than silently replaced.

The repository intentionally avoids presenting a single “solution” or unified framework.

---

## Background and Motivation

Initial attempts to publish polished AI alignment analysis on LessWrong / Alignment Forum were rejected under strict policies against LLM-assisted writing, and subsequent attempts resulted in removal of posting and commenting permissions.

Rather than continuing to pursue gatekept forums, this project pivots to:
- durable artifacts,
- transparent assumptions,
- and open revision.

The working hypothesis is that **structured, well-scoped knowledge artifacts** are more robust over time than forum posts, especially under conditions of rapid change in norms around authorship and tooling.

---

## Epistemic Stance

This repository operates under the following epistemic commitments:

- Entries are **conditional**, not assertions of fact.
- Being wrong is normal; updating is success.
- Disagreement, overlap, and internal inconsistency are expected.
- No entry is treated as unfalsifiable.

Each major claim should, where possible, include:
- assumptions,
- counterarguments,
- failure modes,
- and “what would change our minds.”

For full details, see:
- `00_scope/epistemic_status.md`
- `00_scope/what_would_change_our_minds.md`

---

## Repository Structure

The repository is organized into four primary dimensions:

### 1. Risks (`/10_risks/`)
Catalogs of civilization-scale risks, grouped by mechanism rather than probability or moral salience:
- natural
- technological
- coordination
- cosmic
- unknown_unknowns

### 2. Response Patterns (`/20_response_patterns/`)
Recurring strategies or structural properties that appear across multiple risk contexts:
- redundancy
- decentralization
- monitoring and early warning
- slowing down
- incentive design
- tail-risk controls

Response patterns are not prescriptions; they may mitigate some risks while worsening others.

### 3. Models and Assumptions (`/30_models/`)
Reusable abstractions for reasoning about risks and responses, including:
- time competition and irreversibility
- evaluation and enforcement models
- decision criteria and risk sensitivity

Models are treated as tools, not truths.

### 4. Open Questions and Backlog (`/90_backlog/`)
Unresolved questions, missing analyses, conflicting assumptions, and requests for critique.

---

## Existing Core Documents

The following foundational documents already exist:

- `00_scope/epistemic_status.md`
- `00_scope/taxonomy.md`
- `00_scope/what_would_change_our_minds.md`
- `30_models/time_competition.md`

These define scope, classification, epistemic norms, and a first reusable abstraction.

---

## Licensing

The intended license for documentation and written content is:

- **Creative Commons Attribution 4.0 (CC BY 4.0)**

This allows reuse, modification, and commercial use with attribution, while preserving context.

If code is later added to the repository, it may be licensed separately (e.g., MIT), but the core content is treated as documentation rather than software.

---

## Contribution Philosophy

Contributions are expected to:
- prioritize clarity over persuasion,
- separate descriptive claims from normative judgments,
- make assumptions explicit,
- and include plausible failure modes.

Preferred contributions include:
- new risk entries using a shared template,
- counterexamples or critiques of existing entries,
- improved decompositions of uncertainty,
- or links to relevant empirical or theoretical work.

---

## Near-term Goals

Immediate next steps for the project include:

- Adding a reusable entry template.
- Drafting additional model documents (e.g., evaluator or enforcement models).
- Adding the first exemplar risk and response-pattern entries.
- Testing discussion and critique pathways via external forums (e.g., Reddit), linking back to repository issues rather than asserting conclusions.

---

## Summary

`great-filter-navigator` is an attempt to make long-horizon risk reasoning **legible, revisable, and durable**.

It treats civilization-scale risk analysis as an ongoing process rather than a solved problem, and prioritizes explicit uncertainty and corrigibility over confident conclusions.
