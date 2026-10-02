# Frontend Rules

## React

Prefer functional components.

Components should have a single clear responsibility.

Avoid:

- excessive prop drilling
- duplicated UI logic
- large monolithic components
- unnecessary client components

---

# Next.js

Use the App Router.

Prefer Server Components by default.

Use Client Components only when required by:

- state
- event handlers
- browser APIs
- client-side hooks
- interactive behavior

Do not add "use client" automatically.

---

# Data Fetching

Prefer server-side data fetching when possible.

Avoid unnecessary client-side fetching.

Do not expose secrets or privileged credentials to client code.

---

# Server Actions

Use Server Actions for appropriate server mutations when they simplify
the architecture.

Validate all input received by Server Actions.

Server Actions must enforce authorization.

---

# API Routes

API routes should:

1. Validate input.
2. Authenticate the request when required.
3. Authorize the operation.
4. Execute business logic.
5. Return a consistent response.
6. Handle expected errors.
7. Avoid leaking internal implementation details.

---

# TypeScript

Avoid:

any

Prefer:

- interfaces
- types
- generics
- discriminated unions
- explicit return types where useful

Do not disable TypeScript checks to bypass implementation problems.