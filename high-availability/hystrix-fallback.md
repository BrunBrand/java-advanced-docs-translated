# Hystrix Fallback

When a Hystrix command fails (timeout, exception, circuit open), it can execute a **fallback** method. Fallbacks can:

- Return a default value or cached response.
- Route the request to an alternative service.
- Provide a user‑friendly error message.

Fallbacks keep the user experience consistent even during outages.
