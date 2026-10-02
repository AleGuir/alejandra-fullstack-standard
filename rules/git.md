# Git Rules

## Branches

Recommended:

main
develop
feature/*
fix/*
refactor/*
hotfix/*

---

## Commits

Use clear and descriptive commit messages.

Prefer Conventional Commits:

feat:
fix:
refactor:
docs:
test:
chore:
perf:

Example:

feat: add employee vacation request

---

## Pull Requests

A PR should explain:

- what changed
- why it changed
- how it was tested
- potential risks

Avoid mixing unrelated changes in one PR.

---

## Before Merge

Verify:

- TypeScript
- lint
- tests
- build
- security-sensitive changes