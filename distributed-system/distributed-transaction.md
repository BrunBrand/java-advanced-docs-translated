# Distributed Transactions

Coordinating a single transaction across multiple services is challenging. Common patterns:

- **Two‑Phase Commit (2PC)** – a coordinator asks each participant to prepare and then commit or rollback. Provides ACID semantics but can block during failures.
- **Try‑Confirm/Cancel (TCC)** – each service implements `Try`, `Confirm` and `Cancel` methods. Offers more flexibility and compensation.
- **Saga pattern** – break the transaction into a series of local transactions with compensating actions on failure.

Choose a pattern based on consistency requirements and failure tolerance.
