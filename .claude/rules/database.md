---
paths:
  - "**/*.sql"
  - "**/*.lua"
  - "**/*.ts"
  - "**/*.js"
---

# Database Rules

- Use parameterized queries for all user-controlled values.
- Never construct SQL queries using direct string concatenation with user input.
- Keep database queries readable and maintainable.
- Avoid unnecessary database queries inside frequently executed loops.
- Prefer batching queries when multiple records must be processed.
- Handle database errors explicitly.
- Do not silently ignore failed queries.
- Use transactions when multiple related database changes must succeed or fail together.
- Do not modify the database schema without considering existing installations.
- Prefer migrations for schema changes.
- Preserve existing data when modifying schemas.
- Use appropriate indexes for frequently queried columns.
- Avoid SELECT * when only specific columns are required.
- Keep database-specific logic out of UI components.