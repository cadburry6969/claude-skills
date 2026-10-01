---
paths:
  - "**/*"
---

# Testing Rules

- Test new functionality when practical.
- When fixing a bug, consider adding a regression test.
- Test important edge cases.
- Do not remove existing tests merely to make a change pass.
- Do not modify tests to hide an actual implementation bug.
- Keep tests deterministic.
- Avoid tests that depend on external services unless the test explicitly requires integration testing.
- Test authorization and validation logic separately from UI behavior.