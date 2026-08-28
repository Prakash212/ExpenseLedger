# Create CQRS Command or Query Prompt

Implement `{RequestName}` for `{Feature}` using the existing ExpenseLedger CQRS/MediatR architecture.

Requirements:
- Place it under the correct Application feature folder.
- Use the existing MediatR request/handler patterns.
- Commands may mutate state; queries are read-only.
- Keep Domain/Application independent from infrastructure implementations.
- Add FluentValidation where needed.
- Project only required fields for queries.
- Support CancellationToken.
- Add Redis caching for suitable read-heavy queries and invalidate affected keys after successful commands.
- Add handler and validator tests.

Return exact paths and complete files.