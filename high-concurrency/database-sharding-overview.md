# Introduction to Database Sharding

To handle high read/write traffic, monolithic databases are broken into **shards**. Benefits include:

- **Improved concurrency** – many shards operate in parallel, allowing more transactions per second.
- **Isolation of failures** – problems on one shard do not affect others.
- **Capacity expansion** – more shards can be added to meet business growth.

Sharding adds complexity: cross‑shard transactions, global sorting and aggregation require additional logic. The following articles discuss dynamic expansion, global IDs and sharding methods.
