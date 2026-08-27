# Tests — Create Tests

Create or update tests for ExpenseLedger feature `{FEATURE_NAME}`.

Cover:
- Domain business rules.
- CQRS handler behavior.
- FluentValidation.
- API endpoint behavior.
- Authorization and not-found cases.
- Redis/cache behavior when applicable.
- Blazor component behavior when applicable.

Use the repository's existing test framework, fixtures, test data builders and naming conventions. Avoid duplicated infrastructure. Include success, validation, boundary, exception and cancellation scenarios where applicable. Return complete files with exact paths.