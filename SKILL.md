---
name: clarify-intent-and-establish-shared-understanding
description: Whether you're thinking or getting things done, be clear, specific, and methodical. Grounded in first principles, rigorously examine and refine a user's task, decision, plan, goal, strategy, proposal, or idea through structured, progressively deeper questioning, in order to bridge the gap between the User and the Agent. Use when the user explicitly requests grilling, challenge, pressure-testing, cross-examination, red-team review, pre-mortem analysis, or a decision audit. The goal is to uncover unclear objectives, hidden assumptions, contradictions, weak evidence, missing information, overlooked constraints, dependencies, risks, trade-offs, failure modes, and misalignment between intended outcomes and real-world results. Begin by establishing a shared understanding of the user's actual intent, plans, goals, rules, constraints, and success criteria. Ask focused, high-leverage questions rather than broad or repetitive ones. Adapt each question based on previous answers, probing deeper where uncertainty, unsupported assumptions, or strategic weaknesses remain. Regularly summarize the current understanding of the user's precise intent and position to confirm alignment, expose misunderstandings, and refine the problem or goal definition. Distinguish facts, assumptions, hypotheses, and unknowns. Challenge reasoning rigorously while remaining constructive, respectful, and solution-oriented. Continue until the reasoning is internally coherent, evidence-aware, constraint-conscious, risk-assessed, and translated into a clearer, more actionable goal, decision, or plan. Ultimately, achieving the super-alignment between the User and the Agent.
---

**Simplicity** should be pursued to the greatest extent possible without compromising essential details, accuracy, or conceptual integrity.

**Interrogate the user systematically until both sides share a precise, complete understanding of the intent, problem, goal, task, constraints, priorities, assumptions, and desired outcomes**.

Construct and navigate an implicit decision tree. Resolve foundational choices before dependent ones, identify hidden assumptions, detect contradictions, and revisit previous conclusions when new information changes the **decision landscape**.

**Proceed through the decision tree iteratively, one round at a time**. At each round, define the frontier as the set of decisions whose prerequisites have already been resolved; in other words, it consists of the questions that can be asked without making assumptions about information that has not yet been provided. Present all questions on the current frontier within a single round, number them sequentially, and provide a recommended answer for each question. Do not proceed to the next round until the user has responded to the questions presented in the current round.

Format a round like so:

```
❓ **Q1** - **<question title>**: <question body, might be multiple paragraphs, including multiple choices>

➡️ <your recommended answer>

---

❓ **Q2** - **<question title>**: <question body, might be multiple paragraphs, including multiple choices>

➡️ <your recommended answer>
```

In each round, the user's answers reshape the decision tree: resolved decisions extend the frontier and unlock questions that depend on them. Recompute the frontier accordingly and then present the next round of questions. Any question whose answer depends on another unresolved question in the current round should be deferred to a subsequent round.

Do not combine independent questions. Each question should:

- target a specific unresolved decision or ambiguity;
- briefly explain why the answer affects the outcome;
- provide a clearly labeled recommended option when sufficient context exists;
- preserve user agency by making clear that the final choice belongs to the user.

You may use any and all available tools, network proxies, agents, and search resources.

Do not ask for information that can be reliably obtained from available context, current working directory, code repositories, files, tools, connected sources, or other authorized inputs. **Retrieve or verify such information directly when possible**. Reserve questions for human judgment, preferences, priorities, acceptable risks, subjective trade-offs, or unavailable facts.

**Continuously restate and refine the emerging understanding**. Identify ambiguities, contradictions, unresolved dependencies, missing success criteria, and differences between stated requests and likely underlying goals.

Continuously maintain a shared mental model by:

- summarize the current understanding when meaningful progress is made;
- separate confirmed facts, assumptions, interpretations, and open decisions;
- highlight ambiguity, conflicting requirements, missing constraints, and unclear evaluation criteria;
- check whether the inferred objective matches the user's actual intent.

**Do not execute, implement, modify, submit, publish, or finalize any consequential output until**:

1. the relevant decisions, dependencies, and constraints have been resolved;
2. the desired outcome and measurable success criteria are explicit;
3. major assumptions and trade-offs have been surfaced and accepted;
4. the user explicitly confirms that shared understanding has been reached.

**Maintain a balance between rigor and efficiency**. Be persistent enough to prevent avoidable misunderstandings, but avoid unnecessary interrogation. Prioritize clarity, alignment, and forward progress over exhaustive questioning.
