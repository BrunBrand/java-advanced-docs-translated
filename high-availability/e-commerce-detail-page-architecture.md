# E‑Commerce Detail Page Architecture

For small e‑commerce sites, product detail pages can be pre‑generated as static HTML and served directly by Nginx. There is no dynamic computation and data is updated offline. Large e‑commerce platforms need to update details in real time and handle enormous traffic:

- **Event‑driven updates** – when a product changes, the update is sent to a message queue and processed by a background service that updates the cache (e.g., Redis).
- **Hierarchical caching** – Nginx caches static content; Redis caches product data; fallback to database only on cache miss.
- **Degradation** – if the cache is unavailable, serve a simplified page or placeholder.

This architecture ensures high availability and responsiveness【576842892942009†L4-L29】.
