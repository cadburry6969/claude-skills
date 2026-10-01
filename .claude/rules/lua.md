---
paths:
  - "modules/**/*.lua"
  - "bridge/**/*.lua"
  - "config/**/*.lua"
  - "*.lua"
---

# Lua Rules

- Use Lua typings and annotations where they improve type safety and editor support.
- Prefer local variables and local functions.
- Avoid unnecessary global variables.
- Avoid modifying global state unless explicitly required.
- Keep functions small and focused.
- Prefer early returns over deeply nested conditions.
- Avoid unnecessary table mutations.
- Do not attach functions to tables unless there is a clear reason to do so.
- Reuse existing functions instead of duplicating logic.
- Validate external or user-provided values before using them.
- Handle nil values explicitly where appropriate.
- Do not silently ignore errors.
- Keep client-only and server-only logic separated.
- Do not trust client-provided values on the server.
- Avoid unnecessary loops over large tables.
- Cache values that are repeatedly accessed in performance-sensitive code.
- Use descriptive names for variables and functions.
- Keep configuration values inside the appropriate config files.