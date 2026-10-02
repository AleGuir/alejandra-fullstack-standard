# Security Rules

## Secrets

Never commit:

- API keys
- passwords
- tokens
- private keys
- service role keys

Use environment variables.

---

## Environment Variables

Public variables must use:

NEXT_PUBLIC_

Only values safe for browser exposure may use this prefix.

Private credentials must never use it.

---

## Authentication

Authentication answers:

"Who is this user?"

Authorization answers:

"What is this user allowed to do?"

Never treat authentication as authorization.

---

## Authorization

Every protected operation must verify permissions server-side.

Frontend restrictions are not security boundaries.

---

## Supabase

Never expose the Supabase service role key to the browser.

Use server-side environments for privileged operations.

---

## Input

Treat all external input as untrusted.

Validate and sanitize where appropriate.

---

## Files

Uploaded files must be validated for:

- type
- size
- permissions
- storage location

Do not trust client-provided MIME types alone.