# UX Checks

Use these checks before final response. Do not output a score unless the user asks.

## Task Fit

- Is the user job clear?
- Is the primary action obvious at the decision moment?
- Are secondary actions clearly lower priority?
- Does the flow make the next step, consequence, and success state clear?

## Project Context Fit

- Does the UX match the product category, audience, and risk level?
- Does it reuse existing navigation, component patterns, state patterns, and copy voice?
- Are assumptions stated when the project context is incomplete?

## State Completeness

- Default, loading, empty, error, disabled, success, permission, long-content, and mobile states are handled where relevant.
- Async work shows status and does not lose user input.
- Errors explain what failed, whether user data is safe, and what to do next.
- Destructive or irreversible actions have review, confirmation, or recovery.

## Interaction

- Controls have clear labels and predictable outcomes.
- Keyboard use can complete the primary task.
- Focus order follows the task order.
- Touch/click targets are usable and not crowded.
- Dynamic status updates are announced when needed.

## AI And Tool Use

- User input, model output, tool activity, pending approval, and completed action are distinguishable.
- AI uncertainty, assumptions, sources, or missing inputs are visible when they affect decisions.
- Users can stop, retry, edit, undo, or recover from failed AI/tool actions.
- Raw tool JSON is hidden unless the surface is developer-facing and requested.

## Visual Skill Boundary

- Do not critique palette, typography taste, illustration style, or motion personality.
- Do flag visual choices that break readability, contrast, focus, task priority, control affordance, or state recognition.
- Let the UI skill choose the visual expression for each UX requirement.

## Verification Evidence

For implementation work, verify with the strongest practical subset:

- Focused component or route tests.
- Typecheck or build.
- Desktop and mobile screenshots.
- Keyboard tab order and focus visibility checks.
- Screen-reader labels and dynamic status checks where relevant.
- Contrast check only for critical readability and controls.
