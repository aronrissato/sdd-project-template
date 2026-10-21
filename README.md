# Spec-Driven Development Project Template

Reusable starting point for software projects developed collaboratively with AI using a Spec-Driven Development (SDD) workflow.

This repository defines the **process and document structure**. Each actual project should have its own copy of these documents, filled with that project's approved decisions.

## Documents

- [`project.md`](project.md) — problem, objectives, audience, success criteria, and initial scope.
- [`requirements.md`](requirements.md) — functional and non-functional requirements, business rules, expected behavior, edge cases, and acceptance criteria.
- [`design.md`](design.md) — architecture, technologies, components, interfaces, data, security, and technical decisions.
- [`tasks.md`](tasks.md) — ordered implementation tasks, dependencies, deliverables, and verification.
- [`constitution.md`](constitution.md) — principles and constraints the AI and contributors must follow.
- [`WORKFLOW.md`](WORKFLOW.md) — how to apply the template from idea discovery to implementation.
- [`PROMPT.md`](PROMPT.md) — reusable prompt to start a new project conversation.

## How to use this template

1. Create a separate repository for the actual project. Do not use this template repository to store a project's specific requirements or code.
2. Copy the Markdown files into the new project repository.
3. Start a new chat using the prompt in `PROMPT.md`, replacing only `[INSIRA A IDEIA AQUI]` with your idea.
4. Ask the assistant to read this template and the project files before making changes. If private repository access is unavailable, provide the file contents or connect an authorized GitHub integration.
5. Work through discovery and approval before locking requirements, technical design, or implementation tasks.
6. Implement one task at a time and verify the result against the acceptance criteria.
7. Keep project documents synchronized with approved decisions and the real implementation state.

## Important principles

- The template is a guide, not a reason to over-document.
- Unknown details should remain explicit open questions, not silently become requirements.
- Proposed decisions are not approved decisions.
- Do not begin implementation while a critical requirement or design question remains unresolved.
- Verify work with tests, checks, and observable results; do not rely only on an AI's claim that a task is complete.
- Update specifications when scope or behavior changes.

## Language

The template's guidance is written in English for consistent use with coding tools, but project conversations and project documentation may be in Portuguese or another language chosen by the user.
