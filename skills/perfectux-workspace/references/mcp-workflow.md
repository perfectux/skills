# MCP Workflow

Use PerfectUX MCP as the source of truth when available.

## Detection

- Look for a configured MCP server named `perfectux`.
- Look for resources with `perfectux://` URIs.
- Look for PerfectUX tools such as schema-driven task modification tools or workspace update tools.

Do not ask the user to reconnect when PerfectUX MCP tools or resources are already available.

## Read Order

1. List projects when the user has not named or scoped a project.
2. Read compact project metadata.
3. Read task artifacts, launch package, marketing campaigns, docs, or exports based on the user intent.
4. Prefer `perfectux://projects/{projectId}/exports/design.md` for implementation handoff context.
5. Prefer `perfectux://projects/{projectId}/exports/foundation.json` when structured project data matters.

## Tool Use

- Read resources before proposing writes.
- Use write tools only when the user asks to change PerfectUX workspace artifacts.
- Treat permission failures as recoverable and state the missing permission.
- Keep raw MCP payloads out of user-facing responses unless requested for debugging.
