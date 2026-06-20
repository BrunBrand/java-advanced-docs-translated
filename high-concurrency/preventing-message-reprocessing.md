# Preventing Message Reprocessing

To avoid consuming the same message multiple times:

- Assign a **unique ID** to each message and track processed IDs (e.g., in a database or cache) to achieve idempotent processing.
- Use the **exactly once** semantics offered by some MQs (e.g., Kafka’s consumer offsets).
- Employ transactional message patterns or two‑phase commit when messages coordinate with database transactions.

These methods ensure that messages are processed once even in the face of retries.
