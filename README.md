# PerfectUX Skills

Reusable agent skills maintained by PerfectUX.

All skills use the `perfectux-` prefix so the maintainer is clear. The name after
the prefix distinguishes general-purpose skills from PerfectUX.ai product-specific
skills.

## General-Purpose Skills

These skills can be used in any product or codebase. They do not assume access to
PerfectUX.ai projects, schemas, routes, or MCP tools.

- `perfectux-ux-development`: UX guardrails for agentic development. It keeps
  user tasks, flows, states, feedback, accessibility, and recovery clear while
  leaving visual style to any active UI skill.

## Pairing With UI Skills

Use `perfectux-ux-development` with any visual, taste, or UI quality skill. The
UX skill defines the contract; the UI skill decides how it looks.

Examples:

- `Use $perfectux-ux-development with $taste-skill to build this onboarding flow.`
- `Use $perfectux-ux-development with $ui-ux-pro-max-skill to redesign this dashboard.`
- `Use $perfectux-ux-development with $impeccable-skill to polish this settings page.`

Division of labor:

- UX skill owns: user job, primary action, flow order, required states, feedback,
  accessibility, error recovery, permissions, AI/tool approvals, and QA checks.
- UI skill owns: palette, typography, spacing style, visual density, animation
  style, illustration, brand mood, and final aesthetic expression.
- If there is tension, UX only overrides when task completion, safety,
  accessibility, readability, feedback, or recovery would be harmed.

## PerfectUX.ai Product Skills

These skills are specific to the PerfectUX.ai product, codebase, schemas, MCP
tools, or project workflows. Use the `perfectux-app-` namespace for these.

Planned candidates:

- `perfectux-app-task-schemas`: canonical task schema and modify tool rules.
- `perfectux-app-mcp-workflows`: PerfectUX MCP setup and usage guidance.
- `perfectux-app-workspaces`: Foundation, launch, marketing, and trust-doc workflows.

Remote:

- `https://github.com/PerfectUX/skills.git`
