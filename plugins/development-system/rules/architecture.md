# Architecture Rules

## General

Applications should be organized around business domains and clear
responsibilities rather than only technical layers.

Prefer:

Feature / Domain based organization

over:

A single global folder for all components, services and utilities.

---

## Separation of Concerns

The following responsibilities should remain separated:

- UI
- Business logic
- Data access
- API transport
- Authentication
- Authorization
- External integrations

---

## Business Logic

Business rules should not be embedded directly inside UI components.

Business logic should live in:

- services
- domain modules
- reusable functions
- server-side modules

depending on complexity.

---

## Services

Create a service when:

- logic is reused
- logic communicates with an external system
- logic contains business rules
- logic requires multiple operations

Do not create services for trivial one-line operations.

---

## Components

Create a component when:

- UI is reused
- UI has independent responsibility
- UI has internal state
- UI complexity makes the parent difficult to maintain

Avoid creating components solely to reduce file length.

---

## Hooks

Create a custom hook when:

- stateful behavior is reused
- browser behavior needs encapsulation
- multiple components share the same client-side logic

Do not create hooks for simple calculations that can remain pure functions.

---

## API Endpoints

Create an endpoint when:

- an external client needs access
- a client/server boundary is required
- the operation represents a meaningful resource or action

Do not create endpoints for internal functions that can safely execute
on the server.

---

## Abstractions

Do not create abstractions before a real need exists.

Prefer simple implementations first.

Introduce abstractions when they provide:

- reuse
- testability
- separation
- extensibility
- reduced coupling