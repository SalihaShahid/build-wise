# Bug Fix TDD

Use TDD for bug fixes by first creating a regression test that reproduces the
problem.

## Process

1. Understand the reported bug.
2. Identify expected behavior.
3. Reproduce the incorrect behavior.
4. Write a regression test demonstrating the expected behavior.
5. Run the test and confirm it fails for the correct reason.
6. Implement the smallest fix.
7. Run the regression test and confirm it passes.
8. Run related tests.
9. Refactor if necessary while keeping tests passing.
10. Run regression tests again.

## Regression Test

The regression test should remain in the test suite after the fix.

It should verify the behavior that previously failed.

## Scope

Fix the reported problem without introducing unrelated changes.

If the bug reveals a broader issue, keep unrelated improvements separate unless
they are required to complete the current task.
