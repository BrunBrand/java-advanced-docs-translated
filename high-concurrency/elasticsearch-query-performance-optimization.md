# Optimising Elasticsearch Query Performance

To improve search efficiency:

- Use **filters** instead of queries** for conditions that do not affect scoring; filters are cached.
- Design **mappings** carefully: avoid using **text** type for fields that are never searched; disable `_source` if you never retrieve the original JSON.
- Limit the number of **shards** per node. Too many small shards increase overhead.
- Use **scroll** or **search after** for deep pagination rather than `from`/`size` parameters.

Monitoring cluster metrics (heap usage, query latency, indexing rate) and tuning according to workload is essential.
