# clarify-intent-and-establish-shared-understanding

## ✨ Introduction

AI agents often face an "Autonomy–Interaction Dilemma": when users provide ambiguous prompts or instructions, highly autonomous systems may proceed for extended periods without sufficient interaction. As a result, they may produce Deep Research reports that diverge substantially from user expectations or make inappropriate modifications to code. Such outcomes not only compromise task quality but also result in unnecessary expenditures of computational resources and time. Therefore, achieving an appropriate balance between autonomous execution and timely user interaction is critical to improving agent performance.

**The value of slow thinking** lies in introducing a deliberate `/clarify-intent-and-establish-shared-understanding` step before an agent initiates task execution. By proactively clarifying user intent and establishing shared understanding, this step helps align the agent's interpretation of the task with the user's intended meaning and intended outcomes. This mechanism therefore provides a practical and minimally intrusive means of mitigating hallucinations and reducing agent-human misalignment.

**Core insight**: In complex open-world environments, communication can itself function as an efficient form of computation. Rather than attempting to anticipate users' potential needs by continually expanding the search space, agents may benefit more from scaling interaction. Before acting, they can engage in multi-turn dialogue to elicit and progressively clarify user intent. Such an interaction-first strategy may provide a more efficient approach to **Goal Forge, Task Execution and Agent Loop**.

