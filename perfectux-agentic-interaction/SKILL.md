---
name: perfectux-agentic-interaction
description: Use when an AI agent is designing, building, or reviewing AI, chat, generation, automation, tool-calling, approval, memory, provenance, or human-in-the-loop workflows. MVP guardrails for inspectable, controllable, and recoverable agentic interactions; not for model architecture or visual style.
---

# PerfectUX Agentic Interaction

## Purpose

Make AI and tool-using flows understandable, controllable, and recoverable. This MVP skill defines interaction guardrails, not model behavior, prompt engineering, or visual design.

## Operating Loop

1. Map the agentic path: user input, model reasoning/output, tool activity, review point, commit point, and recovery path.
2. Classify risk: read-only, reversible write, irreversible write, payment, permission, privacy, security, or generated content used downstream.
3. Expose the minimum state users need to understand what is happening and what they can control.
4. Verify that users can stop, inspect, approve, retry, edit, undo, or recover where relevant.

## Boundary

Own:
- Agent state, tool activity, approval points, uncertainty, provenance, memory visibility, user controls, recovery, and irreversible-action safeguards.

Defer:
- Model selection, prompt internals, backend orchestration, visual style, animation style, and raw developer logs unless the surface is developer-facing.

## MVP Contract

Use this internally for AI or tool-using flows:

- User intent:
- Agent capability:
- Tool/action risk:
- Visible states:
- Approval point:
- Commit point:
- Recovery path:
- User controls:
- Provenance needed:

## Guardrails

- Distinguish user input, model output, tool activity, pending approval, and committed result.
- Do not hide irreversible writes behind automatic agent action.
- Show uncertainty, assumptions, sources, or missing inputs when they affect decisions.
- Provide stop, retry, edit, undo, or recover paths based on risk.
- For long-running work, show status and whether the user can safely leave.
- Hide raw tool JSON from end users unless the product is developer-facing and the user asked for it.

## References

- Use `references/agentic-contract.md` for the MVP interaction contract.
- Use `references/checks.md` for review and QA.
