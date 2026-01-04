# Taxonomy

This document describes the **organizational taxonomy** used in this repository.

The purpose of this taxonomy is not to assert that these categories are exhaustive or correct, but to provide a **stable working structure** for cataloging civilization-scale risks, assumptions, and response patterns under uncertainty.

Alternative taxonomies are possible, and disagreement about classification is expected.

## High-level structure

The repository is organized into four primary dimensions:

1. **Risks** — things that could plausibly threaten long-term civilization survival.
2. **Response Patterns** — recurring strategies that appear across many different risk contexts.
3. **Models and Assumptions** — abstractions used to reason about risks and responses.
4. **Open Questions and Backlog** — areas of uncertainty, disagreement, or missing analysis.

Each dimension is intentionally separated to avoid conflating:
- what might go wrong,
- how we might respond,
- and the assumptions used to reason about both.

---

## 1. Risks

Risks are organized by **mechanism**, not by probability or moral salience.

The goal is to group risks that fail or propagate in similar ways, even if their surface causes differ.

### 1.1 Natural risks (`/10_risks/natural`)

Risks arising primarily from non-anthropogenic physical processes.

Examples:
- Solar storms
- Asteroid or comet impacts
- Supervolcanic eruptions
- Long-term climate shifts driven by natural cycles

These risks are often:
- hard to influence directly,
- partially predictable,
- mitigated via monitoring, redundancy, or resilience.

---

### 1.2 Technological risks (`/10_risks/technological`)

Risks arising from human-created systems with failure modes that scale faster than governance or correction.

Examples:
- Advanced AI systems
- Biotechnology misuse
- Autonomous weapons
- Complex infrastructure cascades

Key features:
- rapid capability growth,
- feedback loops,
- asymmetric failure costs.

---

### 1.3 Coordination risks (`/10_risks/coordination`)

Risks driven primarily by failures of collective action rather than physical constraints.

Examples:
- Arms races
- Tragedy of the commons
- Regulatory capture
- Mistrust-driven escalation

These risks often interact strongly with technological risks.

---

### 1.4 Cosmic and external risks (`/10_risks/cosmic`)

Risks originating outside the Earth system or outside current human control.

Examples:
- Rare astrophysical events
- Unknown external shocks
- Hypothesized great-filter-style mechanisms

This category includes speculative risks, with explicit uncertainty.

---

### 1.5 Unknown unknowns (`/10_risks/unknown_unknowns`)

A placeholder category for risks that are poorly characterized or currently outside known models.

Entries here should focus on:
- indicators of model incompleteness,
- historical analogies,
- reasons current taxonomies might fail.

---

## 2. Response Patterns

Response patterns are **strategies or structural properties** that recur across multiple risk types.

They are not prescriptions, but **candidate approaches** that may succeed or fail depending on context.

Located in `/20_response_patterns/`.

Common categories include:

- **Redundancy** — multiple independent systems or pathways.
- **Decentralization** — avoiding single points of failure.
- **Monitoring and early warning** — detecting problems before irreversible damage.
- **Slowing down** — delaying irreversible actions under uncertainty.
- **Incentive alignment** — shaping behavior via rewards, penalties, or norms.
- **Tail-risk controls** — prioritizing worst-case outcomes over expected value.

A single response pattern may mitigate one risk while exacerbating another.

---

## 3. Models and Assumptions

Located in `/30_models/`.

This section captures **abstractions used to reason about risks and responses**, including:

- Evaluation and enforcement models
- Time-horizon assumptions
- Observer or oversight assumptions
- Decision criteria (e.g., expected value vs tail-risk sensitivity)

Models are treated as:
- tools, not truths,
- context-dependent,
- subject to failure modes of their own.

---

## 4. Open Questions and Backlog

Located in `/90_backlog/`.

This section tracks:
- unresolved questions,
- missing analyses,
- conflicting assumptions,
- requests for critique or expansion.

This area is explicitly provisional and expected to change frequently.

---

## Cross-cutting principles

Across all categories, contributors are encouraged to:

- Separate **descriptive claims** from **normative judgments**.
- State assumptions explicitly.
- Include plausible failure modes.
- Note interactions between different risks and response patterns.

---

## Summary

This taxonomy is a **working scaffold**, not a final ontology.

Its value lies in enabling comparison, critique, and revision across a diverse and uncertain search space, rather than in asserting a particular worldview.
