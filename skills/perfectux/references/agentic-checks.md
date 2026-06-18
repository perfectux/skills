# Agentic Interaction Checks

Use before final response when AI or tool-using interaction changed.

## State Visibility

- Users can tell whether the agent is thinking, calling tools, waiting for approval, done, failed, or stopped.
- Long-running work shows whether it is safe to leave.
- Completed actions are distinguishable from proposed actions.

## Control

- Users can stop or pause work when the action is still pending.
- Users can edit input or retry output without losing context.
- Users can undo or recover from reversible writes.
- High-risk writes require review before commit.

## Trust

- Assumptions, missing inputs, sources, or uncertainty are visible when they affect decisions.
- Provenance is shown for generated content that will be reused, published, sent, or saved.
- Memory and data use is visible when content will be saved, reused, shared, or sent to external tools.
- Users can edit, revoke, delete, or disconnect saved memory, credentials, integrations, or reusable user data where relevant.
- Raw logs or tool JSON are hidden from end users unless requested in a developer-facing surface.

## Failure

- Failed tool actions say what failed and whether user data changed.
- Recovery paths are specific: retry, reconnect, edit input, restore, or contact an owner.
- The UI does not leave users unsure whether an action happened.
