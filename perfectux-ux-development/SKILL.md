---
name: perfectux-ux-development
description: Use when Codex is building, changing, or reviewing user-facing flows and needs UX guidance for task fit, information architecture, state completeness, feedback, accessibility, error recovery, or AI/tool interactions. Use alongside any UI or visual-design skill; not for visual style.
---

# PerfectUX UX Development

## Purpose

Guide agentic development toward usable UX without owning visual style. This skill creates a compact UX contract that any UI, visual, or taste skill can render.

## Operating Loop

1. Read the project first: route, existing components, data states, copy, navigation, user request, and active UI skill.
2. Draft a compact UX contract. Keep it internal unless the user needs to see it.
3. Hand only UX constraints to UI skills: user job, action priority, required states, feedback, accessibility, and recovery.
4. Implement or review the smallest change that improves completion, confidence, safety, or clarity.
5. Verify UX checkpoints and report evidence, not taste claims.

## Boundary

Own:
- User job, primary action, secondary actions, flow order, information architecture, feedback, required states, copy intent, accessibility baseline, error recovery, permissions, and AI/tool review points.

Defer:
- Palette, typography, spacing style, illustration, animation style, visual density, brand mood, and overall aesthetic direction. Let the active UI skill decide these.

Intervene in visual decisions only when they harm task completion, safety, accessibility, readability, focus order, or recovery.

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

- Use `references/ux-contract.md` when coordinating with another UI skill.
- Use `references/checks.md` for QA before final response.
- Use `references/industry-anchors.md` only when a decision needs standards grounding.
