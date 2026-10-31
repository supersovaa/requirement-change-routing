# requirement-change-routing

A lightweight skill for routing unsettled requirements and constraints to existing user-grilling workflows.

## When to use

Use it when creating or revising a requirement or constraint, or when another work phase would adopt a new guarantee.

Apply its rules **within the current work**, using the affected requirements and source checks already available. Before adopting an assistant-proposed new requirement or constraint, obtain the user's decision through the responsible grilling workflow. Distinguish code and test behavior from established requirements. Continue independent work while the dependent decision is settled.

This adds a routing rule rather than another approval stage, recurring scan, or tracking document.

## Responsibility and related skills

- [`SKILL.md`](SKILL.md) defines the routing behavior.
- [`grill-into-pr`](https://github.com/supersovaa/grill-into-pr) owns detailed questions and documentation-only design PRs when applicable.
- [`feature-introduction-threshold`](https://github.com/supersovaa/feature-introduction-threshold) owns the value and scope of functional choices.
- [`implemented-feature-change-handoff`](https://github.com/supersovaa/implemented-feature-change-handoff) owns the handoff from settled changes to implementation and test planning.

## Installation

Place `SKILL.md` at `<skills-root>/requirement-change-routing/SKILL.md`, or install this repository through the agent's skill-installation mechanism. Link it from the relevant work-type entries in the target repository's agent instructions.
