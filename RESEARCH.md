# Core Research Challenge: Eval Architect

## The research question

**How far can validity-centered evaluation design for AI agents be generalized and automated across different domains?**

Our experimental artifact, **Eval Architect**, investigates whether an AI agent can **design, implement, and critique evaluations of other agents**, given sufficient information about their tasks and contexts.

**Domain-agnostic ≠ context-free.** No evaluation is valid in the abstract. It depends on the target agent's mission, environment, population, constraints, risks, and intended use of the results. A good Eval Architect must request missing context and sometimes refuse to make a strong claim.

This is a **research challenge, not a product deadline**. Its purpose is to connect papers, experiments, and shared learning. Members may work on their own agent-evaluation problems instead.

## The foundational distinction

```text
What is the system supposed to do?
  → Which claim matters for a real decision?
  → Is the target a directly observable criterion or a latent construct?
  → Which evidence would discriminate success from failure?
  → Which measurements and evaluators can produce that evidence?
  → What interpretation is warranted, for which population and conditions?
  → What is NOT established?
```

**Measurement ≠ evaluation ≠ claim.** A high tool-call success rate does not, by itself, establish good agent decisions or successful missions. Even a high task score may not justify claims about broad autonomy, safety, or general reliability.

Distinguish at least three levels when relevant:

| Level | Question |
| --- | --- |
| **Tool / MCP** | Did the tool execute the requested operation correctly? |
| **Agent policy / trajectory** | Did the agent choose appropriate tools, arguments, sequence, recovery, and stopping? |
| **Mission outcome** | Did the overall task actually succeed under its constraints? |

Then ask a fourth question: **Does this evidence actually warrant the intended claim?**

Classical software tests verify defined invariants; agent evals also examine variable behavior, task distributions, judgment quality, and the validity of inferences. They complement rather than replace each other.

## Input and output: minimal research contract

**Input:** target agent description or access; one concrete capability/mission; users or task population; environment/tools; operational constraints and risks; available traces/test data; intended decision; and missing information explicitly marked.

**Proposed output (not yet implemented):**

1. **Claim design:** relevant capability, construct/criterion, bounded and decision-relevant claims, assumptions.
2. **Evidence plan:** task distribution, representative and failure cases, measures, human or deterministic reference criteria, sampling and uncertainty.
3. **Evaluation specification:** scenarios, graders/verifiers, tool/policy/outcome observations, baseline and reproducibility requirements.
4. **Validity argument:** content, criterion, construct, external, and consequential threats *where relevant*; what the results would and would not establish.
5. **Critique:** ways a weak agent or flawed evaluator could score well; missing evidence; next discriminating test.
6. **Optional implementation:** a runnable harness, produced with coding-agent assistance and independently tested.

Selecting **which claim matters** is part of the research. Do not merely fill a standardized claim sentence with plausible-looking variables.

## Progression (hypotheses, not commitments)

- **Stage 0 — Human baseline:** humans design and critique a validity argument on a bounded agent capability.
- **Stage 1 — Eval design:** Eval Architect proposes claims, evidence plans, and explicit limits; humans challenge them.
- **Stage 2 — Execution:** generate and run checks or test harnesses; verify that graders catch seeded failures and avoid trivial false positives.
- **Stage 3 — Sequential evaluation:** investigate agent trajectories, decisions, and counterfactual estimates with assumptions and uncertainty stated.

The first cycle should prioritize **valid evaluation design**, not a full autonomous eval platform.

## Evaluating the evaluator

We must not accept "the agent generated an eval" as proof that the eval is valid. Start with **multiple distinct target contexts**, e.g. repository investigation, evidence-based research, and tool-driven workflows. Compare its proposals with independent expert reasoning and deliberate counterexamples.

The strongest early checks are whether it can **construct, critique, and repair** evaluations on *unseen* problems: choose meaningful claims, detect proxy failures, delimit scope, find unsupported inferences, and revise weak evaluation designs.

Protect against self-grading, shared judge bias, benchmark gaming, data leakage, superficial templates, and overclaims from tiny samples. An impressive report is not evidence of validity by itself.

## How this connects to delegated coding

A coding agent may implement the evaluation infrastructure, but the delegation contract must state the **claim, acceptance criteria, required evidence, and boundaries**. The delegated implementation itself needs checks: does the harness run, detect known failures, and record the claimed signals accurately?

**Completion means evidence supports the defined acceptance claim—not that the coding agent says the task is finished.**

## Open research questions

- Can claim selection be automated without substituting easy proxies for decision-relevant capabilities?
- When is context insufficient to support a defensible evaluation?
- What evidence discriminates good validity reasoning from convincing template completion?
- How do we evaluate judges, task coverage, generalization, and consequences?
- Under what assumptions can we attribute outcomes to agent decisions or estimate unobserved alternatives?

**Status:** research definition only. No validated universal Eval Architect or experimental results are claimed here.
