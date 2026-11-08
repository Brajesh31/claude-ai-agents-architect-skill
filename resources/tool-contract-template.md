# Agent Tool Contract Template

## Tool identity
- Name:
- Purpose:
- Owning service:
- Human owner:

## Contract
- Input schema:
- Required fields:
- Optional fields:
- Output schema:
- Error schema:
- Timeout:
- Rate limit:

## Security and execution
- Authentication mechanism:
- Authorization rules:
- Resource scope:
- Read-only or side-effecting:
- Confirmation required before execution:
- Idempotency strategy:
- Data that must be redacted:

## Failure behavior
| Failure | Retry? | Safe fallback | User-visible message |
|---|---|---|---|
| Invalid input | No | Ask for correction | |
| Permission denied | No | Stop and request authorization | |
| Timeout | Limited | Check operation status before retry | |
| Provider error | Bounded | Surface failure and preserve context | |

## Verification
- [ ] Inputs are validated server-side.
- [ ] Permissions follow least privilege.
- [ ] Side effects are explicit.
- [ ] Retries cannot create duplicate actions.
- [ ] Errors are typed and observable.
- [ ] Tests cover valid, invalid, and adversarial inputs.
