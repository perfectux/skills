# UX Review Rubric

Use this for audits, redesigns, and final QA. Score mentally by risk and user impact; do not output a mechanical score unless the user asks.

## Intent And Task Fit

- Is the primary user job clear within five seconds?
- Is there exactly one primary action per decision moment?
- Are secondary actions visually subordinate?
- Does the page answer "what is this, why should I care, what happens next"?

## Project Context Fit

- Does the UX match the product category, audience, and risk level?
- Does it reuse existing navigation, component patterns, design tokens, and copy voice?
- Does it account for real data states: loading, empty, error, permissions, latency, long content, and mobile?
- Are industry standards translated into concrete product decisions instead of applied generically?
- Are assumptions stated when the project context is incomplete?

## Information Architecture

- Are navigation labels stable, plain, and mutually exclusive?
- Are related items grouped by user intent rather than internal ownership?
- Can users recover from deep links, empty states, and missing permissions?
- Does each section have a clear job, or is it filler?

## Interaction Quality

- Are click targets large enough and spaced safely?
- Are hover, focus, active, disabled, loading, and success states defined?
- Can the workflow be completed with keyboard only?
- Are destructive actions confirmed with clear consequences?
- Are generated or AI outputs reviewable before irreversible use?
- Can users stop, retry, edit, undo, or recover from failed AI/tool actions?

## Accessibility

- Text and non-text contrast meet WCAG 2.2 AA targets.
- Focus order follows visual order.
- Focus is visible and not obscured by sticky headers or overlays.
- Controls have accessible names that match visible labels.
- Dynamic status updates are announced when needed.
- Motion respects reduced-motion preferences.
- Content works at common mobile widths and with text zoom.

## Content Quality

- Labels use user language, not implementation terms.
- Button text is short and action-specific.
- Error messages explain the problem and the next step.
- Empty states explain what can be done now.
- AI uncertainty, assumptions, sources, or missing inputs are explained when they affect user decisions.
- No fake metrics, fake proof, vague adjectives, or decorative metadata.

## Visual And Layout Quality

- Typography establishes hierarchy without oversized noise.
- Spacing supports scanning and grouping.
- Color carries meaning consistently.
- Cards, borders, and shadows communicate hierarchy rather than decoration.
- Real visual assets represent real product states or useful examples.
- Mobile composition is explicitly designed.

## Verification Evidence

For implementation work, verify with the strongest practical subset:

- Focused component or route tests.
- Typecheck or build.
- Desktop and mobile screenshots.
- Keyboard tab order and focus visibility checks.
- Reduced motion check when motion is present.
- Contrast check for critical text and buttons.
