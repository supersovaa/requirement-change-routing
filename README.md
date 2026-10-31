# requirement-change-routing

A lightweight skill for routing **unsettled requirement decisions** to the appropriate user-grilling workflow, regardless of the phase in which they are discovered.

## When to use

Use it when creating or revising requirements or constraints, or when design, planning, implementation, tests, or review expose a decision about the required behavior.

The skill compares the user's effective decisions with the authoritative requirements/design, distinguishing required behavior from current code and test behavior. It sends only unresolved decisions to the responsible clarification workflow. New requirements or constraints proposed by the assistant require the user's decision before adoption. Work independent of those decisions can continue.

## Responsibility and related skills

- [`SKILL.md`](SKILL.md) contains the complete behavior.
- [`grill-into-pr`](https://github.com/supersovaa/grill-into-pr) owns detailed user grilling and documentation-only design PRs when the work uses that workflow.
- [`feature-introduction-threshold`](https://github.com/supersovaa/feature-introduction-threshold) evaluates the value and scope of functional choices.
- [`implemented-feature-change-handoff`](https://github.com/supersovaa/implemented-feature-change-handoff) hands settled changes to already implemented features into implementation and test planning.

This skill provides routing rather than a second grilling process or a requirement-history store.

## Installation

Place `SKILL.md` at `<skills-root>/requirement-change-routing/SKILL.md` in the target agent's skill directory, or install this repository using the agent's skill-installation mechanism. Link to the skill from each applicable work-type entry in the target repository's agent instructions.
