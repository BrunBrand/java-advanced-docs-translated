# Dubbo SPI

The **Service Provider Interface (SPI)** in Dubbo allows developers to extend core functionality. By placing an implementation under `META-INF/dubbo` and declaring it in a configuration file, Dubbo loads it at runtime. SPI is used to plug in custom protocols, cluster strategies, filters and more.
