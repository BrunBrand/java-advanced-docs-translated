# Find the Top 500 Numbers

To keep track of the top 500 largest numbers in a stream, maintain a **min‑heap** of size 500. For each incoming number:

1. If the heap has fewer than 500 elements, insert the number.
2. Otherwise, compare the number with the smallest element (root). If it is larger, replace the root and heapify.

At the end, the heap contains the top 500 numbers.
