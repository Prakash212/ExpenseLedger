# Refactor Component Prompt

Refactor an existing ExpenseLedger component without changing intended behavior.

- Inspect all usages before modifying the component API.
- Preserve backward compatibility unless the task explicitly allows a breaking change.
- Consolidate duplicated logic and CSS into the shared component.
- Prefer existing Ledger components over new equivalents.
- Preserve Light/Dark Notebook theme behavior.
- Keep scoped CSS owned by the reusable component.
- Validate responsive, accessibility and keyboard behavior.
- Update affected callers and tests when an API changes.
- Return complete files with exact repository paths when code is requested.
