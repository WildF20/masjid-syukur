---
trigger: always_on
---

# Testing Rules

Every feature must include:

- Feature Test
- Integration Test when applicable

Requirements:

- Happy path
- Validation errors
- Authorization checks
- Edge cases

When changing:

- Database schema
- Seeder
- Policy
- Resource

Agent must evaluate whether tests need updates.

Never leave failing tests.