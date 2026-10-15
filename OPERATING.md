# How CRIVO Lab works

## The agreement

- **Goal:** build transferable research and engineering competence in AI agent evaluation.
- **Approach:** study a meaningful problem, test an idea, challenge the evidence, improve our understanding.
- **Not:** a lecture series, a mandatory software team, a leaderboard, or a paper-count competition.
- **Time:** one **60-minute meeting per week**; roughly **1–2 hours/week** for regular participation. More involvement is voluntary.
- **Access:** researchers, students, and practitioners at different levels are welcome. Members may return at any cycle.

Why this format: **reading without application doesn't demonstrate transfer; application without critique can reward misleading evidence; mandatory delivery turns research into a product sprint.**

## One cycle = three weeks

| Week | Meeting focus (60 min) | What should exist afterward |
| --- | --- | --- |
| **1 — Study** | 10 min problem; 20 min paper reasoning; 20 min critical discussion; 10 min experiment scope | One question and a feasible experiment or critique plan |
| **2 — Apply** | 10 min hypothesis; 35 min working clinic; 15 min evidence check | An experiment, a design, or an explicit blocker with evidence |
| **3 — Critique & Improve** | 10 min findings; 30 min cross-review; 15 min revision plan / rapid fix; 5 min synthesis | A corrected result or documented limitation and a short cycle record |

Most building happens **asynchronously**. Do not use the meeting as a status-report ceremony. If implementation is too large, reduce scope. Never invent results to complete a cycle.

## Roles, not bureaucracy

| Role | Responsibility | Load |
| --- | --- | --- |
| **Facilitator** (rotates each cycle) | Posts the question and paper, hosts the three meetings, ensures the cycle note is closed | Small, time-boxed |
| **Investigator(s)** (volunteers) | Own a real question or agent capability, run the experiment, show evidence | Optional, scope agreed upfront |
| **Critic(s)** (different participants) | Try to falsify the inference, identify weaknesses, propose a discriminating test | A focused review |
| **Everyone** | Bring a question, interpret evidence, contribute constructively | No individual report required |

A **problem owner** can provide a research or engineering problem and relevant context without committing to implementing the solution. Rotate roles to avoid dependence on the founder. No volunteer experiment means the cycle can be a *design-and-critique* cycle.

## The only required artifact

Maintain **one short Markdown record per cycle** (see [template](cycles/TEMPLATE.md)). It should say what we asked, what we tried, what the evidence does and does not justify, what critique changed, and what remains open. Link to code, traces, datasets, or issues instead of duplicating them.

No compulsory slide decks, individual weekly reports, or extra dashboards.

## How to join or contribute

1. Read [README](README.md) and the current entry in [ROADMAP](ROADMAP.md).
2. Attend a session; ask a question or review an argument. Having an agent/codebase is **not** required.
3. Want to investigate? Propose a bounded problem via a GitHub issue or volunteer in the cycle discussion.
4. Want to improve the shared memory? Open a small PR to a cycle record or research document.

Use Discord for fast discussion and GitHub for outcomes that must survive chat history. **Meeting day/time and Discord invitation are not confirmed**; add them to README once agreed.

## Standards for evidence and discussion

- Distinguish **measurement**, **interpretation**, and **claim**. Write down the claim the evidence supports—and what it **does not** support.
- Separate observed findings from hypotheses and future work; link primary artifacts when possible.
- Welcome disagreement and negative results; challenge arguments, not people.
- No private credentials, sensitive agent traces, proprietary code, or third-party data without permission.
- Agree on public release, credit, authorship, and licensing before publishing shared artifacts. This private repository does **not** grant permission to redistribute others' material.
- Use AI coding agents for implementation as useful; independently examine experiment design, assumptions, tests, and results. A generated eval does not certify itself.

## When the format starts failing

| Warning sign | Do this |
| --- | --- |
| One person does all the preparation | Rotate facilitation, split small tasks, or postpone a cycle. |
| Meetings turn into passive presentations | Start with a concrete question and discuss competing answers. |
| Experiments become an obligation or stall | Cut scope; a reviewed design or documented negative result counts. |
| Everyone feels they learned, but cannot handle a new case | Test transfer on an unfamiliar problem; change the method, not the attendance target. |

## After the first two cycles (six-week pilot)

Ask three questions: **(1)** Can participants apply the ideas to a *new* case? **(2)** Did we produce reusable evidence or better methods? **(3)** Was participation sustainable without one person doing everything?

Keep, simplify, or change the format based on observed results. Do not treat attendance or filled-in templates as proof of learning. If an entire paper cannot be applied within a week, test one claim or assumption instead.

## Short invitation text

> CRIVO Lab is a lightweight AI Agent Evaluation research group. We meet weekly and explore one important question through a three-week loop: **Study → Apply → Critique & Improve**. We read research, try ideas on real agent problems, and review what the evidence truly supports. Our shared challenge is to investigate whether an AI agent can design rigorous evaluations of other agents across domains. Reading, experimental work, and critical review all count; coding is voluntary. Start with the [README](README.md) and [Roadmap](ROADMAP.md). Meeting details will be announced.
