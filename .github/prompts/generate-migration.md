# Generate Migration Prompt

Create an EF Core migration for the requested ExpenseLedger schema change.

Before coding:
- Inspect the current DbContext and entity configurations.
- Check existing migrations and naming conventions.
- Preserve existing data and backward compatibility where possible.

Requirements:
- Correct relationships, indexes, constraints and delete behavior.
- No accidental destructive changes.
- Include the migration and model snapshot updates as required.
- Explain any data migration risk briefly.
- Provide complete files with exact paths when code is requested.
