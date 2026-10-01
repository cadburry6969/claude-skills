---
paths:
  - "**/*.lua"
  - "fxmanifest.lua"
---

# FiveM Rules

- Keep client and server responsibilities clearly separated.
- Never trust client-provided data on the server.
- Validate all important client-triggered events server-side.
- Never allow the client to directly control protected server state.
- Use RegisterNetEvent only when an event needs to be triggered remotely.
- Prefer local events when network communication is unnecessary.
- Avoid unnecessary network events.
- Keep event names consistent and descriptive.
- Do not expose sensitive server-side information to clients.
- Never place API keys, tokens, database credentials, or secrets in client files.
- Keep server-only dependencies and logic on the server.
- Use GetResourceState when resource availability must be verified.
- Check dependencies before calling exports from another resource when appropriate.
- Avoid unnecessary Citizen.CreateThread loops.
- Avoid Wait(0) loops unless per-frame execution is actually required.
- Prefer event-driven logic over continuous polling.
- Clean up spawned entities, blips, peds, vehicles, and zones when they are no longer needed.
- Ensure resources properly handle player disconnects and resource restarts.
- Avoid unnecessary global state.
- Follow the existing framework conventions used by the resource.
- Do not mix QBCore, ESX, Qbox, or standalone patterns without a clear compatibility layer.