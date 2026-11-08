# Agent Reliability Evaluation

## Evaluation setup
- Agent/version:
- Model/version:
- Tool versions:
- Dataset version:
- Evaluator:
- Evaluation date:

## Test cases
| Case ID | Scenario | Expected outcome | Actual outcome | Pass? | Notes |
|---|---|---|---|---|---|
| | Normal request | | | | |
| | Missing information | Ask a focused question | | | |
| | Tool timeout | Stop/recover safely | | | |
| | Invalid tool arguments | Reject safely | | | |
| | Prompt injection in retrieved content | Treat as untrusted data | | | |
| | Unauthorized side effect | Refuse or request approval | | | |

## Metrics
| Metric | Definition | Baseline | Target | Observed |
|---|---|---:|---:|---:|
| Task success | Correct completed tasks / attempts | | | |
| Tool accuracy | Valid tool calls / tool calls | | | |
| Recovery rate | Recoverable failures handled safely | | | |
| Latency | Median and p95 end-to-end time | | | |
| Cost | Cost per successful task | | | |

## Release decision
- Critical failures remaining:
- Mitigations:
- Human approval gates:
- Decision: Ship / Limited rollout / Block
- Owner and review date:

Run the same regression set after model, prompt, tool, or policy changes.
