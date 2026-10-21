# Implementation Plan

> **Purpose:** Turn approved requirements and design into small, ordered, verifiable implementation tasks.
>
> This is a living plan. Update task statuses as work progresses and keep it consistent with the code and specifications.

## 1. Current state

- **Plan status:** Draft / In review / Approved
- **Current milestone:** [Milestone]
- **Last updated:** [YYYY-MM-DD]
- **Requirements:** See [requirements.md](requirements.md)
- **Design:** See [design.md](design.md)

## 2. Task status definitions

Use these statuses consistently:

- **Proposed:** Identified but not approved for execution.
- **Ready:** Scope, dependencies, and verification are clear.
- **In progress:** Implementation is underway.
- **Blocked:** Cannot proceed; blocker is recorded.
- **In review:** Implementation is complete and awaiting verification/review.
- **Done:** Acceptance criteria and required checks have passed.
- **Deferred:** Intentionally moved out of the current plan with rationale.

## 3. Milestones

Define small milestones that produce useful, verifiable increments.

| Milestone | Outcome | Included task IDs | Exit criteria | Status |
| --- | --- | --- | --- | --- |
| M-01 | [Useful increment] | [T-001, T-002] | [What must be true] | Proposed |

## 4. Task backlog

| ID | Task | Depends on | Requirement / design references | Verification | Status |
| --- | --- | --- | --- | --- | --- |
| T-001 | [One bounded deliverable] | None | [FR-001, ADR-001] | [Test or observable check] | Proposed |

Task ordering must respect dependencies. Avoid tasks that combine unrelated features or hide several uncertain design decisions.

## 5. Task detail template

Use this template for tasks that are complex or risky enough to need additional detail.

### T-001 — [Task title]

- **Status:** Proposed / Ready / In progress / Blocked / In review / Done / Deferred
- **Goal:** [Specific outcome]
- **Context:** [Why this task exists]
- **Scope included:** [What will change]
- **Scope excluded:** [What must not change]
- **Dependencies:** [Completed tasks or external prerequisites]
- **Requirements / design references:** [IDs and documents]
- **Expected deliverables:** [Files, behavior, configuration, etc.]
- **Acceptance criteria:** [Observable conditions]
- **Verification:** [Tests, commands, checks, and expected outcomes]
- **Risks / open questions:** [Items that could block implementation]
- **Result:** [What actually changed and verification evidence]

## 6. Definition of ready

A task is Ready when:

- Its objective and boundaries are understandable.
- Required decisions and dependencies are resolved.
- Its expected result connects to an approved requirement or an explicitly approved maintenance need.
- Acceptance criteria and verification are clear enough to evaluate completion.
- No unresolved blocker makes the proposed implementation speculative.

## 7. Definition of done

A task is Done only when all applicable conditions are met:

- The implementation matches its approved scope.
- Relevant automated tests pass.
- Relevant build, lint, type-check, static-analysis, or other project checks pass.
- Acceptance criteria are verified, or any unavoidable manual verification is explicitly recorded.
- Documentation and configuration are updated as needed.
- No known critical regression or unresolved issue is hidden.
- Task status and actual outcome are recorded.

If a check cannot be run, record why and do not claim it passed.

## 8. Execution log

| Date | Task / milestone | Outcome | Verification evidence | Follow-up |
| --- | --- | --- | --- | --- |
| [YYYY-MM-DD] | [ID] | [Summary] | [Commands, tests, or manual checks] | [Next step] |

## 9. Blockers and changes

| ID | Blocker / change | Impact | Decision or next action | Status |
| --- | --- | --- | --- | --- |
| BL-001 | [Description] | [Affected work] | [Action / approval needed] | Open |

## 10. Progress summary

- **Done:** [Task IDs]
- **In progress:** [Task IDs]
- **Blocked:** [Task IDs and reasons]
- **Next task:** [ID and reason it is next]
- **Plan changes requiring approval:** [None or list]

Do not report a percentage complete unless the method of calculating it is clear and meaningful.
