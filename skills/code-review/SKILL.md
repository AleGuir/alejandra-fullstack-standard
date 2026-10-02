# Code Review

Review code using the following order.

## 1. Correctness

Does the code actually solve the requested problem?

## 2. Architecture

Does it follow the project architecture?

## 3. Security

Check:

- authentication
- authorization
- input validation
- secrets
- data exposure
- RLS

## 4. TypeScript

Check:

- unsafe any
- incorrect types
- unnecessary casts
- duplicated types

## 5. Maintainability

Check:

- duplication
- excessive complexity
- unclear naming
- unnecessary abstractions

## 6. Performance

Check:

- unnecessary queries
- unnecessary renders
- excessive client components
- caching opportunities

## 7. Testing

Check whether relevant behavior is tested.

## 8. Documentation

Check whether important architectural changes are documented.

## Output

Categorize findings as:

CRITICAL
HIGH
MEDIUM
LOW
SUGGESTION