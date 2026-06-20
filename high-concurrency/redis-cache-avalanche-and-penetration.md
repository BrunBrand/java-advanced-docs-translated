# Redis Cache Avalanche and Penetration

Cache failures can cause heavy load on the database:

- **Cache avalanche** – many keys expire simultaneously, causing a spike in database traffic. Randomise expiration times or use mutex locks to stagger expirations.
- **Cache penetration** – queries for non‑existent keys bypass the cache and hit the database. Use Bloom filters or cache nulls to prevent repeated misses【700207876182062†L82-L96】.
- **Hot key breakdown** – a single popular key expires and many requests go through to the database. Use logical expiration and proactive cache warming.

Mitigating these issues keeps the cache effective and protects the database.
