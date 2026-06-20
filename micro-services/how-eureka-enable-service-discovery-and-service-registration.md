# Service Discovery with Eureka

Netflix **Eureka** is a service registry. Architecture:

- **Eureka server** – maintains a registry of service instances.
- **Service registration** – services send heartbeats to the server to remain in the registry.
- **Service discovery** – clients query the server to find available service instances.

Eureka is often paired with Ribbon (client‑side load balancing) and Hystrix (fault tolerance) to build resilient microservices.
