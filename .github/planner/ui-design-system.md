# ExpenseLedger V2 — Notebook UI Design System

## Design Goal
ExpenseLedger uses a notebook-inspired finance interface with one shared component language across Dashboard, Expenses, Categories, Products, Product Groups, Reports, and future features.

## Light Theme
- Primary canvas: warm cream / paper.
- Surfaces: soft paper white / cream.
- Accent: Ledger blue.
- Success: emerald.
- Danger: muted brick red.
- Warning: amber.
- Shadows: soft paper depth.
- Borders: avoid visible hard borders unless required for accessibility or table separation.

## Dark Theme
- Primary canvas: midnight navy.
- Surfaces: deep navy / charcoal.
- Accent: Ledger blue with restrained gold highlights.
- Success: emerald.
- Danger: muted red.
- Shadows: soft, tight elevation; avoid large glow halos.

## Shared Interaction Language
- Hover should use subtle elevation and color refinement.
- Pressed state removes lift.
- Focus must remain keyboard-visible.
- Disabled state reduces emphasis without changing geometry.
- Avoid layout shift when validation appears.

## Layout Rules
- Consistent spacing tokens.
- Reusable controls own their visual CSS.
- Pages own only composition/layout.
- Search, page-size selection, pagination and action controls must look identical across CRUD pages.

## Approved Page Size Style
Use PS-02 Sharp:
- Button-like compact surface.
- Sharp/small corner radius.
- No visible border.
- Soft notification-like shadow.
- One-pixel hover lift.
- Arrow comfortably inset from the right edge.

## CRUD Action Style
Edit and Delete actions use the shared `LedgerButton` styles. Do not create page-specific edit/delete button CSS.

## Modal Rules
Use `LedgerDialog`. Keep form spacing stable before and after validation. Use shared Ledger inputs and selectors.

## Accessibility
- Preserve visible focus states.
- Use semantic buttons, labels, table headers, dialogs, and ARIA attributes where necessary.
- Do not use color as the only status signal.
