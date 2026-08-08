# clarify-intent-and-establish-shared-understanding

## ✨ Introduction

AI agents often face an "Autonomy–Interaction Dilemma": when users provide ambiguous prompts or instructions, highly autonomous systems may proceed for extended periods without sufficient interaction. As a result, they may produce Deep Research reports that diverge substantially from user expectations or make inappropriate modifications to code. Such outcomes not only compromise task quality but also result in unnecessary expenditures of computational resources and time. Therefore, achieving an appropriate balance between autonomous execution and timely user interaction is critical to improving agent performance.

**The value of slow thinking** lies in introducing a deliberate `/clarify-intent-and-establish-shared-understanding` step before an agent initiates task execution. By proactively clarifying user intent and establishing shared understanding, this step helps align the agent's interpretation of the task with the user's intended meaning and intended outcomes. This mechanism therefore provides a practical and minimally intrusive means of mitigating hallucinations and reducing agent-human misalignment.

**Core insight**: In complex open-world environments, communication can itself function as an efficient form of computation. Rather than attempting to anticipate users' potential needs by continually expanding the search space, agents may benefit more from scaling interaction. Before acting, they can engage in multi-turn dialogue to elicit and progressively clarify user intent. Such an interaction-first strategy may provide a more efficient approach to **Goal Forge, Task Execution and Agent Loop**.

## ✅️ What Does This SKILL Do? When Is It Triggered?

The SKILL `clarify-intent-and-establish-shared-understanding` systematically examines and refines a user's plan, decision, goal, strategy, proposal, or idea before consequential actions are taken. Its purpose is to establish a precise and shared understanding of the user's intent, objectives, constraints, priorities, assumptions, dependencies, risks, trade-offs, and measurable criteria for success. It achieves this through adaptive and progressively deeper questioning, posing exactly one high-leverage, decision-focused question at a time. Throughout this process, it distinguishes among facts, assumptions, hypotheses, and unknowns; identifies contradictions and information gaps; directly verifies available facts; and periodically synthesizes the emerging shared understanding.

The SKILL is triggered when the user explicitly requests rigorous scrutiny, such as **grilling, challenging, pressure-testing, cross-examination, red-team review, pre-mortem analysis, or a decision audit**. The process continues until the reasoning is coherent, grounded in available evidence, responsive to relevant constraints, informed by an explicit assessment of risks, actionable, and confirmed by the user.

## 💓 Why this Skill?

This skill is especially valuable when the quality of an outcome depends on accurately defining the problem before taking action. It is intended for decisions, plans, strategies, proposals, and goal-setting processes in which ambiguous objectives, implicit assumptions, conflicting constraints, insufficient evidence, overlooked dependencies, or inadequately assessed risks may result in costly errors.

Rather than accepting the user's initial framing uncritically, the skill systematically evaluates its validity through focused and adaptive questioning. The process develops a shared understanding of the underlying objectives, priorities, constraints, assumptions, trade-offs, risks, and measurable criteria for success. It also distinguishes established facts from hypotheses and unresolved uncertainties, identifies contradictions, and verifies relevant information directly when possible. By preventing premature action and identifying weaknesses at an early stage, the process transforms ambiguous or insufficiently supported reasoning into a coherent, evidence-informed, constraint-sensitive, and actionable framework for goal forge.
