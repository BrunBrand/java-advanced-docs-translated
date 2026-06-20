# Find Common URLs

Given two huge files containing billions of URLs, find the URLs that appear in both. Solutions:

- **Hash partitioning** – split both files into N parts using a hash function, so that identical URLs end up in the same partition. Compare each pair of corresponding partitions by loading them into memory and using a hash set.
- **Bitset** – assign each URL an integer ID via hashing and mark presence in two bitsets, then compute their intersection.

This divide‑and‑conquer strategy avoids loading the entire dataset into memory【386122166985391†L14-L27】.
