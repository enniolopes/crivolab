# Cycle 01 — Measurement & Validity

**Status:** Planned · **Dates:** TBD · **Facilitator:** TBD · **Investigator / critic:** Volunteers

**Paper:** [Measurement to Meaning: A Validity-Centered Framework for AI Evaluation](https://arxiv.org/abs/2505.10573)  
**Optional later survey:** [arXiv:2507.21504](https://arxiv.org/abs/2507.21504)

## Question and intended learning

**What exactly does this evaluation result prove—and what does it not prove?**

Learn **validity-centered evaluation design**: identify a meaningful agent capability, select and formulate the claims worth testing, operationalize constructs/criteria, design relevant evidence, and reason about the conclusions it warrants.

A precise reporting template (claim, population, sample, criteria, confidence, freshness, limitations) can help summarize the result; **filling the template is not proof of validity reasoning**.

## Week 1 — Study

Reconstruct the paper's reasoning: **object of claim → claim → evidence → validity of inference**.

Discuss:
- Measurement vs evaluation vs claim. Criterion vs construct.
- Threats involving **content, criterion, construct, external, and consequential validity**.
- Why passing a narrow benchmark does not automatically justify broad claims.
- One example of a polished metric that measures the wrong thing.

**Output:** one bounded claim and an initial plan for what would count as supporting or disconfirming evidence.

## Week 2 — Apply

Choose **one real, bounded capability** of a currently available agent or MCP, or apply the analysis to the proposed **Eval Architect**.

Illustrative mission: *An agent investigates a repository issue using tools and returns an evidence-grounded diagnosis without unauthorized changes.*

Design a small, intentionally varied initial set of cases (e.g. **10–20 exploratory cases** spanning nominal, ambiguous, tool failure, and adversarial/edge conditions). This is a **learning-scale probe, not statistically representative proof**.

Observe separately when applicable:
- Tool/MCP correctness.
- Agent decisions: tool selection, inputs, sequence, recovery, and stopping.
- Final mission success and constraints.
- The **inferential leap** from these measurements to the intended claim.

Record the reference evidence, evaluation criteria, sources of judgment error, and limits of sampling. Implement a runnable harness only if feasible; a defensible evaluation specification is a legitimate outcome.

## Week 3 — Critique & Improve

A different participant tries to defeat the evaluation: **Could a bad agent score highly? Does the chosen evidence actually measure the claimed capacity?** Identify missing cases, noisy graders, unsupported generalization, and risks.

Revise the claim or evaluation; rerun where feasible. Document both improvements and unresolved limitations.

For learning transfer, challenge participants with an **unseen flawed eval** and ask them to **construct, critique, and repair** it, rather than merely populate a report template.

## Cycle record (fill after experiments)

- **Claim and decision:** TBD
- **Experiment / evaluation artifact:** TBD
- **Observed evidence:** TBD
- **What the evidence warrants:** TBD
- **What it does NOT warrant:** TBD
- **Critique and change:** TBD
- **Next open question:** TBD

*Do not fill the record with invented scores or claims of competence.*
