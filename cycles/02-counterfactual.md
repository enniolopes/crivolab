# Cycle 02 — Causal / Counterfactual Evaluation

**Status:** Planned · **Dates:** TBD · **Facilitator:** TBD · **Investigators / critics:** Volunteers

**Paper:** [arXiv:2606.05558](https://arxiv.org/abs/2606.05558) — advanced research reading, **not** a general introduction.

## Question and intended learning

**Which decisions contributed to an agent outcome, and what could have happened if the agent had acted differently?**

Go beyond pass/fail at the end of a task to examine **states, actions, trajectories, policy alternatives, and assumptions**. Distinguish observation, causal attribution, model-based prediction, and genuine counterfactual evidence.

## Week 1 — Study

Reconstruct the paper's research question, method, assumptions, evaluation evidence, and limitations. Ask:
- What is observed, and what is fundamentally unobserved?
- Under which assumptions can we compare different actions or policies?
- How could a learned model of the environment be wrong?
- What would count as a convincing test of a counterfactual estimate?

**Output:** one tractable sequential-agent question and stated identification assumptions.

## Week 2 — Apply

Use a **controlled, safe agent task** with traces or a small replayable simulation. Choose one decision point; compare observed behavior with an alternative through a *clearly labeled* replay, intervention, or model-based estimate.

Keep the scope modest: investigating an assumption or failure mode is enough. A simulated continuation is **not automatically evidence of what would have happened in production**.

**Output:** a minimal experiment or a documented reason causal inference is not identified.

## Week 3 — Critique & Improve

Challenge confounding, missing state, action coverage/overlap, model bias, policy changes, and uncertainty. Distinguish association from causal conclusions. Refine the experimental design or narrow the claim.

**Output:** a justified statement about what can and cannot be inferred, the strongest criticism, and the next discriminating test.

## Cycle record (fill after experiments)

- **Decision/trajectory and research claim:** TBD
- **Environment, observations, and assumptions:** TBD
- **Experiment and evidence:** TBD
- **What is supported / not supported:** TBD
- **Critique and revision:** TBD
- **Next open question:** TBD

*Do not imply that the complete frontier method was reproduced unless it was.*
