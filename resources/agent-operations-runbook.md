# Agent Operations Runbook

## Service details

- Agent or workflow:
- Environment:
- Technical owner:
- Operational owner:
- Criticality:
- Support hours:

## Health signals

| Signal | Expected range | Alert threshold | Response owner |
|---|---|---|---|
| Task success rate | | | |
| Tool error rate | | | |
| Median / p95 latency | | | |
| Cost per successful task | | | |
| Queue age | | | |
| Repeated side effects | | | |

## Normal operations

1. Check service health and recent error trends.
2. Review failed tasks and sanitized tool traces.
3. Confirm model, prompt, and tool versions.
4. Compare spend and latency with the approved limits.
5. Record incidents and follow-up actions.

## Pause procedure

- Disable new task intake.
- Allow safe read-only work to finish when appropriate.
- Stop pending side-effecting actions.
- Preserve execution identifiers and sanitized diagnostics.
- Notify the responsible operator.

## Recovery procedure

1. Identify the failure category.
2. Confirm whether any external side effect already completed.
3. Prevent duplicate execution.
4. Restore dependencies or revert the faulty change.
5. Run a narrow verification test.
6. Resume gradually after approval.

## Incident record

- Incident ID:
- Start and end time:
- User impact:
- Trigger:
- Affected tools:
- Actions already completed:
- Recovery steps:
- Follow-up owner:
- Preventive change:

## Release gate

- [ ] Permission changes reviewed.
- [ ] Regression suite passed.
- [ ] Recovery path tested.
- [ ] Monitoring and alerts are active.
- [ ] Rollback owner is available.
- [ ] Production approval recorded.