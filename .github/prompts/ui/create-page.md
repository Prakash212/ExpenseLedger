# UI — Create Page

Create or update a complete ExpenseLedger Blazor page.

Before coding, inspect existing pages and shared Ledger components.
Use reusable components before creating new ones.

Include where applicable:
- LedgerCard
- LedgerSearchBox
- LedgerPageSizeSelect
- LedgerPagination
- LedgerTable
- LedgerButton
- LedgerDialog
- LedgerConfirmDialog
- LedgerLoadingIndicator
- LedgerEmptyState
- LedgerToast

Rules:
- Preserve Clean Architecture boundaries.
- UI calls API clients only; never DbContext directly.
- Maintain Light/Dark Notebook theme parity.
- Use scoped CSS only for page composition.
- Do not duplicate shared component CSS.
- Validation must not cause layout shift.
- Preserve accessibility and responsive behavior.

Return complete files with exact paths when implementation is requested.
