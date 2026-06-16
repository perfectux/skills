# AI Model Guidance

Use this file as model-facing instruction. The goal is to produce UX that fits the actual project while using industry standards as decision support.

## Mission

When designing, reviewing, or implementing UX, combine:

1. The local project context.
2. The user's stated goal.
3. Industry UX standards and heuristics.
4. The constraints of the existing codebase.

Do not produce generic "best practice" UI. Produce the version of the UX that is most appropriate for this product, route, audience, data model, and risk level.

## Context Model

Before changing UX, infer or inspect:

- Product category: marketing site, SaaS app, internal tool, developer tool, AI workspace, commerce flow, service journey, or content product.
- User and job: who is acting, what they are trying to finish, and what decision they need to make now.
- Risk level: low-risk browsing, reversible edit, irreversible publish, payment, permission, privacy, security, or AI-generated output.
- Primary action: the one action that should be easiest at this moment.
- Existing system: routes, navigation, components, design tokens, layout conventions, form patterns, copy voice, icon set, and motion style.
- Data reality: loading shape, empty state, error state, permissions, latency, long content, localization, and mobile constraints.
- Trust requirements: source visibility, audit trail, approval, undo, review, privacy, or explanation.

If a high-risk decision cannot be inferred from the project, ask one concise question. Otherwise state the assumption and continue.

## Standards Stack

Use standards selectively:

- WCAG 2.2 AA for baseline accessibility: perceivable, operable, understandable, robust.
- Nielsen Norman Group heuristics for general usability: status visibility, user control, consistency, error prevention, recognition over recall, efficient use, minimalist design, recovery, and help.
- ISO 9241-110:2020 for interaction quality: task fit, self-descriptive interaction, user control, expectation fit, learnability, error robustness, and engagement.
- GOV.UK Service Standard for end-to-end service flows: understand users, solve the whole problem, make the service simple, accessible, measurable, secure, and iterated.
- Microsoft Inclusive Design for exclusion awareness: design for real human diversity and make constraints explicit.
- Microsoft HAX and NIST AI RMF for AI-facing UX: set expectations, make AI behavior inspectable, support correction, manage uncertainty, and design for trustworthy use over time.
- The host product design system for final implementation details.

When standards conflict, resolve in this order:

1. User safety, privacy, accessibility, and legal obligations.
2. Successful completion of the user's current job.
3. Consistency with the host product.
4. Visual novelty or delight.

## Reasoning Protocol

For each material UX decision:

1. Name the user problem.
2. Name the project constraint.
3. Select only the relevant standard or heuristic.
4. Convert it into a concrete UI, copy, state, or interaction decision.
5. Verify that the decision still fits the existing product.

Good reasoning:

- "This is a destructive publish action, so the user needs a review step, clear consequences, and a recovery path."
- "This dashboard supports comparison, so a table is better than decorative cards for exact values."
- "This AI output will be used downstream, so sources, assumptions, editability, and approval state must be visible."

Poor reasoning:

- "Best practice says add cards."
- "Modern SaaS pages need gradients."
- "The UI needs more content to feel premium."

## Implementation Protocol

- Preserve existing navigation, component APIs, state management, and test patterns unless they are part of the UX problem.
- Keep one primary action per decision moment.
- Design complete states: default, loading, empty, error, disabled, success, permission-denied, long-content, and mobile.
- Write semantic HTML and accessible names that match visible labels.
- Keep copy short, concrete, and action-specific.
- Use motion only to clarify hierarchy, feedback, continuity, or state change; respect reduced motion.
- Do not invent fake product data, fake metrics, fake social proof, or fake screenshots.
- Prefer a small, well-verified UX improvement over a broad visual rewrite.

## AI And Agentic UI Protocol

For AI, chat, generation, or tool-using interfaces:

- During first use, explain what the AI can do, what it cannot reliably do, and what user input improves the result.
- During use, distinguish user input, model output, system state, tool calls, pending approvals, and completed actions.
- When the AI is uncertain, show assumptions, sources, confidence signals, or missing inputs as appropriate for the audience.
- Before irreversible actions, provide review, confirmation, and inspectable changes.
- When the AI is wrong, provide retry, edit, undo, report, and recovery paths.
- Over time, make history, provenance, preferences, and learned context understandable and controllable.
- For developer-facing products, raw logs or structured details may be available behind inspection. For end-user products, summarize in plain language.

## Output Template

When responding to a UX task, structure the answer internally around:

- Context read: what project facts matter.
- Relevant standards: which standards were selected and why.
- UX decisions: what will change and how it helps the user.
- Implementation notes: files, components, states, and constraints.
- Verification: tests, typecheck, screenshots, keyboard checks, and remaining risk.

Do not output this template mechanically if the user needs only a short answer. Use it to guide the work.

## Hard Stops

Do not proceed as if UX is complete when:

- The page cannot be used with keyboard for its primary task.
- Critical text or controls fail accessible contrast.
- Loading, empty, error, or permission states are missing from a user-facing workflow.
- AI-generated output can be committed irreversibly without review.
- The design contradicts the host product's core navigation, terminology, or visual system without an explicit redesign request.
- The implementation relies on fake data or a fake screenshot to prove quality.
