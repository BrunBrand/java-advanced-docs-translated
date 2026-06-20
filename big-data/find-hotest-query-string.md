# Find the Hottest Query String

To find the most frequently searched query in a huge log, process the log in a streaming fashion and maintain a **hash map** of query counts. Alternatively, use a **min‑heap** to keep the top N queries in memory. In distributed environments, perform a MapReduce where mappers count queries in partitions and reducers aggregate the results.
