# Redis Expiration Policies and LRU

When Redis reaches its memory limit, it evicts keys based on the configured **maxmemory-policy**:

- **noeviction** – returns an error when memory is exhausted.
- **allkeys-lru** – removes the least recently used keys.
- **volatile-lru** – LRU among keys with expiration.
- **allkeys-random/volatile-random** – evicts random keys.

Properly setting expiration times and choosing an eviction policy prevents memory issues and ensures important data stays in the cache.
