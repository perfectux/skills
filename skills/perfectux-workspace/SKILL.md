---
name: perfectux-workspace
description: Use when an AI agent is working with PerfectUX.ai projects, workspace data, MCP resources, canonical task artifacts, launch packages, marketing campaigns, docs, exports, or schema-driven modify tools. Requires or benefits from PerfectUX MCP; not for general UX guidance outside PerfectUX.ai.
---

# PerfectUX Workspace

## Purpose

Work safely with PerfectUX.ai workspace context, project artifacts, and MCP tools. This skill is app-specific: use it only for PerfectUX.ai projects, assets, exports, or MCP-backed workflows.

## Operating Loop

1. Detect PerfectUX context:
   - Prefer an available `perfectux` MCP server, `perfectux://` resources, or PerfectUX MCP tools.
   - If MCP is unavailable, continue from repository or user-provided context and mention MCP only when it would materially improve the result.
2. Read before writing:
   - List or read project resources before proposing changes.
   - Prefer `DESIGN.md` export or Foundation JSON when implementation needs product context.
3. Classify intent:
   - Read/review context.
   - Improve UX or copy.
   - Modify canonical task artifacts.
   - Update launch, marketing, docs, or export-adjacent workspace assets.
4. Use schema-driven tools only for writes, and respect approval boundaries.
5. Keep user-facing output friendly; never expose raw MCP JSON unless the surface is developer-facing and requested.

## Boundaries

Own:
- PerfectUX project context, MCP resource selection, task artifact semantics, schema-driven modify tool usage, approval boundaries, user-facing summaries, and recovery from MCP/tool failures.

Defer:
- PerfectUX backend architecture, model selection, prompt internals, billing policy, and visual style unless the user asks.

Use `perfectux` instead for general UX, copy, accessibility, state completeness, or agentic interaction work that does not depend on PerfectUX.ai workspace context.

## Workspace Contract

- Project or workspace:
- User intent:
- Source of truth:
- Artifact type:
- Read resources:
- Proposed write, if any:
- Approval point:
- Recovery path:
- Must not change:

## MCP Rules

- Use existing PerfectUX MCP configuration without asking the user to reconnect.
- Do not invent project IDs, task IDs, asset IDs, permissions, or generated outputs.
- If the user did not identify a project and multiple projects are available, ask one concise selection question.
- Prefer read resources over asking the user to paste context.
- Treat tool permission errors as recoverable: explain the missing permission and the smallest next action.

## Write Rules

- Use canonical task schemas and schema-driven `modify_*_task` tools only.
- Do not reintroduce `modify_task_proposal`.
- Do not use legacy public fields such as `colorPalette`, `neutralLight`, `result.*`, or public `newResult` inputs.
- Let proposal review and approval happen through the tool approval flow.
- Do not directly overwrite task artifacts from prose when a modify tool exists.
- Use idempotency keys when action tools require them.

## References

- Use `references/mcp-workflow.md` for resource and tool routing.
- Use `references/project-context.md` to decide which PerfectUX artifact to read.
- Use `references/task-modification-tools.md` before modifying canonical task artifacts.
- Use `references/approval-boundaries.md` before any write or high-risk action.
- Use `references/checks.md` before final response.
