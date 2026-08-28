# Create Dashboard Widget Prompt

Create a reusable ExpenseLedger dashboard widget.

Requirements:
- Define the widget data contract in Contracts/Application as appropriate.
- Implement CQRS query and MediatR handler for server-side data retrieval.
- Apply Redis caching when the data is suitable for caching and define invalidation rules.
- Expose a documented .NET 10 API endpoint.
- Build the Blazor widget with existing LedgerCard/stat/chart components.
- Support Light/Dark Notebook themes and responsive layouts.
- Handle loading, empty, error and refresh states.
- Keep chart rendering separated from data retrieval.
- Add tests for query, handler, endpoint and component behavior as appropriate.
- Return complete files with exact paths when code is requested.
