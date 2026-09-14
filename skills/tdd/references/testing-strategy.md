
### `references/testing-strategy.md`

```md
# Testing Strategy

Choose the smallest test level that provides meaningful confidence.

## Unit Tests

Prefer for:

- Business rules
- Domain logic
- Validation
- Pure functions
- Isolated error handling

## Component Tests

Prefer for:

- UI behavior
- Component state
- User interaction
- Rendering
- Component validation

Test observable behavior rather than internal implementation.

## Integration Tests

Use when behavior depends on multiple components or system boundaries.

Examples:

- Database interaction
- API integration
- Service interaction
- Serialization
- External service adapters

## End-to-End Tests

Use for important complete user workflows.

Examples:

- Authentication
- Registration
- Checkout
- Critical business workflows

Do not use E2E tests when a lower-level test provides sufficient confidence.

## Test Selection

For each behavior ask:

1. What is the smallest meaningful test boundary?
2. Can this behavior be tested without external dependencies?
3. Does the behavior cross a system boundary?
4. Does the behavior require complete user-flow verification?

Prefer focused tests.

## Regression Testing

After implementation:

1. Run new tests.
2. Run modified tests.
3. Run closely related tests.
4. Run the broader test suite when practical.

Investigate failures caused by the implementation.

Do not remove or weaken tests simply to obtain a passing suite.
