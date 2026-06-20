# Redis Master–Slave Replication

Redis supports asynchronous replication. A **slave** connects to the **master**, performs an initial full sync and then receives a stream of write commands. Benefits:

- Separates read and write workloads.
- Provides redundancy for failover.

However, replication is asynchronous and slaves can lag behind the master. Use Redis Sentinel for automatic monitoring and failover.
