# Redis Cluster

Redis Cluster partitions data across multiple nodes. Key points:

- The **key space** is divided into 16,384 **hash slots**; each node owns a set of slots.
- Each master has one or more **slave** nodes for replication.
- The cluster uses a **gossip protocol** to maintain membership and coordinate failover.
- Clients compute the slot of a key and send commands directly to the correct node.

Cluster mode provides automatic sharding and failover, enabling Redis to scale horizontally.
