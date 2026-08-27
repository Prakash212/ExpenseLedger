# Create Repository Prompt

Create a repository abstraction only when the existing architecture genuinely requires one.

- Inspect Persistence and Application interfaces first.
- Keep interfaces in the appropriate inner layer and implementations in Persistence/Infrastructure.
- Expose query methods that match application use cases rather than leaking EF IQueryable broadly.
- Support CancellationToken.
- Keep transactions and persistence concerns out of Domain/Application business rules.
- Add tests using the repository's existing database testing strategy.
- Do not introduce a generic repository merely for abstraction's sake.
- Return complete files with exact paths when code is requested.
