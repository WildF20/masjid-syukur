---
trigger: always_on
---

# Security Rules

Always:

- Validate request input.
- Use Form Requests.
- Protect admin routes.
- Apply authorization policies.
- Escape user-generated content.

Never:

- Trust frontend validation.
- Expose sensitive configuration.
- Commit secrets.
- Store plaintext passwords.

Any security concern must be reported.