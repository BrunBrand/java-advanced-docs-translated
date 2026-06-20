# Hystrix Execution Isolation

Hystrix isolates dependencies so that failures in one service do not block others. Two isolation strategies:

- **Thread isolation** – each dependency call runs in its own thread pool, limiting the number of concurrent calls【22235231890149†L14-L58】.
- **Semaphore isolation** – for fast, non‑blocking calls, Hystrix uses a semaphore to control concurrency without the overhead of threads.

Isolation ensures that slow or failing dependencies cannot exhaust core resources.
