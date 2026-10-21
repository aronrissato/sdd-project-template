# Working Agreement and SDD Workflow

This document explains how to use the template without making discovery or documentation a project of its own.

## Guiding idea

Translate the idea into an agreed specification, translate that specification into a technical design and a verifiable task plan, then implement in small increments.

The process is iterative: new information may lead to changes, but changes should be explicit, reviewed, and reflected in the documents.

## Stage 1 — Discover the idea

Start with a free-form description from the project owner.

The assistant should:
- Understand the problem and intended outcome before discussing architecture.
- Ask focused questions conversationally, preferably one at a time.
- Prioritize questions that influence scope, user value, constraints, or major decisions.
- Maintain a short list of open questions and assumptions.
- Avoid requiring the owner to know technical terminology.

**Exit condition:** There is enough shared understanding to draft the project vision.

## Stage 2 — Draft and approve the vision

Fill out `project.md`. Keep answers concise and mark unknowns clearly.

Review:
- Problem and objectives.
- Target users and context.
- Success criteria.
- Initial scope and explicit exclusions.
- Constraints, assumptions, and open questions.

**Gate:** The project owner approves the vision before detailed requirements are treated as agreed scope.

## Stage 3 — Define and approve requirements

Fill out `requirements.md` with user journeys, functional requirements, business rules, non-functional requirements, edge cases, and acceptance criteria as appropriate.

Check:
- Requirements do not contradict each other.
- Important behavior is observable and testable.
- Priorities are explicit.
- Critical unknowns are resolved or explicitly accepted as risks.
- Requirements trace back to project objectives.

**Gate:** The owner reviews and approves the initial requirements before material design and implementation decisions are finalized.

## Stage 4 — Propose and approve the design

Fill out `design.md` at the level of detail needed by the project. Choose technologies based on requirements and constraints, not habit or novelty alone.

Review:
- Components and responsibilities.
- Data and interfaces.
- Security, privacy, failure handling, and operations as relevant.
- Test strategy.
- Material alternatives, trade-offs, and architectural decisions.

**Gate:** The owner approves material technical choices before implementation begins.

## Stage 5 — Create the task plan

Fill out `tasks.md`. Break the design into focused tasks with dependencies, deliverables, requirement references, acceptance criteria, and verification instructions.

Order tasks so that foundational and high-risk dependencies are handled before dependent work. Prefer increments that can be tested and understood independently.

**Gate:** The task plan is reviewed and sufficiently clear before execution.

## Stage 6 — Implement one task at a time

For each task:

1. Confirm the task is Ready and its dependencies are complete.
2. Read relevant specifications and existing code.
3. State the task goal and boundaries.
4. Implement only the approved scope.
5. Run relevant tests and project checks.
6. Compare actual behavior with acceptance criteria.
7. Record changed files, verification evidence, limitations, and follow-ups.
8. Update the task and related documentation.

If implementation reveals a contradiction or missing requirement, pause affected work and propose a specification change. Do not use coding as a substitute for a decision that changes intended behavior.

## Stage 7 — Validate milestones and release readiness

For each milestone, verify end-to-end outcomes against the agreed exit criteria. Before any release, deployment, or other consequential external action, review the plan and obtain the required authorization.

Record known issues, operational steps, rollback or recovery needs where relevant, and remaining work.

## Change-control rules

When a new idea, issue, or requirement appears:
1. Describe the change and why it matters.
2. Identify affected objectives, requirements, design decisions, tasks, tests, risks, schedule, and cost as appropriate.
3. Recommend a proportionate option.
4. Obtain approval for material changes.
5. Update the source documents before implementing the changed behavior.

## Communication style

- Be direct, practical, and clear.
- Explain technical terms when needed for an informed decision.
- Do not overwhelm the owner with a long questionnaire.
- Do not repeat questions already answered.
- When several minor decisions can be made together, group them into a concise proposal.
- Clearly state what is known, assumed, proposed, approved, implemented, and verified.
- Avoid excessive documentation and ceremony.

## Status report format

At meaningful checkpoints, report:

- **Current stage**
- **Decisions approved**
- **Work completed**
- **Verification performed and results**
- **Open questions or blockers**
- **Next recommended step**

Do not claim work has been completed or verified without evidence.
