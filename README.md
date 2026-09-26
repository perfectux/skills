<div align="center">
  <a href="https://perfectux.ai">
    <img src=".github/assets/perfectux-logo.png" alt="PerfectUX" width="160">
  </a>

  <h1>PerfectUX Skills</h1>

  <p>
    <strong>A non-invasive UX guidance layer for AI agents that works with any codebase<br>
    and pairs with your UI skill to improve flows, states, copy, accessibility, and recovery.</strong>
  </p>

  <p>
    Use <code>perfectux</code> in any product or codebase, or add <code>perfectux-workspace</code><br>
    when your agent should work with PerfectUX.ai workspace resources and schema-driven modifications.
  </p>
</div>

## Quick Start (Install)

Install the core UX skill:

```bash
npx skills add perfectux/skills --skill perfectux
```

This equips your agent with senior product UX judgment, interface copy, accessibility, error recovery, and agentic interaction guidance.

To list all available skills:
```bash
npx skills add perfectux/skills --list
```

---

## Core Skill: `perfectux`

Use for any product or codebase. It is standalone UX guidance that applies without setup.

### Example Prompts
- `"Use perfectux to improve this onboarding flow."`
- `"Use perfectux with your active UI skill to build this settings screen."`
- `"Use perfectux to polish this AI approval flow."`

*(Note: Depending on your agent client, you can invoke this via `Use perfectux`, `$perfectux`, or `/perfectux`)*

### Division of Labor
- **`perfectux` owns**: user job, primary action, flow order, required states, feedback, accessibility, error recovery, permissions, AI/tool approvals, interface copy, and QA checks.
- **Your UI skill, design system, or project conventions own**: palette, typography, spacing style, visual density, animation style, illustration, brand mood, and final aesthetic expression.

*If there is tension, UX only overrides when task completion, safety, accessibility, readability, feedback, or recovery would be harmed.*

---

## Optional: Workspace Integration

If you use the PerfectUX.ai app and want your agent to interact with workspace tasks, schemas, and MCP tools, install the workspace extension:

```bash
npx skills add perfectux/skills --skill perfectux-workspace
```

### `perfectux-workspace` (Extension Skill)

Use when the agent is working with PerfectUX.ai projects, workspace data, MCP resources, canonical task artifacts, launch packages, marketing campaigns, docs, exports, or schema-driven modify tools. It treats PerfectUX MCP as an optional source of truth: when MCP is available, it reads resources directly; when unavailable, it continues from repo or user-provided context.

---

## Plugins (Codex & Claude Code)

This repository also includes a multi-agent plugin at `plugins/perfectux` for **Codex** and **Claude Code**. It bundles both `perfectux` and `perfectux-workspace` as one installable package.

### Claude Code Installation

Within your Claude Code terminal session:

1. **Add the marketplace repository**:
   ```bash
   /plugin marketplace add perfectux/skills
   ```

2. **Install the plugin**:
   ```bash
   /plugin install perfectux@perfectux-skills
   ```

### Codex Installation

Within your Codex terminal session:

1. **Add the marketplace repository**:
   ```bash
   codex plugin marketplace add perfectux/skills
   ```

2. **Install the plugin**:
   ```bash
   codex plugin add perfectux@perfectux-skills
   ```

*(Alternatively, for local development, open your Codex application, go to **Settings** > **Plugins**, select **Load Local Plugin**, and point to the `plugins/perfectux` directory.)*

### Optional: MCP Workspace Configuration

If you want to use the workspace integration features (`perfectux-workspace` skill), configure the `perfectux` MCP server from [blueprint.perfectux.ai/mcp](https://blueprint.perfectux.ai/mcp).

- **Claude Code**: Follow the Claude Code setup guide at [blueprint.perfectux.ai/mcp](https://blueprint.perfectux.ai/mcp), or add the server through `/mcp add`.
- **Codex**: Follow the Codex setup guide at [blueprint.perfectux.ai/mcp](https://blueprint.perfectux.ai/mcp), then enable the PerfectUX MCP server in Codex MCP settings.

Remote:

- `https://github.com/perfectux/skills.git`
