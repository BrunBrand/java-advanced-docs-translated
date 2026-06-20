# Building an Elasticsearch Production Cluster

A production cluster should include:

- **Multiple master nodes** (3 or 5) to avoid split‑brain.
- **Dedicated data nodes** sized according to indexing and query workload.
- **Shard allocation awareness** to distribute replicas across racks/availability zones.
- **Snapshot and restore** processes for backups.

Index design (shard count, mapping, lifecycle management) should be planned up front. Use monitoring tools (Kibana, Prometheus) to observe cluster health and perform capacity planning.
