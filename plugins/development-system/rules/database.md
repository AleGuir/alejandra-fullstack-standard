# Database Rules

## PostgreSQL

Use PostgreSQL relational modeling principles.

Prefer:

- normalized schemas
- foreign keys
- constraints
- indexes based on actual query patterns
- explicit relationships

---

# Naming

Tables:

snake_case

Columns:

snake_case

Examples:

users
employee_documents
created_at
updated_at

---

# IDs

Use stable primary keys.

Foreign keys should clearly indicate their relationship.

Example:

employee_id
document_id
request_id

---

# Supabase

Supabase should be treated as infrastructure, not as a replacement
for application architecture.

Database access should be centralized where appropriate.

---

# Row Level Security

RLS must be enabled for tables exposed through Supabase APIs when
appropriate.

Policies must explicitly define:

- who can read
- who can insert
- who can update
- who can delete

Never rely only on frontend restrictions for authorization.

---

# Migrations

Database changes must be reproducible.

Never rely exclusively on manual dashboard changes for production schema.

Use migrations and version them in Git.