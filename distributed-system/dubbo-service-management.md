# Dubbo Service Management

Service governance in Dubbo includes:

- **Service registration and discovery** – providers register their services with a registry (e.g., Zookeeper), consumers subscribe to changes.
- **Dynamic configuration** – configure provider parameters (timeouts, retries) via the registry.
- **Service grouping and versioning** – support multiple versions of a service concurrently.

These features make it easier to operate large microservice deployments.
