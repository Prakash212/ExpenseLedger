# ExpenseLedger V2 — Coding Standards

## General
- Prefer clear, maintainable code over clever abstractions.
- Follow SOLID and dependency inversion.
- Keep methods focused and small.
- Avoid magic strings and unexplained constants.
- Use dependency injection and options where configuration is required.

## Async
- Use asynchronous APIs for I/O.
- Accept and propagate `CancellationToken` through application and infrastructure boundaries.
- Suffix asynchronous methods with `Async`.

## Validation
- Validate commands/requests with FluentValidation.
- Keep domain invariants in the Domain layer.
- Do not duplicate validation logic across UI and handlers unnecessarily.

## Errors
- Use consistent application errors/results.
- API failures use ProblemDetails.
- Do not leak stack traces or infrastructure details to clients.

## Logging
- Use structured Serilog logging.
- Include correlation/trace identifiers where available.
- Never log passwords, tokens, secrets, or sensitive personal data.

## Testing
- Unit test application/domain behavior.
- Add integration tests for persistence and API boundaries.
- Test cache invalidation and important authorization paths.

## UI
- Use shared Ledger components.
- Keep business logic out of Razor markup.
- Keep component CSS scoped.
- Preserve light/dark theme parity.
