# claude-ai-agents-architect-skill

A practical Claude Code skill for designing AI agents that are capable without becoming unpredictable or difficult to operate.

## Capabilities

- Agent goals, boundaries, and role design.
- Tool schemas, permissions, and side-effect controls.
- ReAct, plan-and-execute, and state-machine workflows.
- Memory selection and retention policies.
- Multi-agent orchestration and shared-state design.
- Reliability testing, observability, and safe recovery.

## Install

~~~bash
git clone https://github.com/Brajesh31/claude-ai-agents-architect-skill.git ~/.claude/skills/ai-agents-architect
~~~

## Use

~~~text
/ai-agents-architect
~~~

Describe the agent's goal, environment, available tools, data access, expected autonomy, and constraints. The skill will turn those details into an architecture and implementation plan.

## Design sequence

1. Define the user outcome and the agent's non-goals.
2. Select the simplest suitable execution pattern.
3. Specify tools and permission boundaries.
4. Design state and memory.
5. Add time, iteration, retry, and spend limits.
6. Plan for errors, hostile inputs, and partial outages.
7. Evaluate realistic cases before expanding autonomy.

## Supporting materials

| File | Purpose |
|---|---|
| [Agent architecture brief](resources/agent-architecture-brief.md) | Capture the goal, runtime, capabilities, state, and control model. |
| [Tool contract template](resources/tool-contract-template.md) | Define schemas, access, side effects, retry behavior, and errors. |
| [Agent reliability evaluation](resources/agent-reliability-evaluation.md) | Test quality, tool behavior, recovery, latency, and cost. |
| [Architecture decision record](resources/architecture-decision-record.md) | Compare design options and record the selected approach. |
| [Agent operations runbook](resources/agent-operations-runbook.md) | Define monitoring, pause, escalation, and recovery procedures. |

## Practical rule

A constrained agent that completes one valuable task consistently is a stronger starting point than a broad agent with unbounded permissions.

## License

MIT. See the root [LICENSE](LICENSE).