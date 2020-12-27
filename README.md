# kafka_ecosystem
---

* https://docs.confluent.io/platform/current/tutorials/examples/clients/docs/java.html#client-examples-java
* https://www.confluent.io/learn/kafka-tutorial/

## 00. Confluent Certified Developer for Apache Kafka
---

* B. Development
   * [03. Performance, Throughput, Latency and Scaling](#03f-b03-development-performance-throughput-latency-and-scaling)
   * [04. Message ordering and delivery guarantees](#03a-b04-development-message-ordering-and-delivery-guarantees)
   * [06.Producer Partition Selection](#03b-b06-development-producer-partition-selection)
   * [07. Consumer Offset management](#03c-b07-development-consumer-offset-management)
   * [08. Consumer groups, partition assignments, partition rebalances](#03d-b08-development-consumer-groups-partition-assignments-partition-rebalances)
   * [10. Topic Co-partitioning](#03e-b10-development-topic-co-partitioning-log-compacted-topics)


| ID | Domain | Task
| ----------- | ----------- | ------ |
| A.01 | Application design  | Kafka command line tools |
| A.02 | Application design  | Pub Sub and Streaming |
| A.03 | Application design  | Overall Apache Kafka architecture and design |
| A.04 | Application design  | Apache Kafka APIs, configuration and metrics |
| A.05 | Application design  | Message Metadata |
| A.06 | Application design  | System Metrics |
| A.07 | Application design  | Kafka Message Key selection (choices and factors) |
| B.01 | Development         | Kafka Clients - Producer & Consumer, concepts and functions |
| B.02 | Development         | Client Troubleshooting & Debugging|
| B.03 | Development         | Performance, Throughput, Latency and Scaling |
| B.04 | Development         | Message ordering and delivery guarantees |
| B.05 | Development         | Serialization and Deserialization |
| B.06 | Development         | Producer Partition selection |
| B.07 | Development         | Consumer Offset management |
| B.08 | Development         | Consumer groups, partition assignments, partition rebalances |
| B.09 | Development         | Data retention strategies and implication |
| B.10 | Development         | Topic Co-partitioning, Log compacted Topics |
| C.01 | Deployment/Testing | Application deployment choices| 
| C.02 | Deployment/Testing | Securing your data| 
| C.03 | Deployment/Testing | Monitoring & troubeshooting clients|
| C.04 | Deployment/Testing | client tuning |
| C.05 | Deployment/Testing | Kafka Streams application |
| C.06 | Deployment/Testing | KSQL and ksqlDB use cases |

## 01. Understanding Kafka technologies 
---

https://kafka-tutorials.confluent.io/
https://www.confluent.io/learn/kafka-tutorial/

One of the best way to do it is via https://docs.confluent.io/platform/current/quickstart/ce-docker-quickstart.html or https://docs.confluent.io/platform/current/quickstart/cos-docker-quickstart.html - an all in one platform - which installs the following

- Kafka Zookeeper
- Kakfa Brokers
- REST Proxy
- Schema Registry 
- Kafka Connect 
- KSQL DB Server 
- KSQL DB CLI 
- Confluenct Control Center (only for confluent, not for open source)

```

Swarajits-MacBook-Air:docker-compose swarajitroy$ git clone git@github.com:confluentinc/cp-all-in-one.git
Cloning into 'cp-all-in-one'...
remote: Enumerating objects: 30, done.
remote: Counting objects: 100% (30/30), done.
remote: Compressing objects: 100% (26/26), done.
remote: Total 723 (delta 15), reused 14 (delta 4), pack-reused 693
Receiving objects: 100% (723/723), 4.16 MiB | 2.66 MiB/s, done.
Resolving deltas: 100% (361/361), done.

Use the cp-all-in-one file,  /Users/swarajitroy/KAFKA_ECOSYSTEM/docker-compose/cp-all-in-one/cp-all-in-one

Swarajits-MacBook-Air:cp-all-in-one-community swarajitroy$ ls
README.md		docker-compose.yml

Swarajits-MacBook-Air:cp-all-in-one-community swarajitroy$ docker-compose up -d


Swarajits-MacBook-Air:cp-all-in-one-community swarajitroy$ docker-compose ps
     Name                    Command                  State                                        Ports
------------------------------------------------------------------------------------------------------------------------------------------
broker            /etc/confluent/docker/run        Up             0.0.0.0:29092->29092/tcp, 0.0.0.0:9092->9092/tcp, 0.0.0.0:9101->9101/tcp
connect           /etc/confluent/docker/run        Up (healthy)   0.0.0.0:8083->8083/tcp, 9092/tcp
ksql-datagen      bash -c echo Waiting for K ...   Exit 1
ksqldb-cli        /bin/sh                          Up
ksqldb-server     /etc/confluent/docker/run        Up             0.0.0.0:8088->8088/tcp
rest-proxy        /etc/confluent/docker/run        Up             0.0.0.0:8082->8082/tcp
schema-registry   /etc/confluent/docker/run        Up             0.0.0.0:8081->8081/tcp
zookeeper         /etc/confluent/docker/run        Up             0.0.0.0:2181->2181/tcp, 2888/tcp, 3888/tcp

```

## 02. Understand Kafka Security
---

## 03. Understand Kafka Producers & Consumers 
---


### 03.A B.04 Development (Message ordering and delivery guarantees)
---

- https://medium.com/@felipedutratine/kafka-ordering-guarantees-99320db8f87f
- https://supergloo.com/kafka/kafka-architecture-delivery/
- https://www.instaclustr.com/a-visual-understanding-to-ensuring-your-kafka-data-is-literally-in-order/


### 03.B B.06 Development (Producer Partition selection)
---

- https://www.confluent.io/blog/apache-kafka-producer-improvements-sticky-partitioner/
- https://blog.newrelic.com/engineering/effective-strategies-kafka-topic-partitioning/
- https://www.logicbig.com/tutorials/misc/kafka/using-keys-for-partition-assignment.html
- https://dzone.com/articles/kafka-producer-architecture-picking-the-partition#

### 03.C B.07 Development (Consumer Offset management)
---

- https://docs.confluent.io/platform/current/clients/consumer.html


### 03.D B.08 Development (Consumer groups, partition assignments, partition rebalances)
---

- https://dzone.com/articles/understanding-kafka-consumer-groups-and-consumer-l
- https://dzone.com/articles/understanding-kafka-consumer-groups-and-consumer-l-1
- https://medium.com/streamthoughts/understanding-kafka-partition-assignment-strategies-and-how-to-write-your-own-custom-assignor-ebeda1fc06f3
- https://medium.com/streamthoughts/apache-kafka-rebalance-protocol-or-the-magic-behind-your-streams-applications-e94baf68e4f2


### 03.E B.10 Development (Topic Co-partitioning, Log compacted Topics)
---

- https://blog.newrelic.com/engineering/effective-strategies-kafka-topic-partitioning/
- https://medium.com/xebia-france/kafka-streams-co-partitioning-requirements-illustrated-2033f686b19c
- https://towardsdatascience.com/log-compacted-topics-in-apache-kafka-b1aa1e4665a7

### 03.F B.03 Development (Performance, Throughput, Latency and Scaling)
---

- https://www.confluent.io/blog/kafka-fastest-messaging-system/
- https://www.confluent.io/blog/configure-kafka-to-minimize-latency/
- https://www.confluent.io/white-paper/optimizing-your-apache-kafka-deployment/
- https://www.datadoghq.com/blog/monitoring-kafka-performance-metrics/
- https://blog.newrelic.com/engineering/kafka-best-practices/

## 04. Understand Kafka Schema Registries
---

## 05. Understand Kafka Connnect 
---

## 06. Understand Kafka Streams
---


- https://www.confluent.io/blog/secure-kafka-deployment-best-practices/
- https://medium.com/@stephane.maarek/introduction-to-apache-kafka-security-c8951d410adf
