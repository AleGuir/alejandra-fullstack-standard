# Alejandra Fullstack Standard

## Purpose

This repository defines the development standards, architecture
principles, coding conventions, security practices and workflows
used across my fullstack projects.

These standards are intended to be used by developers and AI coding
agents.

---

# Core Principles

All development should prioritize:

- Clean Code
- SOLID
- DRY
- KISS
- Separation of Concerns
- Single Responsibility
- Maintainability
- Scalability
- Security
- Testability
- Explicit over implicit behavior

---

# Technology Standards

Default stack:

- Next.js
- React
- TypeScript
- PostgreSQL
- Supabase
- Git
- GitHub
- Vercel

---

# Architecture

Follow the architecture rules defined in:

- rules/architecture.md
- rules/frontend.md
- rules/backend.md
- rules/database.md
- rules/security.md
- rules/testing.md
- rules/git.md
- rules/documentation.md
- rules/naming.md

---

# General AI Development Rules

Before modifying code:

1. Inspect the existing architecture.
2. Inspect related components and modules.
3. Reuse existing functionality when possible.
4. Avoid unnecessary abstractions.
5. Do not introduce dependencies without justification.
6. Do not duplicate business logic.
7. Do not modify unrelated code.
8. Preserve existing conventions unless there is a documented reason
   to change them.

Before completing a task:

1. Validate the implementation.
2. Check TypeScript errors.
3. Check linting.
4. Run relevant tests.
5. Review security implications.
6. Review the generated diff.
7. Update documentation when necessary.

---

# Skills

Reusable development workflows are located in:

skills/

When a task matches one of these workflows, use the corresponding skill.
