# Agentic Contract

Use this MVP contract for AI, automation, or tool-using flows.

- User intent:
- Agent capability:
- Tool/action risk:
- Visible states:
- Approval point:
- Commit point:
- Recovery path:
- User controls:
- Provenance needed:

## Fill Rules

- Keep each field short.
- Ask only when risk cannot be inferred.
- Treat irreversible writes, payments, permissions, privacy, and generated content used downstream as high-risk.
- For low-risk read-only flows, keep controls light but still show status and recovery.

## Required Distinctions

- User input: what the user asked for.
- Model output: what the AI produced.
- Tool activity: what external action is happening.
- Pending approval: what needs user review.
- Committed result: what has already changed.
