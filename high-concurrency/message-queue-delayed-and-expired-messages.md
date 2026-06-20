# Delayed and Expired Messages in MQ

Some use cases require messages to be delivered after a delay or to expire if not consumed:

- **Delayed messages** – broker stores the message until the delay time elapses. Some MQs support this natively (e.g., RabbitMQ with delayed exchange), otherwise implement a delay queue via a scheduler.
- **TTL (Time To Live)** – messages expire after a set time and are removed from the queue to avoid processing stale data.

Implementing delay and expiration requires careful configuration and monitoring to avoid message loss.
