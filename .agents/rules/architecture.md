---
trigger: always_on
---

# Architecture Rules

This project uses:

- Laravel 12
- PHP 8.4
- PostgreSQL
- Filament 4
- Tailwind CSS

Architecture Principles:

- Follow Laravel conventions whenever possible.
- Avoid over-engineering.
- Prefer Laravel native solutions before introducing third-party packages.
- Keep code modular and domain-oriented.
- Every feature must be self-contained.
- Use Service classes for business logic.
- Controllers should remain thin.
- Models should not contain complex business logic.

New features must respect this structure.

Always explain why a new package is needed before adding it.