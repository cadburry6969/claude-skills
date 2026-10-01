---
paths:
  - "**/*.{ts,tsx}"
---

# TypeScript Rules

- Prefer TypeScript types over implicit any.
- Avoid any unless absolutely necessary.
- Prefer interfaces or type aliases that clearly describe domain data.
- Keep types close to the code they describe when they are not shared.
- Use shared types for data exchanged between modules.
- Avoid unnecessary type assertions.
- Validate unknown external data before treating it as a known type.
- Prefer optional chaining and nullish coalescing where appropriate.
- Avoid non-null assertions unless the value is guaranteed to exist.
- Keep functions strongly typed.
- Do not duplicate type definitions for the same data structure.