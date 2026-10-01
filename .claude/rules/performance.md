---
paths:
  - "**/*"
---

# Performance Rules

- Avoid unnecessary polling.
- Prefer event-driven logic where possible.
- Avoid per-frame execution unless required.
- Avoid creating unnecessary objects inside frequently executed loops.
- Avoid repeated database queries for the same data.
- Cache frequently accessed immutable data when appropriate.
- Do not optimize prematurely at the expense of readability.
- When modifying performance-sensitive code, consider CPU usage, memory usage, network traffic, and database load.
- Avoid unnecessary NUI messages.
- Batch related NUI updates when possible.
- Clean up timers, threads, listeners, and event handlers when they are no longer needed.