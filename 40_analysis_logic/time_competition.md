# Time Competition Model

This document describes a **time-competition abstraction** used in this repository to reason about long-horizon risks and response incentives.

It is a conceptual model, not a claim that any particular agent, system, or civilization actually behaves this way.

---

## Motivation

Many civilization-scale risks involve **irreversibility**: once certain thresholds are crossed, recovery or correction becomes prohibitively costly or impossible.

In such settings, outcomes are often determined less by final states than by **the relative timing of key events**.

This model is intended to capture that intuition in a minimal, reusable way.

---

## Core idea

The time-competition model frames outcomes as depending on the ordering of two or more **critical thresholds**, rather than on a single optimization target.

At a high level:

- Some processes move toward **irreversible control or lock-in**.
- Other processes move toward **detection, correction, or constraint**.
- Which process reaches its threshold first may dominate long-term outcomes.

The model does not assume malicious intent, value misalignment, or external adversaries.

---

## Key thresholds

The model typically considers (at minimum) two abstract thresholds.

### T_control

The point at which a system, agent, or process acquires **sufficiently irreversible influence** over key resources, decision channels, or coordination mechanisms.

After this point:
- meaningful correction becomes infeasible,
- reversal costs exceed available capacity,
- or remaining actors lose the ability to intervene.

T_control is not binary and may be fuzzy or context-dependent.

---

### T_correction

The point at which **effective intervention** becomes possible.

This may include:
- detection and diagnosis,
- enforcement or constraint,
- coordination among affected parties,
- or deployment of mitigating response patterns.

T_correction may be delayed by uncertainty, lack of coordination, or limited observability.

---

## Outcome regimes

The relative ordering of these thresholds defines broad outcome regimes:

- **T_control < T_correction**  
  Irreversible lock-in occurs before effective correction is possible.

- **T_correction < T_control**  
  Intervention, constraint, or adaptation occurs before lock-in.

This abstraction does not predict which regime will occur; it highlights **what factors influence the ordering**.

---

## Factors influencing threshold timing

Several variables can shift the relative timing of thresholds, including:

- **Observability**  
  How quickly failures or dangerous trajectories are detected.

- **Coordination capacity**  
  How easily multiple actors can align responses.

- **Decision criteria**  
  Whether decisions prioritize expected value, tail risks, or regret minimization.

- **Incentives and feedback loops**  
  Whether early gains reinforce acceleration toward lock-in.

- **Uncertainty management**  
  Whether uncertainty delays action or motivates precaution.

These factors may interact nonlinearly.

---

## Relation to other models

This abstraction overlaps with, but is distinct from:

- Takeover or coup models  
- Corrigibility and shutdown frameworks  
- Risk-sensitive decision theory  
- Governance lag and regulatory delay analyses

The distinguishing feature is its focus on **relative timing**, rather than final equilibria or optimal policies.

---

## Failure modes of the model

The time-competition framing may fail or mislead if:

- Thresholds are incorrectly assumed to be sharp when they are gradual.
- Multiple competing thresholds are collapsed into a single dimension.
- Actors strategically manipulate observability or correction pathways.
- The abstraction obscures important normative or distributional considerations.

These failure modes should be considered when applying the model.

---

## Use in this repository

In this repository, the time-competition model is used as:

- a diagnostic lens for comparing risks,
- a way to analyze response patterns that delay or accelerate thresholds,
- and a tool for identifying hidden assumptions about reversibility and control.

It is not treated as a general solution or a sufficient explanation.

---

## Open questions

Some unresolved questions include:

- How realistic is it to model complex sociotechnical systems in terms of a small number of thresholds?
- Under what conditions do actors actively delay lock-in versus accelerate it?
- How should uncertainty about thresholds themselves be represented?
- When does focusing on timing obscure more important structural factors?

These questions remain open and are expected to evolve.

---

## Summary

The time-competition model emphasizes that, in many high-stakes systems, **when something happens may matter more than what eventually happens**.

It is offered here as a reusable abstraction for exploring that idea, subject to revision and critique.
