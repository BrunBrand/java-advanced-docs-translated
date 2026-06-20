# Dubbo Load Balancing

Dubbo provides several load balancing strategies:

- **Random** – selects a provider randomly; suitable when providers have similar capabilities.
- **Round Robin** – rotates through providers equally.
- **Least Active** – selects the provider with the fewest active calls.
- **Consistent Hashing** – routes requests with the same parameters to the same provider, ensuring session stickiness.

Choosing the right strategy depends on the service characteristics.
