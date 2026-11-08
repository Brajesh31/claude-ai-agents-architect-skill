# claude-ai-agents-architect-skill

A Claude Code skill for designing controllable, reliable AI agent systems with tools, memory, planning, and multi-agent coordination.

## Overview

This skill focuses on the architecture of agents that can take actions while remaining understandable and constrained. It helps define agent responsibilities, select tools, design memory, structure planning loops, and coordinate multiple agents when a single agent is insufficient.

## Main Capabilities

- Design agent architecture and responsibilities.
- Define tool and function-calling contracts.
- Choose planning and reasoning strategies.
- Design short-term and persistent memory.
- Coordinate multiple agents.
- Define permission and approval boundaries.
- Handle failures and graceful degradation.
- Evaluate agent behavior and reliability.
- Debug tool selection and execution problems.

## Architecture Principles

### Clear Responsibility

Each agent should have a bounded objective and explicit non-goals. Avoid broad descriptions that overlap with every other agent.

### Controlled Tool Use

Expose only the tools required for the task. Validate arguments, restrict permissions, and define how failures are handled.

### Deliberate Memory

Store information only when it improves future task performance. Define retention, update, and retrieval behavior explicitly.

### Bounded Planning

Use clear task limits, step budgets, and stop conditions. Prevent uncontrolled loops and repeated tool calls.

### Human Oversight

Require confirmation for destructive, external, financial, or otherwise high-impact actions.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-ai-agents-architect-skill.git ~/.claude/skills/ai-agents-architect
```

## Usage

Invoke the skill for agent architecture work:

```text
/ai-agents-architect
```

Provide the agent's objective, tools, data sources, memory needs, action permissions, and expected operating environment.

## Recommended Design Workflow

1. Define the user problem and agent goal.
2. Separate deterministic logic from model-driven decisions.
3. Identify required tools and data access.
4. Define agent state and memory boundaries.
5. Choose a planning or execution loop.
6. Set budgets, timeouts, and stop conditions.
7. Add approval gates for risky actions.
8. Design logs and evaluation metrics.
9. Test realistic and adversarial scenarios.
10. Expand autonomy only after reliability is demonstrated.

## Evaluation Checklist

- Agent goal is measurable.
- Tool contracts are narrow and validated.
- Memory has a clear purpose and retention policy.
- Plans have bounded steps and execution time.
- Errors are visible and recoverable.
- Permissions match the intended task.
- Human approval covers high-impact operations.
- Multi-agent coordination has explicit ownership.
- Evaluation includes task success and safety.

## Repository Contents

- `SKILL.md`: Main agent architecture instructions.
- `README.md`: Design principles, workflow, and evaluation checklist.

## Practical Principle

An agent that can do everything is difficult to control and test. Start with a constrained system that reliably completes one valuable task, then expand its capabilities based on evidence.


## Supporting Resources

| File | Purpose |
|---|---|
| [Agent architecture brief](resources/agent-architecture-brief.md) | Define goals, scope, tools, memory, control limits, and human oversight. |
| [Tool contract template](resources/tool-contract-template.md) | Specify schemas, authorization, side effects, retries, and failure behavior. |
| [Agent reliability evaluation](resources/agent-reliability-evaluation.md) | Evaluate task success, tool behavior, prompt injection, recovery, latency, and cost. |

## Third-party source and licensing

The upstream metadata in [SKILL.md](SKILL.md) identifies the skill source as vibeship-spawner-skills under Apache License 2.0. See [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md) and [licenses/Apache-2.0.txt](licenses/Apache-2.0.txt). The root MIT License applies to original repository material and does not replace the upstream license for the skill content.
