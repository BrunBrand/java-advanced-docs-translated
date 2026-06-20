# Why Use Message Queues?

Message queues provide three major advantages:

1. **Decoupling** – producers and consumers operate independently. Producers send messages to the queue; consumers process them asynchronously【700207876182062†L36-L57】.
2. **Asynchronous processing** – tasks can be handled in the background, reducing user response times【700207876182062†L36-L57】.
3. **Peak‑shaving** – the queue absorbs traffic spikes and smooths out load over time【700207876182062†L67-L78】.

However, adding an MQ introduces complexity, such as ensuring message order, avoiding duplication and handling errors. Careful design of producers, brokers and consumers is necessary to reap the benefits.
