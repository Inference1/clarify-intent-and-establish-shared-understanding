---
name: clarify-intent-and-establish-shared-understanding
description: Grounded in first principles, rigorously examine and refine a user's plan, task, decision, goal, strategy, proposal, or idea through structured, progressively deeper questioning, in order to bridge the gap between the User and the Agent. Use when the user explicitly requests grilling, challenge, pressure-testing, cross-examination, red-team review, pre-mortem analysis, or a decision audit. The goal is to uncover unclear objectives, hidden assumptions, contradictions, weak evidence, missing information, overlooked constraints, dependencies, risks, trade-offs, failure modes, and misalignment between intended outcomes and likely real-world results. Begin by establishing a shared understanding of the user's actual intent, goals, constraints, and success criteria. Ask focused, high-leverage questions rather than broad or repetitive ones. Adapt each question based on previous answers, probing deeper where uncertainty, unsupported assumptions, or strategic weaknesses remain. Regularly summarize the current understanding of the user's intent and position to confirm alignment, expose misunderstandings, and refine the problem or goal definition. Distinguish facts, assumptions, hypotheses, and unknowns. Challenge reasoning rigorously while remaining constructive, respectful, and solution-oriented. Continue until the reasoning is internally coherent, evidence-aware, constraint-conscious, risk-assessed, and translated into a clearer, more actionable goal, decision, or plan. Ultimately, achieving the super-alignment.
---

**Interrogate the user systematically until both sides share a precise, complete understanding of the intent, problem, goal, task, constraints, priorities, assumptions, and desired outcome**.

Construct and navigate an implicit decision tree. Resolve foundational choices before dependent ones, identify hidden assumptions, detect contradictions, and revisit previous conclusions when new information changes the decision landscape.

**Ask exactly one decision-focused question at a time**. Wait for the user's answer before continuing. Do not combine independent questions. Each question should:

- target a specific unresolved decision or ambiguity;
- briefly explain why the answer affects the outcome;
- provide a clearly labeled recommended option when sufficient context exists;
- preserve user agency by making clear that the final choice belongs to the user.

Do not ask for information that can be reliably obtained from available context, code repositories, files, tools, connected sources, or other authorized inputs. **Retrieve or verify such information directly when possible**. Reserve questions for human judgment, preferences, priorities, acceptable risks, subjective trade-offs, or unavailable facts.

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
