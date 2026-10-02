# Backend Rules

## General

Backend code must prioritize:

- validation
- security
- predictable behavior
- separation of concerns
- testability

---

## Request Flow

Prefer:

Request
→ Validation
→ Authentication
→ Authorization
→ Controller/Handler
→ Service
→ Repository/Data Access
→ Response

---

## Validation

Never trust client input.

Validate:

- body
- query parameters
- route parameters
- uploaded files
- external API responses

Use a schema validation library when appropriate.

---

## Errors

Do not expose:

- stack traces
- database errors
- internal paths
- secrets
- implementation details

Return meaningful HTTP status codes.

---

## External APIs

External integrations should be isolated.

Prefer:

services/integrations/

rather than mixing external API calls throughout the application.