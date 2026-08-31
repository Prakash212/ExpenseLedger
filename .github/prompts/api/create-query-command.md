# Create CQRS Command or Query

Implement `{RequestName}` for `{Feature}`.

Requirements:
- Place it under the correct Application feature folder.
- Use MediatR request/handler patterns already established in the solution.
- Commands may mutate state; queries must remain read-only.
- Use domain/application abstractions rather than concrete infrastructure dependencies.
- Add a FluentValidation validator when inputs require validation.
- Project only required fields for queries.
- Support CancellationToken.
- Add structured logging only where meaningful.
- Apply Redis caching for appropriate read-heavy queries and invalidate affected keys for commands.
- Add unit tests for handler and validator behavior.

Output exact paths and complete files.