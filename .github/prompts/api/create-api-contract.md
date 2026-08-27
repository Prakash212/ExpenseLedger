# API — Create Contract

Create or update API request/response contracts for ExpenseLedger.

Requirements:
- Contracts are transport-safe and independent of EF entities.
- Use request DTOs for input and response DTOs for output.
- Define pagination/filter/sort contracts consistently across list endpoints.
- Preserve nullable/reference semantics explicitly.
- Avoid leaking domain or persistence implementation details.
- Keep contracts suitable for both Blazor and MAUI Android clients.
- Add validation and tests where appropriate.

Inspect existing contracts before creating duplicates. Return complete files with exact paths.
