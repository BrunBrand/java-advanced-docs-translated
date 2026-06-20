# Hystrix Request Cache

Hystrix can cache results within a single request context to avoid duplicate calls. When enabled:

- Subsequent calls with the same cache key return the cached response.
- Caching reduces latency and load on downstream services.
- The cache lives only for the lifetime of the request (e.g., an HTTP request).

Use request caching for idempotent operations to improve efficiency.
