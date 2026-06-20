# Ensuring Message Queue High Availability

Message queues are a critical component. To avoid single points of failure:

- Deploy a **cluster** of brokers (e.g., RabbitMQ mirrored queues or Kafka with multiple brokers).
- Use **replication** so that messages are stored on multiple nodes.
- Enable **persistence** to disk and configure acknowledgment policies.
- Deploy clients with **failover** and **retry** logic to handle broker outages.

High availability ensures that message producers and consumers can continue to operate even when some nodes fail.
