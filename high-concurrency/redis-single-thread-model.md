# Redis Single‑Threaded Model

Redis uses a single thread for command execution but is highly efficient because:

- All data is in memory; operations do not block on disk I/O.
- It uses the **epoll/kqueue** event mechanism to multiplex connections.
- CPU caches are used effectively without the overhead of locks.

The single‑threaded design simplifies concurrency and achieves high throughput.
