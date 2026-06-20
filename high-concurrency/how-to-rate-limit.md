# Rate Limiting Techniques

Rate limiting protects services from overload:

- **Fixed window counter** – simple but can cause bursts at window edges.
- **Sliding window** – tracks requests over a moving time window.
- **Leaky bucket** – processes requests at a constant rate; excess requests are queued or dropped.
- **Token bucket** – tokens accumulate at a steady rate; requests consume tokens.

Implement rate limiting at API gateways or service level to smooth traffic and prevent abuse.
