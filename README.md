# kafka_ecosystem
---

## 00. Confluent Certified Developer for Apache Kafka
---

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

## 02. Understand Kafka Producers
---

## 03. Understand Kafka Consumers 
---

## 04. Understand Kafka Schema Registries
---

## 05. Understand Kafka Connnect 
---

## 06. Understand Kafka Streams
---
