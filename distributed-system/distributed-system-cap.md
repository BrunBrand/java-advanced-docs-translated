# CAP Theorem

The CAP theorem states that a distributed system can only simultaneously provide two of the following three guarantees:

- **Consistency** – all nodes see the same data at the same time.
- **Availability** – every request receives a response (even if it might not contain the most recent data).
- **Partition tolerance** – the system continues to operate despite arbitrary network partitions.

In the presence of a partition, the system must choose between consistency and availability. Designs like MongoDB favour AP (availability and partition tolerance) while others like traditional RDBMS favour CP (consistency and partition tolerance).
