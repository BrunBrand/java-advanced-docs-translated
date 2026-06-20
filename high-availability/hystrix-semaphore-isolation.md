# Hystrix Semaphore Isolation

Semaphore isolation limits concurrent requests using a counting semaphore rather than a thread pool. It is suitable for low‑latency, non‑blocking calls. Advantages:

- Lower overhead compared to thread pools.
- Fast failure when the semaphore is exhausted.

However, blocking calls within semaphore isolation can still tie up the calling thread.
