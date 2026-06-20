# Check If a Number Exists

To determine whether a given number exists in a massive dataset, use a **bitset** where each bit represents a potential number. Alternatively, partition the data into buckets based on hash values and scan only the relevant bucket. Bloom filters can provide probabilistic membership checks with low memory usage.
