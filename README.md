# kafka_ecosystem
---

## 01. Understanding Kafka technologies 
---

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

Swarajits-MacBook-Air:cp-all-in-one swarajitroy$ ls
README.md		docker-compose.yml

Swarajits-MacBook-Air:cp-all-in-one swarajitroy$ docker-compose up -d

Creating network "cp-all-in-one_default" with the default driver

Pulling zookeeper (confluentinc/cp-zookeeper:6.0.0)...
6.0.0: Pulling from confluentinc/cp-zookeeper
Digest: sha256:5fdb4796cc354de1d1e06bab7acb7db967c389e00a5421afc58216f57606718d
Status: Downloaded newer image for confluentinc/cp-zookeeper:6.0.0

Pulling broker (confluentinc/cp-server:6.0.0)...
6.0.0: Pulling from confluentinc/cp-server
Digest: sha256:d5ba29dbd01ad6f8ebd7c83be89d4949c830b7d0d503d80b882ac739e7974067
Status: Downloaded newer image for confluentinc/cp-server:6.0.0

Pulling schema-registry (confluentinc/cp-schema-registry:6.0.0)...
6.0.0: Pulling from confluentinc/cp-schema-registry
Digest: sha256:447f6a3419f7473ff6e24bba84bfa82fe5a0d04be24c01d7b576055bbf58410c
Status: Downloaded newer image for confluentinc/cp-schema-registry:6.0.0

Pulling connect (cnfldemos/cp-server-connect-datagen:0.4.0-6.0.0)...
0.4.0-6.0.0: Pulling from cnfldemos/cp-server-connect-datagen
Digest: sha256:2fd272ffdd3b726583608c272496361fd6acf1ce15e3ec71637b7758c8b16c08
Status: Downloaded newer image for cnfldemos/cp-server-connect-datagen:0.4.0-6.0.0

Pulling ksqldb-server (confluentinc/cp-ksqldb-server:6.0.0)...
6.0.0: Pulling from confluentinc/cp-ksqldb-server
Digest: sha256:eb49c05247ce7e6ebf46067c9ea8a6e5297205f0a9d85a266bb991b351bbbb40
Status: Downloaded newer image for confluentinc/cp-ksqldb-server:6.0.0

Pulling control-center (confluentinc/cp-enterprise-control-center:6.0.0)...
6.0.0: Pulling from confluentinc/cp-enterprise-control-center
Digest: sha256:7093866d25b1a31aac38c53a681387547bf4e1db358e60c1dc15900b038f6354
Status: Downloaded newer image for confluentinc/cp-enterprise-control-center:6.0.0

Pulling ksqldb-cli (confluentinc/cp-ksqldb-cli:6.0.0)...
6.0.0: Pulling from confluentinc/cp-ksqldb-cli
Digest: sha256:069f9e99b8f9ebc240bbcbcb418587e947e394af66a736911c80839297cd7389
Status: Downloaded newer image for confluentinc/cp-ksqldb-cli:6.0.0

Pulling ksql-datagen (confluentinc/ksqldb-examples:6.0.0)...
6.0.0: Pulling from confluentinc/ksqldb-examples
Digest: sha256:84d44f038e6f5cc4efb4aa4c5efef6088b9a61b96f878fdcef3ae6a6c3b4412b
Status: Downloaded newer image for confluentinc/ksqldb-examples:6.0.0

Pulling rest-proxy (confluentinc/cp-kafka-rest:6.0.0)...
6.0.0: Pulling from confluentinc/cp-kafka-rest
Digest: sha256:1168da10a2b810b8025d9089ffc77a3817e8debafc38ace776e7e545b801ba3a
Status: Downloaded newer image for confluentinc/cp-kafka-rest:6.0.0


Creating zookeeper       ... done
Creating broker          ... done
Creating schema-registry ... done
Creating connect         ... done
Creating rest-proxy      ... done
Creating ksqldb-server   ... done
Creating control-center  ... done
Creating ksqldb-cli      ... done
Creating ksql-datagen    ... done

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
