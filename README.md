# requirement-change-routing

A lightweight skill for distinguishing work governed by settled requirements and design from requirement or constraint choices that need user judgment.

## When to use

Use it when deciding whether to ask the user for a requirements/design decision during any kind of work, including creating or revising requirements or constraints and proposing new guarantees.

Apply it **within the current work**, reusing the relevant decisions, source checks, questions, documents, and PRs.

## Responsibility and related skills

- [`SKILL.md`](SKILL.md) owns the boundary between proceeding under the settled contract and routing remaining requirement or constraint decisions.
- The current work phase owns corrections, implementation choices, and review classification.
- [`grill-into-pr`](https://github.com/supersovaa/grill-into-pr) owns detailed questions and documentation-only design PRs when applicable.
- [`feature-introduction-threshold`](https://github.com/supersovaa/feature-introduction-threshold) owns the value and scope of functional choices.
- [`implemented-feature-change-handoff`](https://github.com/supersovaa/implemented-feature-change-handoff) owns the handoff from settled changes to implementation and test planning.

## Installation

Place `SKILL.md` at `<skills-root>/requirement-change-routing/SKILL.md`, or install this repository through the agent's skill-installation mechanism. Link it from the relevant work-type entries in the target repository's agent instructions.
