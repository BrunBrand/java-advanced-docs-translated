# Sentinel vs. Hystrix

Both Alibaba **Sentinel** and Netflix **Hystrix** provide fault tolerance for microservices, but they differ:

- **Resource protection** – Sentinel focuses on flow control, rate limiting and circuit breaking at runtime, with a UI for configuration.
- **Programming model** – Hystrix wraps calls in commands via annotations or code; Sentinel uses API calls or integrates at the RPC framework level.
- **Current status** – Hystrix has entered maintenance mode; Sentinel is actively developed.

Choosing between them depends on ecosystem and feature requirements.
