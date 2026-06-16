---
name: perfectux-ux-standards
description: General-purpose UX standards workflow maintained by PerfectUX for AI-built web interfaces, product flows, landing pages, forms, dashboards, and agentic UI. Use when Codex needs to design, critique, rewrite, or verify UX using usability heuristics, accessibility, information architecture, interaction feedback, content clarity, responsive behavior, trust, and visual polish. This skill is not specific to the PerfectUX.ai product.
---

# PerfectUX UX Standards

## Overview

Use this general skill to make AI-generated interfaces more usable, credible, accessible, and production-ready. Treat it as a UX operating system, not a visual trend pack or a PerfectUX.ai product integration.

## Workflow

1. Identify the surface: landing page, product workflow, dashboard, form, settings, AI/chat UI, onboarding, empty/error state, or documentation.
2. Identify the user's job, primary action, decision context, and risk level. If these are unclear and the change is risky, ask one concise question.
3. Read the existing implementation, screenshots, copy, route behavior, and design tokens before proposing changes.
4. Choose the relevant references:
   - Use `references/foundations.md` for core UX principles and source-backed standards.
   - Use `references/review-rubric.md` for critique, redesign, or QA.
   - Use `references/patterns.md` for surface-specific patterns.
5. Make the smallest change that materially improves the user's outcome. Do not add decorative complexity unless it clarifies hierarchy, feedback, state, or trust.
6. Verify with evidence: focused tests, typecheck, browser screenshots for visual work, keyboard/focus checks where applicable, and mobile viewport review.

## Decision Rules

- Start with user success, not aesthetics. Every layout and interaction decision must make the user more confident, faster, safer, or better informed.
- Prefer established platform and product conventions over novelty for critical workflows.
- Preserve brand and product context unless the user asks for a visual reset.
- Design complete states: default, loading, empty, error, disabled, success, permission-denied, and long-content cases.
- Use motion only for hierarchy, feedback, continuity, or state change. Respect reduced motion.
- Treat accessibility as baseline quality. Use WCAG 2.2 AA as the default target unless the project explicitly requires a different standard.
- Avoid fake precision, fake social proof, decorative status labels, and product screenshots that do not represent a real state.

## Output Expectations

For a critique:
- Lead with the highest-impact issues.
- Tie each issue to user impact.
- Suggest concrete changes, not vague taste feedback.

For implementation:
- Follow the host app's design system, routing, data, and test patterns.
- Keep copy short, specific, and consistent with the page's job.
- Provide visual verification for frontend work where possible.

For final QA:
- Report what was verified and what remains unverified.
- Include exact commands or screenshots used as evidence.
