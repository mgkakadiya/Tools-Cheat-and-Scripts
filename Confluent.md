What is confluent cloud?

    Manage confluent kafka cluster
      cloud providers
        aws
        GCP
        Azure
    cluster Type
      Basic (shared)
        99.5 % up time
        
      Standard (shared)
      Enterprise (shared)
      Dedicated



      what is bootstrap-server in kafka config?
bootstrap.servers is a comma-separated list of host and port pairs that are the addresses of the Kafka brokers in a "bootstrap" Kafka cluster that a Kafka client connects to initially to bootstrap itself.
Kafka broker

A Kafka cluster is made up of multiple Kafka Brokers. Each Kafka Broker has a unique ID (number). Kafka Brokers contain topic log partitions. Connecting to one broker bootstraps a client to the entire Kafka cluster. For failover, you want to start with at least three to five brokers. A Kafka cluster can have, 10, 100, or 1,000 brokers in a cluster if needed.

more information: check this, official doc
http://cloudurable.com/blog/kafka-architecture/index.html
https://kafka.apache.org/documentation/


I acknowledge that SLA downgrades are not supported

Schema Registry
Schema Registry provides a centralized repository for managing and validating schemas for topic message data, and for serialization and deserialization of the data over the network. Producers and consumers to Kafka topics can use schemas to ensure data consistency and compatibility as schemas evolve. Schema Registry is a key component for data governance, helping to ensure data quality, adherence to standards, visibility into data lineage, audit capabilities, collaboration across teams, efficient application development protocols, and system performance.

