# Dubbo Operating Principle

Dubbo is a high‑performance RPC framework. Its architecture includes:

- **Provider** – exposes services.
- **Consumer** – invokes remote services.
- **Registry** – stores provider addresses; consumers subscribe to updates.
- **Monitor** – collects statistics for calls.

The consumer and provider communicate using an agreed protocol (e.g., Dubbo, REST) via the registry and network.
