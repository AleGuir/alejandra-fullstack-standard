# Database Migration

Use when modifying the database schema.

## Process

1. Understand current schema.
2. Check existing relationships.
3. Check RLS policies.
4. Determine migration impact.
5. Create migration.
6. Update types.
7. Update affected services.
8. Update tests.
9. Verify migration.
10. Document breaking changes.

## Never

- delete production data without explicit confirmation
- bypass migrations
- disable RLS casually
- expose privileged credentials