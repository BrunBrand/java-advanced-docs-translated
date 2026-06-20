# Ensuring Message Order

Many messaging systems provide only at‑least‑once delivery. To preserve order:

- Partition messages by a **sharding key** (e.g., user ID) so that all related messages go to the same partition and are consumed sequentially.
- Use **single‑threaded consumption** for topics where order matters.

If ordering must be strict across partitions, you may need to sacrifice parallelism or implement ordering at the application layer.
