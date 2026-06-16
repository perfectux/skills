# UX Foundations

Use these as grounding principles. Do not quote them at length in user-facing output.

## Source-Backed Standards

- W3C WCAG 2.2: use perceivable, operable, understandable, and robust as accessibility foundations. Default to AA for product work.
- Nielsen Norman Group heuristics: use status visibility, real-world language, user control, consistency, error prevention, recognition over recall, efficiency, minimalist design, error recovery, and help as critique lenses.
- Apple Human Interface Guidelines: prefer clarity, deference to content, direct manipulation, feedback, consistency, and forgiving interactions when relevant.
- Material Design 3: use foundations for layout, color, type, motion, and interaction conventions when a Material-like system is present.
- GOV.UK Service Manual / Design System: use plain language, one thing per page, explicit error handling, and high accessibility expectations for service flows.

Reference URLs:
- https://www.w3.org/TR/WCAG22/
- https://www.nngroup.com/articles/ten-usability-heuristics/
- https://developer.apple.com/design/human-interface-guidelines/
- https://m3.material.io/foundations
- https://design-system.service.gov.uk/

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
