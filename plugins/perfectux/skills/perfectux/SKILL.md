---
name: perfectux
description: Use when an AI agent needs general UX, interface copy, product flow, state completeness, accessibility, error recovery, or agentic interaction guidance. Does not require the PerfectUX.ai app, workspace, or MCP connection; not for visual style.
---

# PerfectUX

## Purpose

Guide product work toward clear, usable, recoverable UX without owning visual style. This skill is general-purpose and does not assume access to PerfectUX.ai, workspace data, schemas, routes, or MCP tools.

## Operating Loop

1. Read context first: user request, audience, route/screen, existing components, data states, copy, navigation, and active UI skill.
2. Draft a compact internal UX contract for non-trivial work.
3. Route the work:
   - Flow, IA, states, accessibility, and recovery: use `references/ux-development.md`.
   - Labels, state copy, errors, confirmations, permissions, or AI uncertainty copy: use `references/ux-writing.md`.
   - AI, chat, generation, automation, tool-calling, approval, memory, provenance, privacy, or security flows: use `references/agentic-interaction.md`.
4. Hand only UX constraints to UI skills: user job, action priority, required states, feedback, accessibility, and recovery.
5. Implement or review the smallest change that improves completion, confidence, safety, or clarity.
6. Verify relevant checkpoints and report evidence, not taste claims.

## Boundary

Own:
- User job, primary action, secondary actions, flow order, information architecture, feedback, required states, copy intent, accessibility baseline, error recovery, permissions, AI/tool review points, and user-facing recovery copy.

Defer:
- Palette, typography, spacing style, illustration, animation style, visual density, brand mood, and overall aesthetic direction. Let the active UI skill decide these.

Intervene in visual decisions only when they harm task completion, safety, accessibility, readability, focus order, or recovery.

Use `perfectux-workspace` instead when the task depends on PerfectUX.ai projects, workspace data, MCP resources, canonical task artifacts, launch packages, marketing campaigns, docs, exports, or schema-driven modify tools.

## UX Contract

Use this short shape before non-trivial work:

- User job:
- Primary action:
- Secondary actions:
- Risk level:
- Required states:
- Feedback and recovery:
- Accessibility baseline:
- AI/tool approvals, if any:
- UI skill owns:
- Must not change:

## Guidance

- Ask one question only when missing context could create high-risk UX.
- State assumptions and continue for low-risk unknowns.
- Prefer project conventions over generic patterns.
- Prefer complete states over extra content.
- Prefer reversible actions over warnings.
- Prefer plain action copy over decorative labels.
- Do not expose raw tool JSON unless the product is developer-facing and the user asked for it.

## References

- Use `references/ux-development.md` for the UX contract and UI-skill handoff.
- Use `references/ux-writing.md` for copy rules and state-copy patterns.
- Use `references/copy-checks.md` when interface copy changed.
- Use `references/agentic-interaction.md` for AI and tool-using flows.
- Use `references/agentic-checks.md` when agentic interaction changed.
- Use `references/checks.md` for QA before final response.
- Use `references/industry-anchors.md` only when a decision needs standards grounding.
