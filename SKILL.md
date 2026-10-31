---
name: requirement-change-routing
description: Route unsettled requirement or constraint decisions to the owning clarification workflow when they arise during any kind of work.
---

# Requirement Change Routing

Use this skill when creating or revising requirements or constraints, including when another work phase would introduce a new guarantee.

This skill targets a single-user AI-agent workflow.

## During existing work

Use the user's effective decisions and the relevant requirements/design canon already available to the owning work. Focus on the affected requirements when a new or revised obligation is about to be adopted; reuse existing source checks.

Treat code and tests as evidence of current behavior rather than authority for additional requirements. Route every assistant-proposed new requirement or constraint for a user decision through grilling. If a relevant existing requirement may rest on an unsupported assistant assumption, route its retention, revision, or removal for user judgment.

Proceed directly when the required behavior is already settled. Otherwise, pass the specific unresolved choice and its available evidence to the owning requirements/design clarification workflow; use `grill-into-pr` when applicable. Reuse decisions already made and the owning workflow's questions, documents, and PRs.

Continue independent work while the affected work awaits a decision. Resume the affected work from the settled requirements/design through its normal skill.

## Responsibility

This skill owns the routing decision within existing work. The owning workflow performs clarification and maintains the canon; this skill adds no separate approval stage, recurring repository scan, or tracking artifact.
