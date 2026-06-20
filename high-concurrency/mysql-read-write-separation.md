# MySQL Read/Write Separation

To handle more reads than writes, deploy a **master‑slave** setup: the master handles writes and slaves handle reads. A **proxy** or **middleware** routes read queries to slaves and write queries to the master. Considerations:

- **Replication lag** – writes may not immediately appear on slaves; critical reads should go to the master.
- **Consistency** – set the appropriate consistency level for your application.
- **Failover** – detect master failure and promote a slave.

This architecture improves read throughput but requires careful management【384982481536735†L73-L80】.
