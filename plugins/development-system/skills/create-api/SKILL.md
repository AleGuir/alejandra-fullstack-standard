# Create API

Use this workflow when creating a new API endpoint.

## Steps

1. Understand the requested resource.
2. Inspect existing API conventions.
3. Determine whether an existing endpoint can be extended.
4. Define input schema.
5. Define authorization requirements.
6. Implement business logic in a service when appropriate.
7. Keep data access separated.
8. Implement the endpoint.
9. Implement consistent error handling.
10. Add tests.
11. Update API documentation.

## Before coding

Inspect:

- existing endpoints
- services
- schemas
- authentication
- authorization
- database models

## Never

- expose secrets
- trust client input
- duplicate business logic
- bypass authorization
- put complex business logic directly inside route handlers