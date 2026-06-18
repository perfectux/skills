# PerfectUX Skills

Reusable agent skills maintained by PerfectUX.

This repository ships two public skills:

- `perfectux`: general UX, interface copy, product flow, accessibility,
  recovery, and agentic interaction guidance. It does not require the
  PerfectUX.ai app or MCP.
- `perfectux-workspace`: PerfectUX.ai workspace, MCP, project artifact, export,
  and schema-driven modification workflows.

It also includes a Codex plugin at `plugins/perfectux` that bundles both skills.

## Install

List available skills:

```bash
npx skills add PerfectUX/skills --list
```

Install the general UX skill:

```bash
npx skills add PerfectUX/skills --skill perfectux --agent codex --global
```

Install the PerfectUX.ai workspace skill:

```bash
npx skills add PerfectUX/skills --skill perfectux-workspace --agent codex --global
```

For Claude Code, use `--agent claude-code`; for other agents, replace `codex`
with the agent key supported by the `skills` CLI.

## Codex Plugin

Codex users can install the `PerfectUX` plugin from `plugins/perfectux` when
they want both skills as one installable package. The plugin does not embed an
unauthenticated MCP server config; `perfectux-workspace` automatically uses an
already configured `perfectux` MCP server when available.

## Skill Split

### `perfectux`

Use for any product or codebase. It does not assume access to PerfectUX.ai
projects, schemas, routes, or MCP tools.

Examples:

- `Use $perfectux with your active UI skill to build this onboarding flow.`
- `Use $perfectux to polish this AI approval flow.`

Division of labor:

- `perfectux` owns: user job, primary action, flow order, required states,
  feedback, accessibility, error recovery, permissions, AI/tool approvals,
  interface copy, and QA checks.
- UI skill owns: palette, typography, spacing style, visual density, animation
  style, illustration, brand mood, and final aesthetic expression.
- If there is tension, UX only overrides when task completion, safety,
  accessibility, readability, feedback, or recovery would be harmed.

### `perfectux-workspace`

Use for PerfectUX.ai projects, workspace data, MCP resources, canonical task
artifacts, launch packages, marketing campaigns, docs, exports, and
schema-driven modify tools. It treats PerfectUX MCP as an optional source of
truth: when MCP is available, it reads resources directly; when unavailable, it
continues from repo or user-provided context.

Remote:

- `https://github.com/PerfectUX/skills.git`
