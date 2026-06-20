# Elasticsearch Architecture

Elasticsearch builds on Lucene to provide a distributed, scalable search engine. An Elasticsearch **cluster** contains multiple **nodes** with different roles:

- **Master nodes** manage the cluster state and coordinate shard allocation.
- **Data nodes** store shards and handle CRUD operations and queries.
- **Ingest nodes** process data before indexing (optional).

Data is stored in **indices**, which are split into **shards**. Each shard has one or more **replicas** for fault tolerance. Cluster coordination ensures that primary and replica shards are balanced across nodes. Search requests are routed to the relevant shards, executed in parallel and merged【384982481536735†L4-L66】.
