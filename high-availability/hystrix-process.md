# Hystrix Process

When a Hystrix command executes, the following steps occur:

1. **Check the circuit breaker state** – if open, immediately invoke the fallback.
2. **Obtain an execution permit** – from a thread pool or semaphore.
3. **Execute the run() method** – perform the remote call or computation.
4. **Record metrics** – latency, success/failure.
5. **Invoke fallback** – if the call times out or throws an exception.

This process isolates calls, enforces timeouts and collects metrics for circuit breaker decisions.
