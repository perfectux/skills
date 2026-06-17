# Agentic Contract

Use this baseline contract for AI, automation, or tool-using flows.

- User intent:
- Agent capability:
- Tool/action risk:
- Data and memory scope:
- Visible states:
- Approval point:
- Commit point:
- Recovery path:
- User controls:
- Provenance needed:
- External tool disclosure:
- Saved or shared with:

## Fill Rules

- Keep each field short.
- Ask only when risk cannot be inferred.
- Treat irreversible writes, payments, permissions, privacy, security, memory, external sharing, and generated content used downstream as high-risk.
- For low-risk read-only flows, keep controls light but still show status and recovery.

## Required Distinctions

- User input: what the user asked for.
- Model output: what the AI produced.
- Tool activity: what external action is happening.
- Pending approval: what needs user review.
- Committed result: what has already changed.

## Data And Memory

- State what user content, files, credentials, or account data the agent can access.
- State whether anything will be saved for future use, sent to an external tool, published, shared, or reused downstream.
- Provide edit, revoke, delete, or disconnect controls when memory, integrations, credentials, or reusable user data are involved.
