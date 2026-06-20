# Distributed Lock: Redis vs. Zookeeper

**Redis locks** use simple set operations (e.g., `SETNX` plus expiration) or Redisson. They are fast but do not guarantee safety in all edge cases (network partitions, clock drift). **Zookeeper locks** use persistent sequential znodes. Zookeeper provides strict ordering and automatic release on session expiration, making it more reliable for critical sections but with higher latency and complexity. Choose Redis for high throughput and Zookeeper for strong correctness.
