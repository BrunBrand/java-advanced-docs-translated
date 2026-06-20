# Redis Consistency

Redis provides **eventual consistency** in master‑slave replication; writes are replicated asynchronously. To improve consistency:

- Use **WAIT** command to block until replicas have acknowledged the write.
- Enable **AOF** (Append Only File) persistence to avoid data loss.
- For strong consistency, use a single master or consider Raft‑based systems like Redis Raft.

Trade‑offs between consistency and performance should be chosen based on application needs.
