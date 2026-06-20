# Database Sharding Methods

**Database sharding** splits a large dataset into multiple smaller pieces (shards) to improve throughput and scalability.

- **Vertical sharding** divides tables by functionality (e.g., user profile vs. orders). This reduces table size but can create hotspots if one table grows faster.
- **Horizontal sharding** divides rows across machines by a sharding key (e.g., user ID, timestamp). Each shard stores the same schema but different slices of data.
- **Hybrid** – a combination of vertical and horizontal sharding.

Good sharding strategies evenly distribute load, simplify routing and minimise cross‑shard joins.
