# UX Writing

Make interface text help users understand, decide, act, and recover. Own labels, button text, helper text, empty states, loading text, error messages, success messages, permission copy, confirmations, destructive-action copy, and AI uncertainty copy.

## Writing Rules

- Use the user's language, not implementation terms.
- Start action labels with specific verbs: `Save changes`, `Invite member`, `Retry payment`.
- Avoid vague buttons: `Submit`, `Continue`, `OK`, `Done` unless the context makes the result unmistakable.
- Say what happened, what it means, and what the user can do next.
- Keep helper text near the control it explains.
- Do not invent claims, metrics, social proof, policy, or guarantees.
- Match visible labels and accessible names.
- Preserve existing product terminology unless it blocks comprehension.

## Copy Contract

- User job:
- Decision or action:
- Risk:
- Required state:
- Existing product term:
- Copy intent:
- Must avoid:

## State Copy

Use these patterns as starting points. Adapt to the product voice and user job.

## Empty

Pattern: missing object + next action.

- `No projects yet. Create a project to start generating assets.`
- `No invoices match these filters. Clear filters to see all invoices.`

Avoid: marketing copy, blame, or filler.

## Loading

Pattern: current operation + safe expectation.

- `Saving changes...`
- `Generating draft... You can review it before publishing.`

Avoid: exact progress unless backed by real progress data.

## Error

Pattern: failure + data safety + recovery.

- `Payment failed. Your card was not charged. Try another payment method.`
- `We could not save changes. Your edits are still here. Retry saving.`

Avoid: error codes as the main message unless developer-facing.

## Success

Pattern: completed change + useful next step.

- `Invite sent. You can change this member's role after they join.`
- `Changes saved. View the updated page.`

Avoid: celebratory copy that hides the next action.

## Permission

Pattern: required access + who can help.

- `You need admin access to invite members. Ask an admin to update your role.`
- `Connect billing to publish this plan.`

Avoid: dead ends.

## Confirmation

Pattern: object + consequence + reversibility + final action.

- `Delete "Q2 Launch Plan"? This cannot be undone. Delete plan.`
- `Publish this page? Customers will see the new version immediately. Publish page.`

Avoid: generic `Are you sure?`.

## AI Uncertainty

Pattern: assumption or missing input + user control.

- `Draft based on the files currently selected. Add more sources for a broader answer.`
- `The model could not verify pricing. Review before sending.`

Avoid: presenting generated content as verified fact without support.
