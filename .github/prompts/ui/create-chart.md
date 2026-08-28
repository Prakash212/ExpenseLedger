# Create Chart Prompt

Create a reusable, accessible chart for ExpenseLedger.

- Inspect existing chart libraries and abstractions before adding dependencies.
- Prefer the existing charting approach in the repository.
- Query data through CQRS/API; never embed business/data-access logic in the UI.
- Support Light/Dark Notebook themes without changing chart semantics.
- Provide responsive sizing and readable labels/tooltips.
- Handle loading, empty and error states.
- Avoid excessive animation and respect reduced-motion preferences.
- Add tests around the data transformation/model where practical.
- Return complete files with exact paths when code is requested.
