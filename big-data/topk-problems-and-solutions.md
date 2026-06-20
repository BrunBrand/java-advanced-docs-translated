# Top‑K Problems and Solutions

The **Top‑K** problem seeks the K largest or smallest elements in a dataset. Common solutions:

- **Heap** – maintain a min‑heap of size K; works well for streaming data.
- **Quickselect** – partition the array so that the K largest elements are in one part; average time O(N).
- **Bucket counting** – if the value range is small, use counting sort to find top K.

Choosing a technique depends on data size, memory constraints and whether the data can be modified【386122166985391†L69-L77】.
