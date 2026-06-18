# Task Modification Tools

Use schema-driven `modify_*_task` tools for canonical task artifact edits.

## Rules

- Read the current task artifact first.
- Use the modify tool for the matching task type.
- Let tool approval handle proposal review.
- Do not add a separate prose confirmation when the client or MCP server already provides approval UI, preview, or `confirmationToken`.
- For public PerfectUX MCP, call the same `modify_*_task` tool twice: first for preview, then again with the returned `confirmationToken` after user approval.
- Keep inputs schema-shaped and minimal.
- Do not expose raw tool JSON to end users.

## Do Not Use

- `modify_task_proposal`
- Legacy public fields such as `colorPalette`, `neutralLight`, `result.*`, or public `newResult` inputs
- Freeform overwrites when a schema-driven modify tool exists

## User-Facing Summary

After a successful tool call, summarize:

- What changed.
- Which artifact changed.
- Whether the change is pending approval or already committed.
- What the user can do next.
