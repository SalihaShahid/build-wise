# TDD Cycle

Use this process for every meaningful behavior.

## 1. Identify Behavior

Select one behavior from the task or acceptance criteria.

Define:

- Given
- When
- Then

Keep the behavior focused.

## 2. Write Test

Write the smallest test that describes the expected behavior.

The test must be written before the implementation for that behavior.

## 3. Run Test

Run the test.

Confirm that it fails because the required behavior is missing or incorrect.

If it fails because of test setup, configuration, imports, or unrelated
infrastructure problems, resolve those problems before continuing.

## 4. Implement

Implement the minimum production code required to make the test pass.

Do not implement speculative behavior.

Do not perform unrelated refactoring.

## 5. Run Test Again

Run the new test.

Confirm that it passes.

Run closely related tests to ensure the implementation did not break existing
behavior.

## 6. Refactor

When tests are passing:

- Improve naming.
- Remove unnecessary duplication.
- Simplify logic.
- Improve structure.
- Follow existing project conventions.

Do not change observable behavior during refactoring.

Run the affected tests again after refactoring.

## 7. Continue

Move to the next behavior and repeat the process.

```text
Behavior 1 → Test → Fail → Implement → Pass → Refactor
Behavior 2 → Test → Fail → Implement → Pass → Refactor
Behavior 3 → Test → Fail → Implement → Pass → Refactor
