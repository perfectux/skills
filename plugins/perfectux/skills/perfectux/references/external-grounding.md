# External Grounding

Use only when a UX decision needs external grounding. Default to product context, project conventions, and the active UI skill.

Links are canonical starting points, not bundled standards text. Do not browse or cite them by default. If the answer depends on a version-specific detail, a high-risk claim, or a source citation, verify the current official source first.

## Route

- Accessibility baseline or legal accessibility rationale: start with [WCAG 2.2](https://www.w3.org/TR/WCAG22/); use [WAI-ARIA APG](https://www.w3.org/WAI/ARIA/apg/) only for web widget semantics and keyboard behavior.
- Neutral human-system interaction rationale: use [ISO 9241-110:2020](https://www.iso.org/standard/75258.html) when the decision needs a standard rather than taste.
- AI trust, safety, transparency, privacy, or security risk: start with [NIST AI RMF and current profiles](https://www.nist.gov/itl/ai-risk-management-framework).
- Apple, Android/Google, or Microsoft ecosystem expectations: use [Apple HIG](https://developer.apple.com/design/human-interface-guidelines/), [Material Design](https://m3.material.io/), or [Fluent 2](https://fluent2.microsoft.design/) only for that platform or design system.
- Public-sector, high-trust, form-heavy, or whole-service flows: use [GOV.UK Service Standard](https://www.gov.uk/service-manual/service-standard) or [U.S. Web Design System](https://designsystem.digital.gov/) only when the product context fits.
- Human-AI interaction practice examples: use [Microsoft HAX Toolkit](https://www.microsoft.com/en-us/haxtoolkit/ai-guidelines/) as a practice lens, not a standard.

Apply the smallest relevant source as a constraint, then return to the product task. Prefer the product's design system unless it harms task completion, accessibility, feedback, or recovery.
