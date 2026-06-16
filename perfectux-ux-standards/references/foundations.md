# UX Foundations

Use these as grounding principles. Do not quote them at length in user-facing output. Standards are inputs to project-specific decisions, not a substitute for reading the product.

## Source-Backed Standards

- W3C WCAG 2.2: use perceivable, operable, understandable, and robust as accessibility foundations. Default to AA for product work unless the project requires a stricter target.
- Nielsen Norman Group usability heuristics: use status visibility, real-world language, user control, consistency, error prevention, recognition over recall, efficiency, minimalist design, error recovery, and help as broad critique lenses.
- ISO 9241-110:2020: use task suitability, self-descriptive interaction, expectation fit, learnability, controllability, error robustness, and user engagement as interaction quality checks.
- GOV.UK Service Standard and Design System: use user-needs research, whole-service thinking, simple flows, accessible implementation, measurable outcomes, privacy/security, and iteration for service journeys.
- Microsoft Inclusive Design: recognize exclusion, learn from human diversity, and solve specific constraints in ways that can extend to more users.
- Microsoft HAX Toolkit: use human-AI interaction guidance for expectation setting, feedback, correction, uncertainty, and long-term user control in AI products.
- NIST AI Risk Management Framework: use governance, mapping, measurement, and management of AI risks when UX affects trust, safety, privacy, security, or downstream decisions.
- Apple Human Interface Guidelines: prefer clarity, deference to content, direct manipulation, feedback, consistency, and forgiving interactions when building Apple-platform experiences.
- Material Design 3: use foundations for layout, color, type, motion, and interaction conventions when a Material-like system is present.

Reference URLs:
- https://www.w3.org/TR/WCAG22/
- https://www.nngroup.com/articles/ten-usability-heuristics/
- https://www.iso.org/standard/75258.html
- https://www.gov.uk/service-manual/service-standard
- https://design-system.service.gov.uk/
- https://inclusive.microsoft.design/
- https://www.microsoft.com/en-us/haxtoolkit/
- https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/
- https://airc.nist.gov/airmf-resources/airmf/
- https://developer.apple.com/design/human-interface-guidelines/
- https://m3.material.io/foundations

## Core Principles

1. User goal clarity: the page must make the next useful action obvious.
2. Information hierarchy: primary content, primary action, secondary action, and support content must be visually distinct.
3. Cognitive load control: remove choices, labels, and visual elements that do not help the current decision.
4. Feedback and status: every async action, navigation, save, upload, generation, and destructive action needs clear state.
5. Error prevention and recovery: prevent avoidable errors, then provide plain-language recovery when errors happen.
6. Accessibility: keyboard, screen reader semantics, contrast, target size, focus visibility, motion preferences, and text resizing must be designed in.
7. Content design: use concrete verbs, user-language labels, scannable text, and consistent terms.
8. Trust: pricing, permissions, privacy, generated content, irreversible actions, and AI uncertainty must be explicit.
9. Responsiveness: mobile must be intentionally composed, not merely stacked.
10. Performance perception: reserve space, avoid layout shift, show meaningful loading states, and keep interaction latency low.
11. Project fit: reuse the host product's language, interaction model, design system, and risk posture before adding new patterns.
12. AI accountability: make model output, sources, assumptions, tool activity, approvals, and recovery paths visible at the right level of detail.
