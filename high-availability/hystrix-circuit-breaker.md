# Hystrix Circuit Breaker

A **circuit breaker** stops calling a remote service when failures exceed a threshold. It protects the system by

- **Open state** – if the error rate crosses a threshold, the circuit opens and calls fail immediately.
- **Half‑open** – after a timeout, a few test requests are allowed through. If they succeed, the circuit closes; otherwise it opens again.
- **Closed state** – normal operation; metrics are collected.

Circuit breakers prevent cascading failures and allow the system to recover quickly.
