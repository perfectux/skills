---
name: perfectux
description: PerfectUX is a standalone, non-invasive UX guidance layer for AI agents that works with any codebase and pairs with active UI skills or design systems. Use when an agent needs general UX, interface copy, product flow, state completeness, accessibility, error recovery, agentic interaction guidance, or approval-flow clarity; not for visual style.
---

# PerfectUX

## Purpose

Guide product work toward clear, usable, recoverable UX without owning visual style. This skill is standalone, general-purpose, and works in any codebase.

## Operating Loop

1. Read context first: user request, audience, screen/route/surface, existing components, data states, copy, navigation, and any active UI skill or design system.
2. For non-trivial work, draft a compact internal UX contract and load only the smallest relevant reference below.
3. When a UI skill is active, hand it only UX constraints: user job, action priority, required states, feedback, accessibility, and recovery.
   If no UI skill is active, apply those constraints through the product's existing visual system and avoid inventing a new style.
4. Implement or review the smallest change that improves completion, confidence, safety, or clarity.
5. Verify relevant checkpoints and report evidence, not taste claims.

## Boundary

Own:
- User job, primary action, secondary actions, flow order, information architecture, feedback, required states, copy intent, accessibility baseline, error recovery, permissions, AI/tool review points, and user-facing recovery copy.

Defer:
- Palette, typography, spacing style, illustration, animation style, visual density, brand mood, and overall aesthetic direction. Let the active UI skill, design system, or project conventions decide these.

Intervene in visual decisions only when they harm task completion, safety, accessibility, readability, focus order, or recovery.

## Guidance

- Ask one question only when missing context could create high-risk UX.
- State assumptions and continue for low-risk unknowns.
- Prefer project conventions over generic patterns.
- Prefer complete states over extra content.
- Prefer reversible actions over warnings.
- Prefer plain action copy over decorative labels.

## References

- Use `references/ux-contract.md` for flow, IA, states, accessibility, recovery, UX contracts, and UI-skill handoff.
- Use `references/ux-writing.md` for labels, state copy, errors, confirmations, permissions, and AI uncertainty copy.
- Use `references/copy-checks.md` when interface copy changed.
- Use `references/agentic-interaction.md` for AI and tool-using flows.
- Use `references/agentic-checks.md` when agentic interaction changed.
- Use `references/checks.md` for QA before final response.
- Use `references/external-grounding.md` only when a UX decision needs external grounding for accessibility compliance, platform expectations, public-service constraints, or AI-risk framing; do not load it for ordinary UX work.
