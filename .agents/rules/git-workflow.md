---
trigger: always_on
---

# Git Workflow

Before implementation:

1. Analyze impact.
2. Identify affected modules.
3. Identify database changes.
4. Identify test changes.

After implementation:

1. Run formatter.
2. Run static analysis.
3. Run tests.
4. Verify API contracts.

Generate commit message:

type(scope): summary

Examples:

feat(program): add program management
fix(blog): handle missing thumbnail
refactor(donation): simplify payment flow