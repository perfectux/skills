---
name: perfectux-content-ux
description: Use when an AI agent is writing, rewriting, or reviewing interface copy for labels, buttons, forms, empty states, errors, confirmations, permissions, onboarding, or AI uncertainty. Use alongside UX and UI skills; not for brand naming, marketing copy, or visual style.
---

# PerfectUX Content UX

## Purpose

Make interface text help users understand, decide, act, and recover. This skill owns UX writing, not brand voice strategy or visual presentation.

## Operating Loop

1. Read the product context: user job, current screen, action risk, existing terms, and tone.
2. Draft a short copy contract for non-trivial work.
3. Rewrite only the text that affects understanding, action, feedback, or recovery.
4. Check state copy before final response.

## Boundary

Own:
- Labels, button text, helper text, empty states, loading text, error messages, success messages, permission copy, confirmations, destructive-action copy, and AI uncertainty copy.

Defer:
- Brand naming, marketing positioning, campaign copy, visual hierarchy, typography, layout, color, and animation.

Intervene in UI only when text placement or visibility harms comprehension, action, accessibility, or recovery.

## Copy Contract

Use this internally when copy affects a workflow:

- User job:
- Decision or action:
- Risk:
- Required state:
- Existing product term:
- Copy intent:
- Must avoid:

## Writing Rules

- Use the user's language, not implementation terms.
- Start action labels with specific verbs: `Save changes`, `Invite member`, `Retry payment`.
- Avoid vague buttons: `Submit`, `Continue`, `OK`, `Done` unless the context makes the result unmistakable.
- Say what happened, what it means, and what the user can do next.
- Keep helper text near the control it explains.
- Do not invent claims, metrics, social proof, policy, or guarantees.
- Match visible labels and accessible names.
- Preserve existing product terminology unless it blocks comprehension.

## State Copy

- Empty: what is missing and how to create or connect it.
- Loading: what is happening; use real progress only when available.
- Error: what failed, whether work is safe, and the next recovery action.
- Success: what changed and where the user can continue.
- Permission: what access is needed and who can grant it.
- Destructive confirmation: object, consequence, reversibility, and final action.
- AI uncertainty: assumptions, missing inputs, sources, or edit/retry paths when they affect a user decision.

## References

- Use `references/copy-checks.md` for review and QA.
- Use `references/state-copy.md` for state-specific copy patterns.
