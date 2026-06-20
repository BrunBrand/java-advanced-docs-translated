# Preserving Request Order

Some applications require requests to be processed in the order they were sent. Techniques include:

- Assigning **sequence numbers** to requests and buffering out‑of‑order messages until missing ones arrive.
- Using a **single primary** node to serialise operations.
- Partitioning by a key so that related operations go to the same node and maintain order.

Ordering guarantees often reduce throughput, so they should be applied only where necessary.
