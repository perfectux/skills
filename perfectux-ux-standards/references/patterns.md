# Surface Patterns

Use these patterns selectively. The user's context and existing product system take precedence.

## Landing Or Handoff Pages

- Keep the page's job narrow: explain, route, or convert.
- Use one primary CTA. Avoid duplicate CTAs with the same intent.
- Keep hero copy short enough to fit the first viewport.
- Use a real product image only if it helps the decision. Do not force screenshots into repo handoff or docs pages.

## Product Workflows

- Show current step, saved state, and next action.
- Preserve user input across navigation, errors, and retries.
- Split complex tasks by decision, not by database model.
- Use review screens for irreversible writes, generated outputs, payment, publishing, and permission changes.

## Forms

- Put labels above fields.
- Never use placeholder text as the only label.
- Validate inline at the field and summarize when needed.
- Make optional versus required explicit only when it helps completion.
- Keep helper text close to the field it explains.

## Dashboards

- Start with the decision the dashboard supports.
- Separate status, trends, exceptions, and actions.
- Avoid decorative charts. Every visualization needs a comparison or decision.
- Use tables when exact comparison matters; use cards only for scan summaries.

## AI And Agentic UI

- Distinguish user input, model output, system state, and tool execution.
- Show uncertainty, sources, assumptions, and pending approvals when relevant.
- Make agent actions inspectable before committed writes.
- Provide stop, retry, undo, and edit paths.
- Avoid exposing raw tool JSON to end users unless they are developers and asked for it.

## Empty, Loading, And Error States

- Empty state: say what is missing and how to create or connect it.
- Loading state: reserve final layout space and show meaningful progress when possible.
- Error state: say what failed, whether data is safe, and what to do next.
- Permission state: explain what access is needed and who can grant it.
