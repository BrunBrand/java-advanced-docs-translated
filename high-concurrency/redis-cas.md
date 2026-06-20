# Redis CAS (Check‑And‑Set)

Redis supports optimistic locking via the **WATCH** command. To update a value safely:

1. `WATCH` the key(s).
2. Read the current value and compute the new value.
3. Start a `MULTI`/`EXEC` transaction to set the new value.
4. If the key has changed since it was watched, the transaction will fail and can be retried.

This pattern implements a Compare‑And‑Swap (CAS) mechanism to avoid lost updates in concurrent environments.
