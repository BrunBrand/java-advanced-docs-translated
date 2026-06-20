# Redis Rehashing

Redis uses **hash tables** to store dictionaries. When a table exceeds a certain load factor or shrinks, it resizes itself. To avoid blocking, Redis performs **incremental rehashing**:

- A second table is allocated and rehashing is spread across subsequent operations.
- Each normal operation moves a few buckets from the old table to the new table.

This ensures that rehashing does not block the server and keeps latency predictable.
