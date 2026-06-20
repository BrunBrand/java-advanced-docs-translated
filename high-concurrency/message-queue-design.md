# Message Queue Design

A message queue system typically consists of **producers**, **brokers** and **consumers**. Design considerations:

- **Topic vs. queue** semantics – topics allow publish/subscribe; queues provide point‑to‑point messaging.
- **Load balancing** – distribute messages evenly across consumers.
- **Acknowledgment and retry** – ensure messages are not lost and can be re‑delivered on failure.

Choosing an MQ depends on requirements for throughput, ordering, persistence and community support.
