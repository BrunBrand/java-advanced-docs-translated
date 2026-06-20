# Principles of High Concurrency Design

Systems expecting heavy traffic must be designed to handle thousands or millions of requests per second. Key techniques include:

- **Caching** to serve hot data from memory rather than hitting the database【700207876182062†L82-L96】.
- **Asynchronous processing** via message queues to decouple services and smooth traffic【700207876182062†L36-L57】.
- **Database sharding and read/write separation** to distribute load across servers.
- **Rate limiting** and **circuit breaking** to prevent overload and cascading failures.

Combining these approaches improves throughput and resilience.
