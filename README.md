# 🛠️ Build-Wise

> **Your development copilot for turning ideas into well-defined, actionable, and tested software.**

Build-Wise is a Claude plugin that helps developers move from **unclear ideas to structured implementation**.

It guides you through the development process by helping you:

* Clarify and finalize requirements
* Identify missing information before development starts
* Break requirements into small, implementable tasks
* Define task dependencies and implementation order
* Connect tasks back to the requirements they cover
* Implement tasks using a Test-Driven Development (TDD) workflow

Instead of jumping straight into code, Build-Wise helps you **understand → plan → implement → test**.

---

##  Why Build-Wise?

A lot of development problems don't start with code.

They start with things like:

* Vague requirements
* Missing edge cases
* Unclear scope
* Assumptions that were never discussed
* Tasks that are too large
* Hidden dependencies between tasks
* Tests being written only after implementation

Build-Wise is designed to address these problems before and during implementation.

### The workflow

```text
┌──────────────────────┐
│       Idea           │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Requirements         │
│ Gathering            │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Finalized             │
│ Requirements          │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Task Planning         │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Ordered Tasks +       │
│ Dependencies          │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ TDD Implementation    │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Tested Feature        │
└──────────────────────┘
```

---

# 🧩 Skills

Build-Wise currently provides three core development skills.

## 1. Requirements Gathering

The **requirements-gathering** skill helps turn a vague idea or feature request into a clear requirements document.

Instead of immediately making assumptions and writing code, Build-Wise asks relevant questions to uncover missing information.

### What it does

* Understands the initial feature or idea
* Identifies incomplete information
* Detects ambiguity
* Finds potential edge cases
* Asks relevant questions
* Clarifies goals
* Defines feature scope
* Identifies functional requirements
* Identifies non-functional requirements
* Documents assumptions and constraints
* Produces a structured requirements document
* Allows requirements to be reviewed and refined before implementation

### Requirements Document

The resulting requirements document can include:

```text
Goals
Scope
Functional Requirements
Non-Functional Requirements
Constraints
Assumptions
Edge Cases
```

The user can then review and finalize the requirements before moving to implementation planning.

---

# 2. Task Planning

Once the requirements are finalized, the **task-planning** skill transforms them into smaller, actionable development tasks.


### What each task document includes

Each task can contain:

* Tasks with title and description
* Acceptance/checklist criteria against each task
* Requirements covered
* Dependencies
* Recommended implementation order


Build-Wise also identifies how these tasks relate to each other.

### Task Management Ready

The generated tasks are structured so they can be transferred into tools such as:

* ClickUp
* Linear
* Jira
* GitHub Issues
* Trello
* Other task management systems

The objective is to produce tasks that are clear enough to be picked up and implemented without having to rediscover the original requirements.

---

# 3. TDD

The **TDD** skill helps implement individual tasks using a Test-Driven Development workflow.

The basic cycle is:

```text
       ┌──────────────┐
       │     RED      │
       │ Write a test │
       │ that fails   │
       └──────┬───────┘
              ↓
       ┌──────────────┐
       │    GREEN     │
       │ Implement    │
       │ functionality│
       └──────┬───────┘
              ↓
       ┌──────────────┐
       │   REFACTOR   │
       │ Improve code │
       │ safely       │
       └──────┬───────┘
              │
              └──────────────→ RED
```

### What it does

For a given task, Build-Wise:

1. Understands the task and its requirements
2. Identifies expected behavior
3. Generates relevant test cases
4. Writes tests before implementation
5. Runs or evaluates the tests so they initially fail when appropriate
6. Implements the required functionality
7. Verifies the tests pass

The tests become an executable representation of the expected behavior.

---

# 🔗 How the Skills Work Together

The three skills are designed to work as a connected workflow.

```text
Requirements
     │
     ↓
Task Planning
     │
     ↓
Individual Task
     │
     ↓
TDD
     │
     ↓
Tested Implementation
```

This creates a traceable development flow:

```text
Requirement
     ↓
Task
     ↓
Test
     ↓
Implementation
```


This connection helps keep implementation aligned with the original requirements.

---

# 💡 Usage

Build-Wise can be used throughout the development process.

## Start with Requirements

Give Build-Wise a feature idea:

```text
I want to add a subscription cancellation feature.
```

Use the requirements-gathering skill to identify what needs to be clarified.

For example:

```text
Use requirements-gathering for this feature.
```

Build-Wise will ask relevant questions until the requirements are sufficiently defined.

---

## Finalize Requirements

Once the questions have been answered, Build-Wise produces a structured requirements document.

Review the document and make any necessary changes.

The requirements become the source of truth for the next stage.

---

## Generate Tasks

Once the requirements are finalized:

```text
Create implementation tasks from these requirements.
```

Build-Wise produces individual tasks with:

```text
Task
Description
Acceptance Criteria
Requirements Covered
Dependencies
Implementation Order
```

---

## Implement a Task

Select an implementation task and use the TDD skill:

```text
Implement this task using TDD.
```

Build-Wise will guide the implementation through:

```text
Test
 ↓
Fail
 ↓
Implementation
 ↓
Pass
 ↓
Refactor
```

---


# 🎯 Design Principles

Build-Wise follows a few core principles.

## Clarify Before Coding

Don't immediately code against unclear requirements.

Ask questions first.

---

## Requirements Before Tasks

Tasks should be derived from finalized requirements.

```text
Idea
 ↓
Requirements
 ↓
Tasks
```

Not:

```text
Idea
 ↓
Random Tasks
```

---

## Small, Focused Tasks

A good task should be small enough to:

* Understand
* Implement
* Review
* Test

Large features should be decomposed into smaller pieces.

---

## Testable Behavior

Tasks should have clear acceptance criteria and expected behavior.

This makes it easier to translate requirements into tests.

---

## Traceability

Build-Wise aims to maintain a connection between every stage:

```text
Requirement
     ↓
Task
     ↓
Acceptance Criteria
     ↓
Test
     ↓
Implementation
```

This helps reduce the chance of implementing something that doesn't actually satisfy the original requirement.

---

# 🤝 Contributing

Contributions and ideas are welcome.

If you have an idea for improving Build-Wise:

1. Open an issue
2. Describe the problem or proposed improvement
3. Explain how it fits into the Build-Wise workflow
4. Submit a pull request if you'd like to implement it

When contributing a new skill, try to keep it:

* Focused on a specific development activity
* Reusable across projects
* Clear in its workflow
* Practical for real development
* Consistent with the principles of Build-Wise

---

# 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for details.

---

# ⭐ Support the Project

If Build-Wise is useful to you, consider giving the repository a ⭐ on GitHub.

Feedback, issues, ideas, and contributions are always welcome.

---

# 🧠 Build Wisely

Software development isn't just about writing code.

It's about understanding the problem, defining what needs to be built, breaking it into manageable pieces, and verifying that the implementation actually does what was intended.

Build-Wise brings those steps together into one development workflow:

```text
          THINK
            ↓
       REQUIREMENTS
            ↓
           PLAN
            ↓
          BUILD
            ↓
           TEST
            ↓
         REFACTOR
```

**Build-Wise — Think clearly. Plan carefully. Build confidently.**
