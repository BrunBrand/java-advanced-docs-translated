# Generating Global IDs for Sharded Databases

When data is distributed across many database shards, primary keys must be **globally unique**. Common strategies include:

- **UUIDs** – Universally Unique Identifiers can be generated without coordination, but they are long strings and have poor locality for index storage.
- **Snowflake algorithm** – A 64‑bit ID composed of timestamp, machine identifier and sequence number. It produces roughly ordered IDs and is widely used in distributed systems.
- **Segmented auto‑increment** – Allocate ID blocks to each shard, e.g., one shard generates keys ending in 0–9. This is simple but requires coordination when adding shards.

Choosing a suitable ID generation strategy prevents key collisions and ensures that objects can be moved between shards without changing their IDs.
