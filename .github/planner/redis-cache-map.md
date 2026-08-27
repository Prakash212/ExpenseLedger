# ExpenseLedger V2 — Redis Cache Map

## Purpose
Define cache ownership, keys, TTLs, and invalidation rules.

## Key Naming
Use:
`expensebook:{feature}:{scope}`

Examples:
- `expensebook:categories:all`
- `expensebook:productgroups:all`
- `expensebook:products:all`
- `expensebook:dashboard:summary`
- `expensebook:analytics:{period}`

## Cache Guidance
| Feature | Suggested policy |
|---|---|
| Categories | Cache until mutation invalidation |
| Product Groups | Cache until mutation invalidation |
| Products | Cache until mutation invalidation |
| Dashboard summary | Short TTL, e.g. 5 minutes |
| Expense analytics | Short/medium TTL, e.g. 10–30 minutes |

## Invalidation
- Create/Update/Delete Category -> invalidate categories and dependent dashboard summaries.
- Create/Update/Delete Product Group -> invalidate product groups and dependent product/catalog views.
- Create/Update/Delete Product -> invalidate products and dependent dashboard projections.
- Create/Update/Delete Expense -> invalidate dashboard, summaries, analytics, and any affected period/category cache.

## Rules
- Redis is a performance optimization, never the source of truth.
- Cache misses must execute the normal query path.
- Cache writes and invalidation must be resilient to transient Redis failures.
- Do not cache sensitive authentication tokens or secrets.
