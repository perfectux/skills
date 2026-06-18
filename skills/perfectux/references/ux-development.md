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
- UI skill owns:
- Must not change:

## Fill Rules

- Keep each field to one concise line unless the workflow is complex.
- Infer from project context when safe.
- Ask only when missing context affects safety, payments, permissions, privacy, irreversible actions, or generated content.
- Treat missing loading, empty, error, disabled, success, permission, long-content, and mobile states as implementation work, not follow-up polish.
- Record visual ownership as a handoff, not an instruction.

## UI Skill Handoff

Give the active UI skill constraints, not taste directives:

- What the user must understand.
- What action must be easiest.
- Which states must exist.
- What feedback must appear.
- What recovery paths must be available.
- What cannot be hidden, delayed, or made decorative.

The UI skill owns how those constraints look.

## Conflict Handling

- UX wins only on task completion, safety, accessibility, feedback, state completeness, and recovery.
- UI wins on visual language, hierarchy expression, styling, motion feel, and brand tone.
- If a visual choice blocks a UX requirement, ask the UI skill to express the requirement differently rather than taking over visual direction.
