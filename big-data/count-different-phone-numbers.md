# Count Different Phone Numbers

Given a huge file of phone numbers, count how many distinct numbers exist. A common approach is to use a **bitset** (bitmap). For example, to store 11‑digit phone numbers, allocate a bit array of size equal to the number range; set the bit when a number appears. The number of set bits equals the number of distinct phone numbers. For very large ranges, use a **Bloom filter** or partition the data into smaller chunks.
