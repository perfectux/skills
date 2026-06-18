# Approval Boundaries

PerfectUX workspace actions can affect saved project artifacts. Keep the review point visible.

## Read-Only

- Reading projects, tasks, exports, launch packages, marketing campaigns, or docs is low risk.
- Still state source and freshness when it affects a decision.

## Writes

- Canonical task modifications require schema-driven tools and approval flow.
- Approval flow means the client/tool approval UI or the public MCP preview plus `confirmationToken`, not an extra chat confirmation stacked on top.
- Launch, marketing, and docs updates require a clear object, consequence, and recovery path.
- Use idempotency keys when required by the tool.

## High Risk

Pause or ask one concise question when:

- The target project or artifact is ambiguous.
- The write may overwrite user work.
- The user lacks required MCP permission.
- The action affects published, sent, or externally reused content.

## Recovery

- Permission failure: name the missing permission and smallest fix.
- Validation failure: summarize the invalid field and expected shape.
- Tool failure: say whether any data changed and offer retry or edit path.
