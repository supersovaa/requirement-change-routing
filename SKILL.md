---
name: requirement-change-routing
description: Decide whether work can proceed under settled requirements and design or needs a user decision through the owning clarification workflow.
---

# Requirement Change Routing

Use this skill when deciding whether to ask the user for a requirements/design decision during any kind of work, including creating or revising requirements or constraints and proposing new guarantees.

This skill targets a single-user AI-agent workflow.

## During existing work

Use the user's effective decisions and the relevant requirements/design canon already available to the owning work. Focus on the affected requirements; reuse existing source checks.

Treat code and tests as evidence of current behavior rather than authority for additional requirements.

Before framing a user decision, resolve factual questions from available sources and check whether the effective decisions and relevant canon already settle the required behavior.

For a discrepancy with the canon, first check for a correction that satisfies the settled requirements and design. Carry such a correction through the owning work phase. Choose among compliant implementation options within that phase's authority.

Offer revision of the canon as a user choice only with a concrete basis for reconsidering the governing requirement or constraint, such as a user-requested change, a conflict among requirements, or a relevant requirement supported only by an assistant assumption. Evaluate that basis independently of the implementation already present.

Route every assistant-proposed new requirement or constraint that remains after these checks for a user decision through grilling. If a relevant existing requirement may rest on an unsupported assistant assumption, route its retention, revision, or removal for user judgment.

Proceed directly when the required behavior is already settled. For each remaining decision, pass the specific unresolved requirement or constraint choice, the relevant contract, and evidence that leaves the required behavior unsettled to the owning requirements/design clarification workflow; use `grill-into-pr` when applicable. For a discrepancy, include the contract-preserving correction considered and the requirement-level obstacle that remains. Reuse decisions already made and the owning workflow's questions, documents, and PRs.

Continue independent work while the affected work awaits a decision. Resume the affected work from the settled requirements/design through its normal skill.

## Responsibility

This skill owns the routing decision within existing work. The current work phase owns corrections, implementation choices, and review classification. The owning clarification workflow performs clarification and maintains the canon. Keep this routing within the existing work and its existing artifacts.
