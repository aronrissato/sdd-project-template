# Technical Design

> **Purpose:** Explain how the approved requirements will be implemented and why the chosen approach is appropriate.
>
> Technical choices are proposals until approved. Avoid premature architecture and unnecessary abstraction.

## 1. Status and context

- **Status:** Draft / In review / Approved
- **Last reviewed:** [YYYY-MM-DD]
- **Requirements:** See [requirements.md](requirements.md)
- **Project vision:** See [project.md](project.md)

## 2. Design goals and constraints

List the key qualities the design must support, derived from requirements: simplicity, reliability, security, maintainability, performance, portability, cost, and so on.

## 3. Proposed solution overview

Describe the system and its major parts in plain language. Include a diagram if it clarifies boundaries or data flow.

```text
[User / Client] -> [Application] -> [Storage or external system]
```

Replace this illustrative diagram with one relevant to the actual project.

## 4. Technology choices

| Concern | Proposed choice | Rationale | Alternatives considered | Status |
| --- | --- | --- | --- | --- |
| Language / runtime | [Choice] | [Why it fits] | [Alternatives] | Proposed |
| UI / interface | [Choice or N/A] | [Rationale] | [Alternatives] | Proposed |
| Persistence | [Choice or N/A] | [Rationale] | [Alternatives] | Proposed |
| Hosting / deployment | [Choice or N/A] | [Rationale] | [Alternatives] | Proposed |
| Testing | [Choice] | [Rationale] | [Alternatives] | Proposed |

Include only concerns relevant to this project.

## 5. Components and responsibilities

| Component | Responsibility | Depends on | Requirement IDs |
| --- | --- | --- | --- |
| [Component] | [Single clear responsibility] | [Dependencies] | [FR / NFR IDs] |

Explain important boundaries. Do not create components solely to make the architecture look sophisticated.

## 6. Data design

Describe important entities, relationships, ownership, lifecycle, validation, retention, and migrations where applicable. Add schema or diagrams only when useful.

- **Source of truth:** [Where authoritative data lives]
- **Sensitive data:** [What, if any, and how it is protected]
- **Backup / recovery:** [Requirements or N/A]
- **Migration / compatibility:** [Approach or N/A]

## 7. Interfaces and contracts

Document APIs, events, commands, file formats, integrations, and component contracts needed to implement the requirements.

For each interface, specify relevant inputs, outputs, error responses, validation, authentication/authorization, compatibility expectations, and timeouts or retry behavior.

## 8. Security, privacy, and reliability

Record relevant design measures and how they satisfy requirements. Consider authentication, authorization, secret management, input validation, logging of sensitive data, dependency risks, failure modes, recovery, and access boundaries.

Do not claim a control exists until it is implemented and verified.

## 9. Observability and operations

When relevant, describe logs, metrics, traces, health checks, alerts, configuration, deployment, and troubleshooting. Keep operational design proportional to the project.

## 10. Testing strategy

Map verification levels to requirements and risks.

- **Unit tests:** [What should be tested in isolation]
- **Integration tests:** [Dependencies and contracts]
- **End-to-end / acceptance tests:** [Critical user flows]
- **Security / performance tests:** [Only when relevant]
- **Manual checks:** [What cannot yet be automated]

Identify test data needs and how tests will be run.

## 11. Deployment and configuration

Describe environments, configuration sources, secret handling, build and release steps, rollback, and setup instructions as relevant. Never put real secrets or credentials in this file or repository.

## 12. Architectural decisions

Record material choices as short Architecture Decision Records (ADRs), inline or in separate files as appropriate.

### ADR-001 — [Decision title]

- **Status:** Proposed / Accepted / Superseded
- **Context:** [Problem and constraints]
- **Decision:** [Chosen approach]
- **Alternatives:** [Other options]
- **Consequences:** [Trade-offs and follow-up work]

## 13. Risks and unresolved design questions

| ID | Risk / question | Impact | Mitigation / next step | Status |
| --- | --- | --- | --- | --- |
| DQ-001 | [Item] | Low / Medium / High | [Action] | Open |

## 14. Approval

- **Status:** Draft / In review / Approved
- **Approved by:** [Name or role]
- **Date:** [YYYY-MM-DD]
- **Conditions:** [Details]

The design should be detailed enough to guide implementation, but no more complicated than the requirements justify.
