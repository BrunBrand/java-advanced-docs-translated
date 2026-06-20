# Redis Sentinel

**Sentinel** is a system built into Redis for monitoring and automatic failover. Features:

- **Monitoring** – checks master and slave instances to detect failures.
- **Notification** – alerts clients when a problem is detected.
- **Automatic failover** – promotes a slave to master when the master fails.

Sentinel runs as a separate process and is usually deployed in clusters for high availability.
