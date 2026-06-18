# Agentic Interaction

Make AI and tool-using flows understandable, controllable, and recoverable. Own agent state, tool activity, approval points, uncertainty, provenance, memory and data visibility, user controls, recovery, and irreversible-action safeguards.

## Operating Loop

1. Map the agentic path: user input, model reasoning/output, tool activity, data or memory use, review point, commit point, and recovery path.
2. Classify risk: read-only, reversible write, irreversible write, payment, permission, privacy, security, memory, external sharing, or generated content used downstream.
3. Expose the minimum state users need to understand what is happening and what they can control.
4. Verify that users can stop, inspect, approve, retry, edit, undo, or recover where relevant.

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

## Guardrails

- Distinguish user input, model output, tool activity, pending approval, and committed result.
- Do not hide irreversible writes behind automatic agent action.
- Show uncertainty, assumptions, sources, or missing inputs when they affect decisions.
- Make memory and data use explicit when content will be saved, reused, shared, or sent to external tools.
- Provide stop, retry, edit, undo, or recover paths based on risk.
- Provide edit, revoke, delete, or disconnect controls for saved memory, credentials, integrations, or reusable user data.
- For long-running work, show status and whether the user can safely leave.
- Hide raw tool JSON from end users unless the product is developer-facing and the user asked for it.
