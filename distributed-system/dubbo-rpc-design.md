# Dubbo RPC Design

Dubbo’s RPC model features:

- **Proxy** generation – consumers call a local proxy that hides remote invocation.
- **Protocol abstraction** – supports multiple protocols (Dubbo, HTTP, gRPC).
- **Filter chain** – allows plugins for logging, authentication and metrics.
- **Serialization** – pluggable codecs for data formats.

This design decouples interface, transport and serialization.
