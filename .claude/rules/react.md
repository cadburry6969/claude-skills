---
paths:
  - "web-source/**/*.{ts,tsx,js,jsx}"
  - "web/**/*.{ts,tsx,js,jsx}"
---

# React Rules

- Use modularized components.
- Keep components focused on a single responsibility.
- Avoid unnecessarily large components.
- Prefer reusable components for repeated UI patterns.
- Keep business logic out of presentational components where practical.
- Use TypeScript for new code.
- Define explicit types for component props.
- Avoid using any unless there is a strong reason.
- Prefer existing shared components before creating duplicates.
- Keep API/NUI communication separate from UI rendering where practical.
- Avoid unnecessary useEffect calls.
- Do not use useEffect for derived values that can be calculated directly.
- Avoid unnecessary state.
- Prefer derived values over duplicated state.
- Use stable keys when rendering lists.
- Do not use array indexes as keys when a stable identifier is available.
- Keep components readable and avoid deeply nested JSX.