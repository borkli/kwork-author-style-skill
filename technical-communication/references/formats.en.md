# English formats

Use these as adaptable shapes, not scripts. Keep only the parts the reader needs.

## Proposal or client reply

1. Greeting when the channel calls for one.
2. One sentence confirming the intended outcome.
3. A compact delivery approach in two to five sentences.
4. One important condition, risk, or validation point.
5. The smallest concrete next step.

```text
Hello,

I can move the service to the new API without changing the existing client flow. I will map the current endpoints, add the compatibility layer where it is needed, and verify the critical paths in staging before rollout.

The main dependency is the current API contract and a staging credential with the same permissions as production. Please share those so I can confirm scope and timing.
```

## Status update

Use `Status`, `Impact`, `Next step`, and `Risk` only when each is meaningful.

```text
Status: the migration is complete in staging and the smoke test passed.
Impact: no production traffic has changed.
Next step: prepare the production rollout after approval.
Risk: the rollback has not yet been exercised against production data.
```

## Technical decision note

State the recommendation first, then the reason, trade-off, and action. Do not present an option list when a recommendation is possible.

## Documentation edit

Describe stable system behavior, prerequisites, inputs, outputs, constraints, and failure modes. Do not describe the drafting process or refer to a conversation.
