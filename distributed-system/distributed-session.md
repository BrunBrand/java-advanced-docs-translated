# Managing Sessions in a Distributed System

To share login sessions across multiple servers:

- **Sticky sessions** – use a load balancer that always routes a user to the same server. Simple but reduces fault tolerance.
- **Session replication** – replicate session data to all nodes. Ensures failover but may not scale.
- **Centralised storage** – store sessions in Redis or a database; all servers access the same store. Provides scalability and failover at the cost of extra network hops.

Session management should align with the system’s performance and availability requirements.
