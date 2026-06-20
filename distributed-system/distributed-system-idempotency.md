# Idempotency in Distributed Systems

An operation is **idempotent** if performing it multiple times has the same effect as performing it once. To achieve idempotency:

- Use **unique request IDs** and maintain a log of processed IDs.
- Implement **optimistic locking** with version numbers.
- Design APIs to be naturally idempotent (e.g., `PUT` to set a resource to a specific state).

Idempotency avoids duplicate effects when requests are retried due to failures.
