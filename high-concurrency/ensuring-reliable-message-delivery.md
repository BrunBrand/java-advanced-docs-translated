# Ensuring Reliable Message Delivery

Achieving reliable delivery means no message is lost:

- **Persistence** – ensure that messages are durably stored on disk before acknowledging producers.
- **Acknowledgments and re‑delivery** – if consumers fail, the broker can re‑deliver messages.
- **Transactions** – combine message publishing with database operations in a transactional way.

Different MQs provide different reliability guarantees; choose one that matches your requirements.
