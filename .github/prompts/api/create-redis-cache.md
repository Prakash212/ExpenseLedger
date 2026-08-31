# Create Redis Cache Prompt

Add Redis caching to the requested ExpenseLedger query or workflow.

Requirements:
- Inspect current cache abstractions and existing keys before adding anything.
- Define key naming, serialization, expiration and invalidation.
- Cache only read models or other data that is safe to cache.
- Do not place Redis dependencies in Domain.
- Invalidate cache only after the database mutation succeeds.
- Handle cache misses and temporary Redis failures according to existing application policy.
- Avoid cache stampede where the workload warrants protection.
- Add tests for hit, miss, invalidation and failure paths.
- Return complete files with exact paths when code is requested.
