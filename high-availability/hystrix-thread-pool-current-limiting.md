# Hystrix Thread Pool Current Limiting

Hystrix uses **thread pools** to isolate calls. By configuring the pool size and queue length, you control the maximum concurrency. If the queue is full and the pool is saturated, additional calls are rejected and fallback logic executes. This prevents dependency failures from exhausting server threads【22235231890149†L14-L58】.
