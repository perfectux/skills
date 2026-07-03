# UX Contract

Use a UX contract to coordinate agentic development. It should be short, mostly internal, and safe to hand to any UI skill.

## Template

- User job:
- Primary action:
- Secondary actions:
- Risk level:
- Required states:
- Feedback and recovery:
- Accessibility baseline:
- AI/tool approvals, if any:
- UI skill/design system owns:
- Must not change:

## Fill Rules

- Keep each field to one concise line unless the workflow is complex.
- Infer from project context when safe.
- Ask only when missing context affects safety, payments, permissions, privacy, irreversible actions, or generated content.
- Treat missing loading, empty, error, disabled, success, permission, long-content, and mobile states as implementation work, not follow-up polish.
- Record visual ownership as a handoff, not an instruction.

## Visual Handoff

Give the active UI skill, design system, or existing project conventions constraints, not taste directives:

- What the user must understand.
- What action must be easiest.
- Which states must exist.
- What feedback must appear.
- What recovery paths must be available.
- What cannot be hidden, delayed, or made decorative.
- Which primary content or action area must keep its current container alignment, readable width, and task priority when helper panels or state messages are added.

The UI skill or existing visual system owns how those constraints look. If no UI skill is active, preserve the product's current visual language while implementing the UX requirements.

## Conflict Handling

- UX wins only on task completion, safety, accessibility, feedback, state completeness, and recovery.
- UI/design-system conventions win on visual language, hierarchy expression, styling, motion feel, and brand tone.
- If a visual choice blocks a UX requirement, express the requirement within the current visual system rather than taking over visual direction.
