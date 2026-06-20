# Dynamic Database Shard Expansion

Large systems often start with a small number of database shards and need to expand capacity later. **Dynamic expansion** means adding new shards while the system is running, without stopping service. Key considerations:

- **Vertical vs. horizontal scaling** – vertical sharding splits tables by function, while horizontal sharding splits data by user ID or time. Horizontal sharding usually needs dynamic expansion.
- **Data migration** – when new shards are added, old data must be gradually moved to the correct shard. Use double‑write and ensure data consistency during migration.
- **Routing rules** – update the shard routing algorithm to recognise new shards. Use a consistent hashing or a routing table so that only a portion of the keys move【700207876182062†L36-L57】.
- **Global IDs** – generate globally unique IDs (see the ID generation article) so that records can move between shards without conflicts.

These techniques allow a database cluster to grow with business volume while minimising downtime and ensuring data integrity.
