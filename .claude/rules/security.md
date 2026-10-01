---
paths:
  - "**/*"
---

# Security Rules

- Never hardcode secrets, API keys, passwords, tokens, or private credentials.
- Never expose server credentials to client-side code.
- Never trust client-provided permissions, prices, identifiers, or ownership information.
- Validate authorization on the server.
- Validate input at system boundaries.
- Sanitize data before displaying it in HTML.
- Avoid dynamic code execution unless explicitly required.
- Do not introduce eval-like functionality without a clear justification.
- Do not log passwords, tokens, API keys, or sensitive personal information.
- Do not weaken authentication or authorization checks to make development easier.
- Do not disable security checks merely to bypass an error.
- Keep sensitive configuration in environment variables or server-side configuration.