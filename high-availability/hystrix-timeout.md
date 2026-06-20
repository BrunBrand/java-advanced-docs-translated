# Hystrix Timeout

Setting a timeout for remote calls prevents threads from waiting indefinitely. Hystrix monitors the execution time; if it exceeds the configured threshold, the call is aborted and fallback logic is executed. Timeouts should be tuned based on the expected latency of the dependency.
