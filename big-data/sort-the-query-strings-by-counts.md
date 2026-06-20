# Sort Query Strings by Counts

Given a log of query strings and their counts, sort the queries by count in descending order. For large datasets, use external sorting: break the data into chunks that fit into memory, sort each chunk and merge them. In a distributed system, use MapReduce: mappers emit (count, query) pairs and reducers perform a distributed sort.
