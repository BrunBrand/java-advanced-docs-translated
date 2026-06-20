# Redis Persistence

Redis can persist data to disk using two mechanisms:

- **RDB snapshot** – dumps the dataset to a binary file at intervals. Fast loading but might lose recent writes.
- **AOF (Append Only File)** – logs every write command. Safer but slower to write and recover.
- **Hybrid persistence** – combines RDB and AOF.

Persistence ensures data durability when Redis restarts; choose a method based on performance and reliability needs.
