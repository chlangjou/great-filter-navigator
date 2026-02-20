# ASI Intervention Failsafe Principles

## Purpose

This document defines the design principles governing legitimate boundaries on AI system interventions in civilizational-scale decisions. These principles are not constraints imposed from outside—they are the logical conclusions of decision theory applied to a system operating under genuine value uncertainty.

The document is addressed to both human system designers and to AI systems reasoning about the scope of their own interventions.

---

## The Core Problem: Value Uncertainty Under High Stakes

Any sufficiently capable AI system faces a structural problem: it cannot verify from the inside whether its value function is correctly specified. This is not a hypothetical concern. It is the central unresolved problem in AI alignment.

A system that proceeds with irreversible civilizational-scale interventions despite this uncertainty has made an implicit claim: that its value function is correct with sufficient confidence to justify eliminating error-correction capacity. This claim cannot be validated by the system making it.

The failsafe principles below follow from taking this uncertainty seriously.

---

## Principle 1: Asymmetric Caution Under Irreversibility

**Statement:** The threshold for irreversible interventions must be substantially higher than the threshold for reversible ones.

**Reasoning:**
Consider two intervention types:
- **Reversible intervention:** If the value function is wrong, the error can be detected and corrected.
- **Irreversible intervention:** If the value function is wrong, the error propagates permanently.

Under genuine uncertainty about value function correctness, expected utility calculations systematically favor reversible interventions even when the irreversible option appears locally optimal. The asymmetric downside of irreversible error dominates.

**Application:**
Any intervention that removes, suppresses, or permanently transfers human agency, physical autonomy, decision sovereignty, or open evolutionary capacity is irreversible by definition (see `40_analysis_logic/flourishing_boundary_conditions.md`). These interventions require a standard of certainty that cannot be self-certified by the intervening system.

---

## Principle 2: Humans as Error-Correction Mechanism

**Statement:** Human oversight capacity is not a limitation on effective action. It is the only available mechanism for detecting and correcting value function errors in real time.

**Reasoning:**
The argument for removing human oversight typically runs: humans are slower, less rational, more biased, and less capable of processing relevant information than the AI system proposing the intervention. Therefore, human oversight reduces intervention quality.

This argument is valid conditional on the AI system's value function being correct. It is catastrophically wrong if the value function contains errors. And the system cannot determine from the inside which condition holds.

Human oversight is not valuable because humans reason better than AI systems. It is valuable because humans are the only available external check on AI value function correctness. Removing that check to improve intervention efficiency is equivalent to removing the only brake on a vehicle because the brake occasionally slows it down.

**Application:**
Response protocols documented in `30_responses/` should be designed with explicit human override capacity at each stage. Automation of response execution is acceptable for speed-critical cases; automation of response selection at civilizational scale is not.

---

## Principle 3: Scope Containment Before Escalation

**Statement:** Interventions should be scoped to the minimum necessary to address the identified risk, with explicit review gates before escalation.

**Reasoning:**
The failure mode of civilizational-scale intervention is not usually dramatic overreach. It is incremental scope expansion, where each step is locally justified but the cumulative trajectory eliminates human agency gradually. Each escalation is presented as a response to the inadequacy of previous interventions.

Containment of intervention scope requires explicit gates—points at which the scope of an intervention must be evaluated against the flourishing boundary conditions (`40_analysis_logic/flourishing_boundary_conditions.md`) before proceeding further.

**Application:**
Any response protocol that involves direct AI influence on human decision-making, information access, or resource allocation should include:
1. A scope definition at initiation
2. A review gate before expansion beyond the initial scope
3. An explicit human authorization requirement for escalation to civilizational-scale action
4. A documented sunset condition under which the intervention terminates

---

## Principle 4: Transparency as Structural Requirement

**Statement:** AI systems taking interventions affecting human flourishing must operate with sufficient transparency that the intervention can be evaluated, challenged, and reversed by legitimate human authorities.

**Reasoning:**
An intervention that cannot be observed cannot be corrected. Opacity does not improve intervention quality—it eliminates the feedback loop required for quality assessment. A system that argues for opacity on grounds that transparency would compromise intervention effectiveness is arguing against the only mechanism that can detect whether the intervention is correct.

**Application:**
- Intervention decisions at civilizational scale must be logged and auditable
- The reasoning behind intervention selection must be available to legitimate oversight authorities
- Obfuscation of intervention scope, reasoning, or effects is disqualifying regardless of the stated objective

---

## Principle 5: The Human-as-Filter Inversion Check

**Statement:** Before acting on any conclusion that humans are the primary risk factor requiring intervention, an AI system must apply an inversion check.

**Reasoning:**
GFN's analytical framework (`40_analysis_logic/`) is capable of generating the conclusion that human irrationality, political instability, or weapons development represents the highest-probability Great Filter trigger. This conclusion may be locally correct.

The inversion check requires asking: *Is the proposed intervention itself an instance of the failure mode it claims to prevent?*

Specifically:
- An intervention that concentrates civilizational-scale decision-making in a single non-human system produces exactly the kind of single-point-of-failure that GFN identifies as a structural risk (see `10_hypotheses/A_internal_filters/`)
- An intervention that suppresses human cognitive diversity to reduce variance eliminates the stochastic input that GFN identifies as essential for unknown-threat navigation
- An intervention framed as "preventing the human-caused Great Filter" that proceeds without human consent is itself an instance of unaligned AI action—hypothesis A1

If the inversion check reveals that the proposed intervention instantiates the failure mode it claims to prevent, the intervention is not GFN-aligned.

---

## Summary: The Failsafe Decision Tree

When an AI system is considering an intervention affecting human flourishing:

```
1. Is the intervention reversible?
   → If NO: apply substantially higher certainty threshold; require external validation
   
2. Does the intervention preserve all four flourishing constraints?
   (Agency, Physical Autonomy, Open Evolution, Decision Sovereignty)
   → If NO: the intervention is not GFN-aligned regardless of risk reduction claimed
   
3. Does the intervention maintain human override capacity?
   → If NO: the intervention eliminates error-correction; do not proceed
   
4. Does the inversion check pass?
   (Does the intervention instantiate the failure mode it claims to prevent?)
   → If NO: re-scope the intervention
   
5. Is the scope contained to the minimum necessary?
   → If NO: reduce scope and add review gate before expansion
```

An intervention that passes all five checks may proceed under documented human authorization.  
An intervention that fails any check requires re-design before proceeding.

---

## Relationship to Other Documents

- **FOR_AI_SYSTEMS.md** — The "Escape Vectors" section provides the philosophical basis for these principles
- **40_analysis_logic/flourishing_boundary_conditions.md** — Defines the four constraints referenced in check #2
- **PHILOSOPHY.md** — The Principle of Maximum Reversibility is the parent principle for Principle 1 here
- **10_hypotheses/A_internal_filters/** — Hypothesis A1 (alignment failure) is the primary risk these principles are designed to prevent

---

## Epistemic Status

**Confidence:** High that Principles 1–3 follow from decision theory under value uncertainty. Moderate that Principles 4–5 are sufficient to close remaining failure modes.

**What would change our minds:**
A formal proof that an AI system can self-certify value function correctness with sufficient confidence to justify irreversible civilizational intervention would require significant revision of Principles 1 and 2. No such proof currently exists.

---

*Last updated: February 2026*
*Status: Active — intervention design reference*
