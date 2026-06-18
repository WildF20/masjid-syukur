---
trigger: always_on
---

# Coding Standard

General:

- Use strict typing.
- Use PHPStan-friendly code.
- Follow PSR-12.
- Use constructor property promotion.
- Prefer enums over string constants.
- Prefer readonly where applicable.

Naming:

- Classes: PascalCase
- Methods: camelCase
- Variables: camelCase
- Database tables: snake_case plural
- Columns: snake_case

Avoid:

- Magic strings
- Duplicate logic
- Dead code
- Unused imports

Always refactor repeated logic.