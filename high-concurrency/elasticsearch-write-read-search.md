# Elasticsearch Write, Query and Search

Elasticsearch supports:

- **Indexing** documents via `POST` or `PUT`. Documents are stored in shards and become searchable after a refresh interval.
- **Search** via the `_search` API with queries and filters. It returns hits, scores and aggregations.
- **Bulk operations** for high‑throughput indexing.

Because Elasticsearch is near real‑time, there can be a slight delay between writing and searching a document. Use the refresh API when immediate consistency is required.
