# Testing Rules

Testing should exist at different levels.

## Unit Tests

Use for:

- pure functions
- business rules
- utilities
- transformations

---

## Integration Tests

Use for:

- database operations
- API behavior
- service integrations

---

## E2E Tests

Use for critical user flows.

Examples:

- login
- registration
- checkout
- employee request
- administrative approval

---

## Testing Principle

Do not test implementation details unnecessarily.

Prefer testing behavior and outcomes.

Every important business rule should have automated coverage.