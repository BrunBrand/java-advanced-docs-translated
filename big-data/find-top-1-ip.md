# Find the Most Frequent IP Address

To identify the IP address that appears most frequently in a log, use a hash map to count occurrences. For large logs distributed across machines, perform a MapReduce: mappers emit (IP, count) pairs and reducers aggregate counts. The IP with the highest count is the result.
