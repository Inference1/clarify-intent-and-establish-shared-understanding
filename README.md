# clarify-intent-and-establish-shared-understanding

## 🚀 Quick Start

### Option 1: Ask Your Agent to Install It

Simply tell your agent:

`Install the clarify-intent-and-establish-shared-understanding skill from https://github.com/Inference1/clarify-intent-and-establish-shared-understanding for this project.`

### Option 2: Install with `npx skills`

The easiest command-line method is the [`skills`](https://github.com/vercel-labs/skills) CLI.

**Interactive installation**

```bash
npx skills add Inference1/clarify-intent-and-establish-shared-understanding
```

The installer will let you choose the target Agent and installation scope.

**Install for a specific Agent**

```bash
npx skills add Inference1/clarify-intent-and-establish-shared-understanding -a claude-code
```

Replace `claude-code` with the desired Agent identifier, such as `codex`, `cursor`, `github-copilot`, or `gemini-cli`.

Install globally for that Agent:

```bash
npx skills add Inference1/clarify-intent-and-establish-shared-understanding -a claude-code -g
```

**Install for all supported Agents**

Project-level:

```bash
npx skills add Inference1/clarify-intent-and-establish-shared-understanding --all
```

Global:

```bash
npx skills add Inference1/clarify-intent-and-establish-shared-understanding --all -g
```

Project-level installation is the default; `-g` / `--global` makes the Skill available across projects.

### Option 3: Install Manually

Download the repository as a ZIP from GitHub, or clone it:

```bash
git clone https://github.com/Inference1/clarify-intent-and-establish-shared-understanding.git
```

Then copy the repository folder into your Agent's **project-level** or **global** skills directory. Keep `SKILL.md` inside the Skill folder:

```text
<skills-directory>/
└── clarify-intent-and-establish-shared-understanding/
    └── SKILL.md
```

For example, with Claude Code:

```text
# Project-level
<project>/.claude/skills/clarify-intent-and-establish-shared-understanding/SKILL.md

# Global
~/.claude/skills/clarify-intent-and-establish-shared-understanding/SKILL.md
```

Common Agent locations include:

| Agent          | Project-level     | Global               |
| -------------- | ----------------- | -------------------- |
| Claude Code    | `.claude/skills/` | `~/.claude/skills/`  |
| Codex          | `.agents/skills/` | `~/.codex/skills/`   |
| Cursor         | `.agents/skills/` | `~/.cursor/skills/`  |
| GitHub Copilot | `.agents/skills/` | `~/.copilot/skills/` |
| Gemini CLI     | `.agents/skills/` | `~/.gemini/skills/`  |

For other Agents, use their documented skills directory or let `npx skills add` select the correct location automatically.

The `skills` CLI currently documents project scope as the default, `-g/--global` for user-wide installation, `-a/--agent` for targeting specific agents, and `--all` for installing all discovered skills to all supported agents. ([GitHub][2])

[1]: https://github.com/Inference1/clarify-intent-and-establish-shared-understanding "GitHub - Inference1/clarify-intent-and-establish-shared-understanding: Systematically clarify intent, challenge assumptions, resolve contradictions, and align goals, constraints, risks, and success criteria. · GitHub"
[2]: https://github.com/vercel-labs/skills "GitHub - vercel-labs/skills: The open agent skills tool - npx skills · GitHub"

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
