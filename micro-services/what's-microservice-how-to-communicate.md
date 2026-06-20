# What is a Microservice? How Do Services Communicate?

A microservice is a self‑contained unit that owns its data and implements a specific business capability. Services communicate using:

- **Synchronous protocols** – REST/HTTP or gRPC for request‑response interactions.
- **Asynchronous messaging** – message queues (Kafka, RabbitMQ) or event streaming for decoupled communication.
- **Service mesh** – infrastructure layer that handles communication concerns like retries, timeouts and observability.

Choosing the right communication pattern depends on coupling, latency and reliability requirements.
