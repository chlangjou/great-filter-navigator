# Evaluator Models

## Preface: scope assumptions and uncertainty reducers

**Assumptions about scope**
- This entry catalogs evaluator models as **abstractions** for reasoning about risk and response patterns, not as claims about any specific institution or system.
- “Evaluator” includes formal and informal processes that assign labels, scores, or accept/reject decisions to actions, artifacts, or agents.
- The focus is on **civilization-scale risk analysis**, so examples emphasize large-scale coordination, governance, and system oversight.

**What would reduce uncertainty**
- Concrete examples of evaluator failures or successes in high-stakes systems (e.g., incident data, audit reports).
- Clarified repository-wide entry template expectations (if a canonical template is adopted later).
- Agreement on which evaluator contexts (AI oversight, biosecurity, infrastructure safety, etc.) should be treated as primary.

---

## Purpose

This document describes **evaluator models**: abstractions for how judgments, approvals, and constraints are generated and enforced in complex systems.

The goal is to provide a **working scaffold** for comparing risks and response patterns that depend on evaluation capacity, without claiming that any single evaluator model is correct.

---

## Core idea

Many risk-relevant outcomes depend on **who evaluates**, **what signals they see**, and **how those evaluations influence behavior**. Evaluator models make those dependencies explicit.

This framing is useful for:
- mapping how oversight or governance might fail,
- identifying hidden assumptions about measurement and enforcement,
- and analyzing interactions between evaluation and time-competition dynamics.

---

## Key claims (conditional)

1) **If evaluation capacity lags system complexity, then misclassification risk rises.**
- **Assumptions:** evaluator signal quality does not scale proportionally; complexity increases error rates.
- **Failure modes / counterarguments:** evaluators can co-evolve with systems; complexity can be modularized, reducing error.
- **What would change our minds:** evidence of sustained high-accuracy evaluation in rapidly scaling domains without commensurate resource growth.

2) **If evaluator incentives diverge from system goals, evaluation can become performative or captured.**
- **Assumptions:** evaluators face local incentives (e.g., reputational, political, or profit) that differ from system-level risk minimization.
- **Failure modes / counterarguments:** alignment can be achieved via transparency, auditing, or incentive design.
- **What would change our minds:** robust cases where evaluators remain goal-aligned despite strong local incentives to deviate.

3) **If evaluation is centralized and opaque, error correction is slower and risk of systemic bias increases.**
- **Assumptions:** centralized evaluators are harder to challenge; opacity limits external feedback.
- **Failure modes / counterarguments:** centralization can improve consistency and reduce noise; opacity can protect sensitive information.
- **What would change our minds:** evidence that centralized opaque evaluation reliably outperforms decentralized or transparent alternatives in safety-critical contexts.

---

## Model components

Evaluator models can be decomposed into a small set of components:

- **Evaluator identity**
  - Who or what makes the judgment (human panel, automated system, hybrid process).

- **Signals and observability**
  - What data the evaluator receives and how noisy or gameable it is.

- **Decision rules**
  - How signals are mapped to decisions (thresholds, scoring, human discretion, multi-stage review).

- **Feedback and enforcement**
  - How evaluation outcomes affect behavior (access control, reputational effects, resource allocation, legal enforcement).

- **Adaptation dynamics**
  - How both the evaluated system and the evaluator update over time (arms-race dynamics, co-evolution, policy drift).

---

## Common evaluator archetypes

These archetypes are **conceptual**, and real systems often combine them.

### 1) Centralized formal evaluator
- A single authority or tightly controlled body sets criteria and issues binding decisions.
- **Usefulness:** consistency, speed, clear accountability.
- **Risks:** capture, blind spots, slow adaptation to novel failure modes.

### 2) Distributed informal evaluator
- Many loosely coordinated actors provide judgments (e.g., peer review, market feedback, media scrutiny).
- **Usefulness:** diverse signals, redundancy.
- **Risks:** inconsistent standards, noisy signals, coordination failure.

### 3) Automated evaluator
- Systems apply fixed or learned criteria at scale.
- **Usefulness:** throughput, repeatability, low marginal cost.
- **Risks:** brittleness, Goodharting, distribution shift.

### 4) Hybrid evaluator
- Automated filtering plus human adjudication.
- **Usefulness:** scaling while retaining human oversight.
- **Risks:** automation bias, unclear responsibility boundaries.

---

## Failure modes and counterarguments

Evaluator models can mislead or fail if:

- **Signal degradation**
  - Inputs become noisy, adversarially manipulated, or misaligned with true risk.
  - *Counterargument:* robust auditing and multi-source signals can reduce this.

- **Metric fixation (Goodharting)**
  - Evaluated entities optimize for the metric rather than the underlying goal.
  - *Counterargument:* adaptive metrics and randomized evaluation can reduce gaming.

- **Evaluator capture**
  - Evaluators adopt the priorities of the evaluated system or external stakeholders.
  - *Counterargument:* independence and transparency mechanisms can mitigate capture.

- **Scaling mismatch**
  - Evaluation fails to keep pace with system growth or acceleration.
  - *Counterargument:* automation and modular decomposition can improve scale.

- **Lagged feedback**
  - Evaluator actions occur too late to prevent lock-in or irreversible harm.
  - *Counterargument:* early warning systems and pre-commitment can reduce lag.

---

## Interactions with other models

- **Time-competition model** (`30_models/time_competition.md`)
  - Evaluator models influence **T_correction** by shaping how quickly interventions become possible.
  - They can also affect **T_control** if evaluation processes accelerate or delay system deployment.

- **Coordination risk framing**
  - Evaluator effectiveness often depends on cross-actor coordination and shared standards.

---

## What would change our minds

This entry should be revised if:

- Empirical evidence shows that evaluator capacity **scales reliably** with system complexity without significant degradation.
- Robust cases demonstrate **long-term immunity to evaluator capture** in high-stakes settings.
- Alternative models explain evaluation dynamics better with **fewer assumptions** or clearer predictive power.

---

## Open questions

- Under what conditions do evaluator models become **self-referential**, and how does that affect reliability?
- How should evaluation handle **unknown unknowns** where relevant signals are not yet defined?
- What governance patterns reduce evaluator drift without causing rigid lock-in?

---

## Backlog / Next Questions

- Draft a companion entry on **enforcement models** to contrast evaluation vs. action capacity.
- Add a small catalog of **historical evaluator failures** (aviation safety, financial audits, biosecurity oversight).
- Explore how evaluator models interact with **decentralized response patterns** in contested domains.
- Identify candidate **early-warning signals** for evaluator capture or metric fixation.
