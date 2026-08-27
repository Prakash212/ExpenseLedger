# ExpenseLedger V2 — Ledger Component Map

## Shared UI Components
- `LedgerCard` — page and content surface.
- `LedgerButton` — application actions.
- `LedgerButtonGroup` — grouped actions.
- `LedgerTextBox` — text entry.
- `LedgerSelect` — form selection.
- `LedgerDialog` — modal foundation.
- `LedgerPagination` — paging controls and summary.
- `LedgerPageSizeSelect` — shared page-size selector.
- `LedgerSearchBox` — shared listing search control.
- `LedgerStatusBadge` — status presentation.
- `LedgerEmptyState` — empty results.
- `LedgerLoadingIndicator` — loading state.
- `AppConfirmDialog` / `LedgerConfirmDialog` — confirmation workflow.
- `LedgerToast` / `NotificationService` — transient notifications.

## Composition Rules
Listing pages should compose shared controls rather than create local equivalents.

```text
Listing Page
  -> LedgerCard
     -> Toolbar
        -> Summary
        -> LedgerSearchBox
        -> LedgerPageSizeSelect
        -> LedgerButton
     -> LedgerTable
        -> LedgerStatusBadge
        -> LedgerButton
     -> LedgerPagination
```

## Ownership
Reusable behavior and visual treatment belong to the component. Page CSS should only handle page-specific layout and composition.

## Theme
All components consume shared CSS custom properties. Components must work in both Notebook Light and Notebook Dark themes without page-specific overrides.
