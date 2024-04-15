# Spring Boot Kafka Reactive Project

This is a sample Spring Boot project that demonstrates the integration of Kafka with a Spring Reactive application. The project showcases key concepts related to Kafka, including topics, partitions, serialization, consumer groups, and offset management.

Start a ZooKeeper server:
```bash
bin/zookeeper-server-start.sh config/zookeeper.properties
```

Start a Kafka broker:
```bash
bin/kafka-server-start.sh config/server.properties
```

1. **Producer Project:**
   The producer project leverages the **Spring Boot Reactive framework** to extract a data stream from [Wikimedia Recent Changes](https://stream.wikimedia.org/v2/stream/recentchange). This project is designed to efficiently read the streaming data and subsequently transmit the messages to a Kafka broker.

2. **Consumer Project:**
   The consumer project complements the aforementioned producer by retrieving messages from the Kafka topic. The retrieved messages are then persisted into a DynamoDB database. This dual-project configuration not only demonstrates the integration of Spring Boot Reactive with Kafka for real-time data processing but also showcases the seamless storage of this data in a DynamoDB database, emphasizing end-to-end functionality within the application.

# Kafka-SpringBoot-Application
