# Dubbo Serialization Protocol

Dubbo supports various serialization protocols:

- **Hessian2** – binary format with good performance and cross‑language support.
- **Kryo** – fast serialization library for Java objects.
- **Protobuf** – compact and language‑neutral but requires schema definitions.
- **Java native serialization** – convenient but slow and insecure.

Selecting the right protocol affects performance and interoperability.
