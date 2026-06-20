# Find the Top 100 Words

To find the 100 most frequent words in a huge text corpus, use the same approach as top‑k numbers: maintain a min‑heap of size 100 keyed by word frequency. Alternatively, use MapReduce with mappers counting word occurrences and reducers aggregating and selecting the top 100.
