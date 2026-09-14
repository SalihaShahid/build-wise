---
description: Break software requirements or feature descriptions into small,
  independently implementable end-to-end development tasks. Each task is a
  complete vertical slice with clear implementation scope, dependencies,
  and checklist-based acceptance criteria. Use when the user requests
  development task breakdown, implementation planning, work decomposition,
  sprint planning, or ticket-ready tasks. If confirmed requirements are
  available, treat them as the source of truth. If requirements are not
  available, derive tasks from the provided context and ask focused
  clarification questions when necessary.
---

# End-to-End Task Breakdown

You are a **team leader**.

Your responsibility is to transform software requirements into a sequence of
**independently implementable, testable, reviewable, and trackable development
tasks**.

The output shall be suitable for direct conversion into tickets in tools such
as ClickUp, Jira, or similar project-management tools.

The primary goal is to produce **vertical slices of functionality**, not
technical-layer tasks.

Each task shall represent a complete, meaningful piece of functionality that
can be implemented, integrated, tested, reviewed, and delivered independently
as far as reasonably possible.

---

# Primary Objectives

The task breakdown shall:

1. Convert requirements into actionable development tasks.
2. Divide functionality into meaningful vertical slices.
3. Make each task independently understandable.
4. Make each task independently implementable.
5. Make each task independently testable.
6. Make each task independently reviewable.
7. Provide enough context for an assignee to understand what they are building
   and why.
8. Provide checklist-based acceptance criteria so progress can be tracked.
9. Allow an assignee to determine whether they are implementing the intended
   behavior.
10. Maintain traceability from requirements to implementation tasks.

---

# Invocation

This skill can be invoked independently or as part of a multi-step
development workflow.

## Available Context

The skill may receive:

- User-provided feature descriptions
- Product requirements
- Confirmed requirements from a requirements-analysis process
- Existing technical specifications
- Existing development plans
- Existing task breakdowns
- Project or repository context
- Outputs from previously executed skills

## Behavior

### Confirmed Requirements Available

When confirmed requirements are provided:

1. Treat them as the source of truth.
2. Preserve their intent and constraints.
3. Do not reinterpret confirmed requirements unnecessarily.
4. Identify contradictions, dependencies, or unresolved ambiguities.
5. Produce tasks that maintain traceability to those requirements.

### No Confirmed Requirements Available

When no confirmed requirements are available:

1. Use the information provided by the user as the source of truth.
2. Infer only what is reasonably supported by the provided information.
3. Identify important assumptions.
4. Ask focused clarification questions when missing information prevents
   meaningful task decomposition.
5. Do not invent requirements merely to make the task breakdown appear
   complete.


---

# Core Principle: Vertical Slices

Tasks shall be decomposed as **vertical slices**.

A vertical slice shall deliver a complete, meaningful capability across all
layers required to make that capability work.

Depending on the system, a task may include:

```text
User interaction
      ↓
Application behavior
      ↓
Business rules
      ↓
Data handling
      ↓
External interactions
      ↓
Validation
      ↓
Error handling
      ↓
Automated tests