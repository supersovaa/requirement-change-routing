---
name: requirement-change-routing
description: Identify unresolved requirement decisions during any work phase and route them to the responsible grilling workflow before dependent changes proceed.
---

# Requirement Change Routing

Use this skill whenever a task creates or revises requirements or constraints, or exposes a requirement decision during design, planning, implementation, testing, review, or other work.

This skill targets a single-user AI-agent workflow.

## Identify the decision

Compare the user's current instructions and effective decisions with the relevant requirements and design canon.
Use code, tests, and other implementation artifacts as evidence of current behavior; use the canon and user decisions to establish required behavior.

Identify decisions that remain unsettled about the requested change and its relevant existing requirements.
When a relevant existing requirement may have originated from an unsupported assistant assumption, route the decision to retain, revise, or remove it to the user.
Treat every assistant-proposed new requirement or constraint as a user decision to settle through grilling before adding it to the canon, plan, implementation contract, or acceptance criteria.

## Route and continue

When the required behavior is already determined by the user's instructions and the canon, proceed with the owning work.
When a user decision remains, route it to the workflow that owns requirements or design clarification. Use `grill-into-pr` for GitHub-based requirements/design changes when that workflow applies; use the established owning workflow otherwise.
Give that workflow the affected requirement, the available authoritative evidence, and the specific unresolved decision. Reuse decisions already settled; let the owning workflow manage question format, documentation, and PRs.
Hold only work dependent on the unsettled decision. Continue work whose correctness is independent of that decision.
Resume affected work from the settled requirements and design through its normal work-phase skill.

## Responsibility

This skill owns detecting unsettled requirement changes and routing their decisions.
The clarification workflow owns grilling and the authoritative requirements/design updates; implementation, planning, testing, and review retain their existing owners.
