# Event‑Driven Data Management for Microservices

Microservices often maintain their own databases. To keep data consistent across services:

- Use **event sourcing** – persist events that represent state changes and rebuild state from them.
- Implement **CQRS** (Command Query Responsibility Segregation) – separate write and read models for scalability.
- Publish **domain events** when data changes; other services subscribe and react accordingly.

Event‑driven architectures promote loose coupling and eventual consistency.
