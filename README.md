# Awesome Kafka Resources [![Awesome](https://img.shields.io/badge/AWESOME-%F0%9F%91%93-blue)](https://github.com/rbaddam)

A curated list of awesome Kafka tools and resources.


## Contents

- [Tools and Libraries](#tools-and-libraries)
  - [Command Line Tools](#command-line-tools)
  - [Cluster Provisioning](#cluster-provisioning)
  - [Automation and CI/CD](#automation-and-cicd)
  - [Cluster Resources Management](#cluster-resources-management)
  - [Secrets Management](#secrets-management)
  - [Networking](#networking)
  - [Storage and KRaft](#storage-and-kraft)
  - [Testing and Troubleshooting](#testing-and-troubleshooting)
  - [Monitoring, Alerts, and Visualization](#monitoring-alerts-and-visualization)
  - [Backup and Restore](#backup-and-restore)
  - [Security and Compliance](#security-and-compliance)
  - [Development Tools](#development-tools)
  - [Data Processing and Machine Learning](#data-processing-and-machine-learning)
  - [Miscellaneous](#miscellaneous)
- [Guides, Documentations, Blogs, and Learnings](#guides-documentations-blogs-and-learnings)
  - [Guides](#guides)
  - [Blogs and Videos](#blogs-and-videos)
  - [Learnings and Documentations](#learnings-and-documentations)
- [Anti-Patterns and Common Mistakes](#anti-patterns-and-common-mistakes)
- [Real-World Patterns and Best Practices](#real-world-patterns-and-best-practices)
- [Tool Comparison Tables](#tool-comparison-tables)
- [Contribute](#contribute)
- [License](#license)

---

## Tools and Libraries

Items with :green_heart: indicate open source projects.

### Command Line Tools

- :green_heart:[Apache Kafka (CLI tools)](https://github.com/apache/kafka)
  ![Stars](https://img.shields.io/github/stars/apache/kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/kafka?style=social)
  - The official Kafka repo (includes `kafka-topics`, `kafka-consumer-groups`, `kafka-producer-perf-test`, etc).

- :green_heart:[kcat (kafkacat)](https://github.com/edenhill/kcat)
  ![Stars](https://img.shields.io/github/stars/edenhill/kcat?style=social)
  ![Forks](https://img.shields.io/github/forks/edenhill/kcat?style=social)
  - Swiss army knife for Kafka: produce/consume/metadata/bench.

- :green_heart:[kafkactl](https://github.com/deviceinsight/kafkactl)
  ![Stars](https://img.shields.io/github/stars/deviceinsight/kafkactl?style=social)
  ![Forks](https://img.shields.io/github/forks/deviceinsight/kafkactl?style=social)
  - CLI admin tool (topics, ACLs, consumer groups).

- :green_heart:[kaf](https://github.com/birdayz/kaf)
  ![Stars](https://img.shields.io/github/stars/birdayz/kaf?style=social)
  ![Forks](https://img.shields.io/github/forks/birdayz/kaf?style=social)
  - Modern CLI for Kafka (topic browse, tail, groups, etc).

- :green_heart:[Kafka Tool (kafka-tools)](https://github.com/linkedin/kafka-tools)
  ![Stars](https://img.shields.io/github/stars/linkedin/kafka-tools?style=social)
  ![Forks](https://img.shields.io/github/forks/linkedin/kafka-tools?style=social)
  - LinkedIn’s misc CLI tools (admin / ops helpers).

### Cluster Provisioning

- :green_heart:[Strimzi (Kafka Operator)](https://github.com/strimzi/strimzi-kafka-operator)
  ![Stars](https://img.shields.io/github/stars/strimzi/strimzi-kafka-operator?style=social)
  ![Forks](https://img.shields.io/github/forks/strimzi/strimzi-kafka-operator?style=social)
  - The go-to Kafka-on-Kubernetes operator for most people.

- :green_heart:[Strimzi Drain Cleaner](https://github.com/strimzi/drain-cleaner)
  ![Stars](https://img.shields.io/github/stars/strimzi/drain-cleaner?style=social)
  ![Forks](https://img.shields.io/github/forks/strimzi/drain-cleaner?style=social)
  - Zero-downtime node draining for Kafka on Kubernetes.

- :green_heart:[Bitnami Kafka Helm Chart](https://github.com/bitnami/charts/tree/main/bitnami/kafka)
  ![Stars](https://img.shields.io/github/stars/bitnami/charts?style=social)
  ![Forks](https://img.shields.io/github/forks/bitnami/charts?style=social)
  - “Just give me Kafka on k8s” chart (widely used).

- :green_heart:[Redpanda Operator](https://github.com/redpanda-data/redpanda-operator)
  ![Stars](https://img.shields.io/github/stars/redpanda-data/redpanda-operator?style=social)
  ![Forks](https://img.shields.io/github/forks/redpanda-data/redpanda-operator?style=social)
  - If you’re running Kafka-compatible Redpanda.

- :green_heart:[Confluent for Kubernetes (CFK)](https://github.com/confluentinc/confluent-kubernetes-examples)
  ![Stars](https://img.shields.io/github/stars/confluentinc/confluent-kubernetes-examples?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/confluent-kubernetes-examples?style=social)
  - Practical CFK examples (the operator itself is not fully OSS).

- :green_heart:[k3d + Kafka (dev clusters)](https://github.com/k3d-io/k3d)
  ![Stars](https://img.shields.io/github/stars/k3d-io/k3d?style=social)
  ![Forks](https://img.shields.io/github/forks/k3d-io/k3d?style=social)
  - Handy for spinning local k8s + Kafka stacks fast.

### Automation and CI/CD

- :green_heart:[Terraform Provider: Confluent](https://github.com/confluentinc/terraform-provider-confluent)
  ![Stars](https://img.shields.io/github/stars/confluentinc/terraform-provider-confluent?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/terraform-provider-confluent?style=social)
  - Provision Confluent Cloud stuff with Terraform.

- :green_heart:[Kafka Docker Images (Bitnami)](https://github.com/bitnami/containers/tree/main/bitnami/kafka)
  ![Stars](https://img.shields.io/github/stars/bitnami/containers?style=social)
  ![Forks](https://img.shields.io/github/forks/bitnami/containers?style=social)
  - Widely used Kafka images for CI/dev.

- :green_heart:[Confluent Platform Images](https://github.com/confluentinc/cp-docker-images)
  ![Stars](https://img.shields.io/github/stars/confluentinc/cp-docker-images?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/cp-docker-images?style=social)
  - Confluent’s Docker setup (common in CI and demos).

### Cluster Resources Management

- :green_heart:[CMAK (Cluster Manager for Apache Kafka)](https://github.com/yahoo/CMAK)
  ![Stars](https://img.shields.io/github/stars/yahoo/CMAK?style=social)
  ![Forks](https://img.shields.io/github/forks/yahoo/CMAK?style=social)
  - Old but still everywhere. UI for brokers/topics/partitions. ⚠️ Maintenance has slowed. :contentReference[oaicite:1]{index=1}

- :green_heart:[Kafka UI](https://github.com/provectus/kafka-ui)
  ![Stars](https://img.shields.io/github/stars/provectus/kafka-ui?style=social)
  ![Forks](https://img.shields.io/github/forks/provectus/kafka-ui?style=social)
  - Web UI for managing clusters, topics, consumer groups, schemas, connect, etc.

- :green_heart:[AKHQ](https://github.com/tchiotludo/akhq)
  ![Stars](https://img.shields.io/github/stars/tchiotludo/akhq?style=social)
  ![Forks](https://img.shields.io/github/forks/tchiotludo/akhq?style=social)
  - Kafka GUI with good coverage (topics, groups, schema registry, connect). :contentReference[oaicite:2]{index=2}

- :green_heart:[Kafdrop](https://github.com/obsidiandynamics/kafdrop)
  ![Stars](https://img.shields.io/github/stars/obsidiandynamics/kafdrop?style=social)
  ![Forks](https://img.shields.io/github/forks/obsidiandynamics/kafdrop?style=social)
  - Lightweight UI: browse topics, partitions, consumer groups, messages.

- :green_heart:[Redpanda Console (Kowl)](https://github.com/redpanda-data/console)
  ![Stars](https://img.shields.io/github/stars/redpanda-data/console?style=social)
  ![Forks](https://img.shields.io/github/forks/redpanda-data/console?style=social)
  - One of the best OSS web consoles right now (Kafka-compatible).

- :green_heart:[Confluent Control Center (docs)](https://docs.confluent.io/platform/current/control-center/index.html)
  - Not OSS, but widely used in Confluent shops.

- [Kpow](https://kpow.io/)
  - Commercial UI/operations tool, popular in enterprise environments.

### Secrets Management

- :green_heart:[Strimzi OAuth](https://github.com/strimzi/strimzi-kafka-oauth)
  ![Stars](https://img.shields.io/github/stars/strimzi/strimzi-kafka-oauth?style=social)
  ![Forks](https://img.shields.io/github/forks/strimzi/strimzi-kafka-oauth?style=social)
  - OAuth/OIDC for Kafka on k8s (common in real setups).

- :green_heart:[HashiCorp Vault](https://github.com/hashicorp/vault)
  ![Stars](https://img.shields.io/github/stars/hashicorp/vault?style=social)
  ![Forks](https://img.shields.io/github/forks/hashicorp/vault?style=social)
  - Typical place to store SASL creds, keystores, connector secrets, etc.

- :green_heart:[External Secrets Operator](https://github.com/external-secrets/external-secrets)
  ![Stars](https://img.shields.io/github/stars/external-secrets/external-secrets?style=social)
  ![Forks](https://img.shields.io/github/forks/external-secrets/external-secrets?style=social)
  - Keep Kafka secrets out of manifests, sync from secret stores.

### Networking

- :green_heart:[Kafka Proxy](https://github.com/grepplabs/kafka-proxy)
  ![Stars](https://img.shields.io/github/stars/grepplabs/kafka-proxy?style=social)
  ![Forks](https://img.shields.io/github/forks/grepplabs/kafka-proxy?style=social)
  - Proxy Kafka connections via SOCKS/HTTP, k8s-friendly. :contentReference[oaicite:4]{index=4}

- :green_heart:[Strimzi Kafka Bridge](https://github.com/strimzi/strimzi-kafka-bridge)
  ![Stars](https://img.shields.io/github/stars/strimzi/strimzi-kafka-bridge?style=social)
  ![Forks](https://img.shields.io/github/forks/strimzi/strimzi-kafka-bridge?style=social)
  - HTTP bridge for Kafka (REST-ish producing/consuming).

- :green_heart:[Confluent REST Proxy](https://github.com/confluentinc/kafka-rest)
  ![Stars](https://img.shields.io/github/stars/confluentinc/kafka-rest?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/kafka-rest?style=social)
  - REST Proxy for Kafka (still used, especially with Confluent platform).

### Storage and KRaft

#### KRaft (ZooKeeper-less Kafka)

- :green_heart:[KRaft Mode (official)](https://kafka.apache.org/documentation/#kraft)
  - Kafka without ZooKeeper. Production-ready since 3.3.1, default in 4.0+.
  - Simpler operations, faster metadata propagation, better scalability.
  - Migration guide: [KRaft Migration](https://kafka.apache.org/documentation/#kraft_zk_migration)

#### Tiered Storage and Alternatives

- :green_heart:[Kafka Tiered Storage (official)](https://github.com/apache/kafka)
  ![Stars](https://img.shields.io/github/stars/apache/kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/kafka?style=social)
  - Offload older segments to object storage (S3, Azure Blob, GCS).

- :green_heart:[MinIO](https://github.com/minio/minio)
  ![Stars](https://img.shields.io/github/stars/minio/minio?style=social)
  ![Forks](https://img.shields.io/github/forks/minio/minio?style=social)
  - Common S3-compatible backend for Kafka ecosystem testing.

- :green_heart:[Redpanda](https://github.com/redpanda-data/redpanda)
  ![Stars](https://img.shields.io/github/stars/redpanda-data/redpanda?style=social)
  ![Forks](https://img.shields.io/github/forks/redpanda-data/redpanda?style=social)
  - Kafka-compatible platform; lots of teams use it as an alternative.

### Testing and Troubleshooting

- :green_heart:[Testcontainers Java](https://github.com/testcontainers/testcontainers-java)
  ![Stars](https://img.shields.io/github/stars/testcontainers/testcontainers-java?style=social)
  ![Forks](https://img.shields.io/github/forks/testcontainers/testcontainers-java?style=social)
  - The default approach for Kafka integration tests in JVM land.

- :green_heart:[Toxiproxy](https://github.com/Shopify/toxiproxy)
  ![Stars](https://img.shields.io/github/stars/shopify/toxiproxy?style=social)
  ![Forks](https://img.shields.io/github/forks/shopify/toxiproxy?style=social)
  - Simulate network pain (latency, timeouts) for Kafka clients.

- :green_heart:[k6](https://github.com/grafana/k6)
  ![Stars](https://img.shields.io/github/stars/grafana/k6?style=social)
  ![Forks](https://img.shields.io/github/forks/grafana/k6?style=social)
  - Load testing (useful for HTTP bridges, schema registry endpoints, etc).

- :green_heart:[Cruise Control](https://github.com/linkedin/cruise-control)
  ![Stars](https://img.shields.io/github/stars/linkedin/cruise-control?style=social)
  ![Forks](https://img.shields.io/github/forks/linkedin/cruise-control?style=social)
  - Not just ops — also great for diagnosing imbalance & broker stress.

### Monitoring, Alerts, and Visualization

- :green_heart:[kafka_exporter (Prometheus)](https://github.com/danielqsj/kafka_exporter)
  ![Stars](https://img.shields.io/github/stars/danielqsj/kafka_exporter?style=social)
  ![Forks](https://img.shields.io/github/forks/danielqsj/kafka_exporter?style=social)
  - Most common Prometheus exporter for Kafka. :contentReference[oaicite:5]{index=5}

- :green_heart:[JMX Exporter](https://github.com/prometheus/jmx_exporter)
  ![Stars](https://img.shields.io/github/stars/prometheus/jmx_exporter?style=social)
  ![Forks](https://img.shields.io/github/forks/prometheus/jmx_exporter?style=social)
  - Standard route for JVM metrics (brokers, connect workers, streams apps).

- :green_heart:[Burrow](https://github.com/linkedin/Burrow)
  ![Stars](https://img.shields.io/github/stars/linkedin/Burrow?style=social)
  ![Forks](https://img.shields.io/github/forks/linkedin/Burrow?style=social)
  - Consumer lag checking (classic).

- :green_heart:[kafka-lag-exporter](https://github.com/lightbend/kafka-lag-exporter)
  ![Stars](https://img.shields.io/github/stars/lightbend/kafka-lag-exporter?style=social)
  ![Forks](https://img.shields.io/github/forks/lightbend/kafka-lag-exporter?style=social)
  - Prometheus-native lag monitoring (lightweight alternative to Burrow).

- :green_heart:[Kafka Minion](https://github.com/cloudhut/kminion)
  ![Stars](https://img.shields.io/github/stars/cloudhut/kminion?style=social)
  ![Forks](https://img.shields.io/github/forks/cloudhut/kminion?style=social)
  - Prometheus exporter with detailed consumer group metrics.

- :green_heart:[Xinfra Monitor (LinkedIn)](https://github.com/linkedin/kafka-monitor)
  ![Stars](https://img.shields.io/github/stars/linkedin/kafka-monitor?style=social)
  ![Forks](https://img.shields.io/github/forks/linkedin/kafka-monitor?style=social)
  - End-to-end cluster monitoring and availability testing.

- :green_heart:[Grafana](https://github.com/grafana/grafana)
  ![Stars](https://img.shields.io/github/stars/grafana/grafana?style=social)
  ![Forks](https://img.shields.io/github/forks/grafana/grafana?style=social)
  - Dashboards for Kafka metrics (everyone ends up here).

- :green_heart:[Prometheus](https://github.com/prometheus/prometheus)
  ![Stars](https://img.shields.io/github/stars/prometheus/prometheus?style=social)
  ![Forks](https://img.shields.io/github/forks/prometheus/prometheus?style=social)
  - Metrics backbone.

- :green_heart:[OpenTelemetry Collector](https://github.com/open-telemetry/opentelemetry-collector)
  ![Stars](https://img.shields.io/github/stars/open-telemetry/opentelemetry-collector?style=social)
  ![Forks](https://img.shields.io/github/forks/open-telemetry/opentelemetry-collector?style=social)
  - Logs/metrics/traces pipeline (Kafka shops use it a lot).

### Backup and Restore

- :green_heart:[MirrorMaker 2 (official)](https://github.com/apache/kafka)
  ![Stars](https://img.shields.io/github/stars/apache/kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/kafka?style=social)
  - Cross-cluster replication (DR, migrations).

- :green_heart:[Confluent Replicator (docs)](https://docs.confluent.io/platform/current/multi-dc-deployments/replicator/index.html)
  - Commercial, but common in enterprise environments.

- :green_heart:[Strimzi Cluster Operator (mirror maker examples)](https://github.com/strimzi/strimzi-kafka-operator)
  ![Stars](https://img.shields.io/github/stars/strimzi/strimzi-kafka-operator?style=social)
  ![Forks](https://img.shields.io/github/forks/strimzi/strimzi-kafka-operator?style=social)
  - Good MM2 support for k8s clusters.

### Security and Compliance

- :green_heart:[Apache Ranger](https://github.com/apache/ranger)
  ![Stars](https://img.shields.io/github/stars/apache/ranger?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/ranger?style=social)
  - Often used for Kafka authorization in Hadoop-y ecosystems.

- :green_heart:[Keycloak](https://github.com/keycloak/keycloak)
  ![Stars](https://img.shields.io/github/stars/keycloak/keycloak?style=social)
  ![Forks](https://img.shields.io/github/forks/keycloak/keycloak?style=social)
  - Common OIDC provider for Kafka OAuth flows.

- :green_heart:[cert-manager](https://github.com/cert-manager/cert-manager)
  ![Stars](https://img.shields.io/github/stars/cert-manager/cert-manager?style=social)
  ![Forks](https://img.shields.io/github/forks/cert-manager/cert-manager?style=social)
  - TLS for brokers / connect / schema registry in k8s.

### Development Tools

#### Core clients (widely used)

- :green_heart:[librdkafka](https://github.com/confluentinc/librdkafka)
  ![Stars](https://img.shields.io/github/stars/confluentinc/librdkafka?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/librdkafka?style=social)
  - The C/C++ client that powers a lot of bindings. :contentReference[oaicite:6]{index=6}

- :green_heart:[confluent-kafka-go](https://github.com/confluentinc/confluent-kafka-go)
  ![Stars](https://img.shields.io/github/stars/confluentinc/confluent-kafka-go?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/confluent-kafka-go?style=social)
  - Go client (librdkafka wrapper). :contentReference[oaicite:7]{index=7}

- :green_heart:[Sarama (Go)](https://github.com/IBM/sarama)
  ![Stars](https://img.shields.io/github/stars/IBM/sarama?style=social)
  ![Forks](https://img.shields.io/github/forks/IBM/sarama?style=social)
  - The other Go client you’ll run into everywhere.

- :green_heart:[kafka-go](https://github.com/segmentio/kafka-go)
  ![Stars](https://img.shields.io/github/stars/segmentio/kafka-go?style=social)
  ![Forks](https://img.shields.io/github/forks/segmentio/kafka-go?style=social)
  - Pure Go client (no CGO), very popular.

- :green_heart:[franz-go](https://github.com/twmb/franz-go)
  ![Stars](https://img.shields.io/github/stars/twmb/franz-go?style=social)
  ![Forks](https://img.shields.io/github/forks/twmb/franz-go?style=social)
  - Go client with great protocol coverage.

- :green_heart:[KafkaJS (Node.js)](https://github.com/tulios/kafkajs)
  ![Stars](https://img.shields.io/github/stars/tulios/kafkajs?style=social)
  ![Forks](https://img.shields.io/github/forks/tulios/kafkajs?style=social)
  - The Node.js Kafka client most people end up using.

- :green_heart:[confluent-kafka-python](https://github.com/confluentinc/confluent-kafka-python)
  ![Stars](https://img.shields.io/github/stars/confluentinc/confluent-kafka-python?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/confluent-kafka-python?style=social)
  - Python client backed by librdkafka. :contentReference[oaicite:8]{index=8}

- :green_heart:[confluent-kafka-dotnet](https://github.com/confluentinc/confluent-kafka-dotnet)
  ![Stars](https://img.shields.io/github/stars/confluentinc/confluent-kafka-dotnet?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/confluent-kafka-dotnet?style=social)
  - Solid .NET client.

- :green_heart:[rust-rdkafka](https://github.com/fede1024/rust-rdkafka)
  ![Stars](https://img.shields.io/github/stars/fede1024/rust-rdkafka?style=social)
  ![Forks](https://img.shields.io/github/forks/fede1024/rust-rdkafka?style=social)
  - Rust client (librdkafka binding).

#### Stream processing

- :green_heart:[Kafka Streams (official)](https://github.com/apache/kafka)
  ![Stars](https://img.shields.io/github/stars/apache/kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/kafka?style=social)
  - Java stream processing library built into Kafka.

- :green_heart:[ksqlDB](https://github.com/confluentinc/ksql)
  ![Stars](https://img.shields.io/github/stars/confluentinc/ksql?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/ksql?style=social)
  - Streaming SQL (very common in Confluent setups).

#### Schema and serialization

- :green_heart:[Schema Registry (Confluent)](https://github.com/confluentinc/schema-registry)
  ![Stars](https://img.shields.io/github/stars/confluentinc/schema-registry?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/schema-registry?style=social)
  - Avro/JSON Schema/Protobuf registry. :contentReference[oaicite:9]{index=9}

- :green_heart:[Apicurio Registry](https://github.com/Apicurio/apicurio-registry)
  ![Stars](https://img.shields.io/github/stars/Apicurio/apicurio-registry?style=social)
  ![Forks](https://img.shields.io/github/forks/Apicurio/apicurio-registry?style=social)
  - Another solid schema/API registry option.

- :green_heart:[Karapace (Aiven)](https://github.com/aiven/karapace)
  ![Stars](https://img.shields.io/github/stars/aiven/karapace?style=social)
  ![Forks](https://img.shields.io/github/forks/aiven/karapace?style=social)
  - Open source schema registry and REST proxy alternative.

#### Kafka Connect / integrations

- :green_heart:[Kafka Connect (official)](https://github.com/apache/kafka)
  ![Stars](https://img.shields.io/github/stars/apache/kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/kafka?style=social)
  - Connect runtime lives in upstream Kafka.

- :green_heart:[Debezium](https://github.com/debezium/debezium)
  ![Stars](https://img.shields.io/github/stars/debezium/debezium?style=social)
  ![Forks](https://img.shields.io/github/forks/debezium/debezium?style=social)
  - CDC platform built on Kafka Connect (massively used).

- :green_heart:[Kafka Connect JDBC](https://github.com/confluentinc/kafka-connect-jdbc)
  ![Stars](https://img.shields.io/github/stars/confluentinc/kafka-connect-jdbc?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/kafka-connect-jdbc?style=social)
  - Still the default JDBC connector in a lot of places.

### Data Processing and Machine Learning

- :green_heart:[Spark Structured Streaming (Kafka integration)](https://github.com/apache/spark)
  ![Stars](https://img.shields.io/github/stars/apache/spark?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/spark?style=social)
  - Kafka is one of the main streaming inputs people use with Spark.

- :green_heart:[Flink](https://github.com/apache/flink)
  ![Stars](https://img.shields.io/github/stars/apache/flink?style=social)
  ![Forks](https://img.shields.io/github/forks/apache/flink?style=social)
  - Kafka connectors everywhere in Flink deployments.

- :green_heart:[Benthos](https://github.com/benthosdev/benthos)
  ![Stars](https://img.shields.io/github/stars/benthosdev/benthos?style=social)
  ![Forks](https://img.shields.io/github/forks/benthosdev/benthos?style=social)
  - Stream processing with native Kafka input/output connectors.

- :green_heart:[Vector](https://github.com/vectordotdev/vector)
  ![Stars](https://img.shields.io/github/stars/vectordotdev/vector?style=social)
  ![Forks](https://img.shields.io/github/forks/vectordotdev/vector?style=social)
  - Observability pipeline with Kafka source/sink support.

- :green_heart:[dbt (often paired with Kafka pipelines)](https://github.com/dbt-labs/dbt-core)
  ![Stars](https://img.shields.io/github/stars/dbt-labs/dbt-core?style=social)
  ![Forks](https://img.shields.io/github/forks/dbt-labs/dbt-core?style=social)
  - Not Kafka-native, but shows up in real end-to-end pipelines.

### Miscellaneous

- :green_heart:[awesome-kafka (existing list)](https://github.com/semantalytics/awesome-kafka)
  ![Stars](https://img.shields.io/github/stars/semantalytics/awesome-kafka?style=social)
  ![Forks](https://img.shields.io/github/forks/semantalytics/awesome-kafka?style=social)
  - Another curated list (good for cross-checking ideas).

- :green_heart:[Confluent Examples](https://github.com/confluentinc/examples)
  ![Stars](https://img.shields.io/github/stars/confluentinc/examples?style=social)
  ![Forks](https://img.shields.io/github/forks/confluentinc/examples?style=social)
  - Recipes for clients, streams, connect, schemas.

---

## Guides, Documentations, Blogs, and Learnings

### Guides

- [Apache Kafka Documentation](https://kafka.apache.org/documentation/)
- [Confluent Documentation](https://docs.confluent.io/)
- [Strimzi Documentation](https://strimzi.io/documentation/)
- [Kafka Improvement Proposals (KIPs)](https://cwiki.apache.org/confluence/display/KAFKA/Kafka+Improvement+Proposals)

### Blogs and Videos

- [Confluent Blog](https://www.confluent.io/blog/)
- [Redpanda Blog](https://www.redpanda.com/blog)
- [Strimzi Blog](https://strimzi.io/blog/)
- [The Apache Kafka YouTube channel](https://www.youtube.com/results?search_query=apache+kafka)
- [Confluent YouTube channel](https://www.youtube.com/@Confluent)

### Learnings and Documentations

- [Designing Event-Driven Systems](https://www.confluent.io/designing-event-driven-systems/) (free book)
- [Kafka Internals (community notes)](https://cwiki.apache.org/confluence/display/KAFKA/Index)
- [Schema Registry docs](https://docs.confluent.io/platform/current/schema-registry/index.html)
- [Kafka Connect docs](https://kafka.apache.org/documentation/#connect)

---

## Anti-Patterns and Common Mistakes

### Architecture Anti-Patterns

- **Using Kafka as a database**: Kafka is a log, not a database. No random access, no updates, no deletes (only compaction).
- **Single large topic instead of multiple**: Splits by domain make scaling, security, and retention easier.
- **No partitioning strategy**: Random partitioning kills ordering guarantees. Use key-based partitioning.
- **Ignoring replication factor**: `replication.factor=1` means data loss on broker failure. Use 3+ in production.
- **Over-partitioning**: 1000+ partitions per broker increases latency and recovery time.
- **Under-partitioning**: Can't scale consumers beyond partition count. Plan for growth.

### Operations Anti-Patterns

- **Running without monitoring**: No lag alerts = invisible consumer failures.
- **Skipping schema registry**: Schema evolution without registry = runtime errors in production.
- **No retention policy**: Infinite retention = disk full. Set `retention.ms` or `retention.bytes`.
- **Manual consumer offset management**: Let Kafka handle it unless you have a specific reason.
- **Ignoring ISR (In-Sync Replicas)**: `min.insync.replicas=1` defeats the purpose of replication.

### Development Anti-Patterns

- **Producing synchronously in loops**: Kills throughput. Batch and use async sends.
- **No idempotency**: Network retries without `enable.idempotence=true` = duplicate messages.
- **Blocking consumer poll loop**: Long processing = session timeouts. Use separate worker threads.
- **Catching and logging exceptions**: Consumer stops consuming but doesn't fail. Fail fast or handle properly.
- **Not handling rebalances**: Leads to duplicate processing or data loss.

### When NOT to Use Kafka

- **Low-latency RPC**: Use gRPC, HTTP/2, or message queues (RabbitMQ, SQS).
- **Request-reply patterns**: Kafka isn't built for this. Use traditional queues.
- **Small-scale systems (< 100 msg/sec)**: Overhead not worth it. Use managed queues.
- **Strong transactional consistency across services**: Kafka gives you at-least-once or exactly-once within Kafka, not distributed transactions.
- **Simple pub/sub with no replay needs**: Redis Pub/Sub or NATS might be simpler.

---

## Real-World Patterns and Best Practices

### Multi-Region Disaster Recovery

- **Active-Passive**: Use MirrorMaker 2 for continuous replication. Failover = consumer switch to DR cluster.
- **Active-Active**: Aggregate topics with different prefixes per region. Watch out for circular replication.
- **Stretched clusters**: Not recommended (latency, split-brain risks). Use replication instead.

### Zero-Downtime Rolling Upgrades

1. Upgrade brokers one at a time (rolling restart).
2. Upgrade clients (consumers first, then producers).
3. Use feature flags to toggle new protocol features.
4. Monitor ISR and lag during upgrades.
5. Leverage Strimzi Drain Cleaner on k8s to drain pods gracefully.

### Schema Evolution Best Practices

- **Backward compatibility**: New consumers read old data (add optional fields, not remove).
- **Forward compatibility**: Old consumers read new data (use defaults).
- **Full compatibility**: Both directions (safest for production).
- Use Schema Registry with `BACKWARD` or `FULL` compatibility mode.
- Version schemas explicitly in CI/CD.

### Partition Sizing Guidelines

- **General rule**: 1-3 partitions per consumer in your peak consumer group.
- **Max partitions per broker**: 4000 (above this, recovery time and metadata overhead grows).
- **Partition size**: Keep under 10GB per partition for fast recovery.
- **Key distribution**: Ensure even key distribution to avoid hot partitions.

### Consumer Group Scaling Patterns

- **Horizontal scaling**: Add more consumers (up to partition count).
- **Vertical scaling**: Increase consumer throughput (batching, parallel processing).
- **Static membership**: Use `group.instance.id` to avoid rebalances on restarts.
- **Incremental rebalancing**: Use `partition.assignment.strategy=CooperativeSticky`.

### Transactional Producer Patterns

- **Exactly-once semantics**: Enable `enable.idempotence=true` + `transactional.id`.
- **Atomic multi-partition writes**: Use transactions to write to multiple topics atomically.
- **Consumer isolation**: Set `isolation.level=read_committed` on consumers.
- **Zombie fencing**: Kafka fences out old producers with same `transactional.id`.

### Cloud-Native Kafka on Kubernetes

- **Pod Disruption Budgets**: Set `maxUnavailable=1` to prevent mass evictions.
- **Node Affinity**: Spread brokers across availability zones.
- **Storage Classes**: Use SSD-backed storage with `WaitForFirstConsumer` binding.
- **Resource Limits**: Set memory limits to avoid OOMKills. Use JVM heap = 50-60% of container memory.
- **Liveness vs Readiness**: Readiness should check Kafka health, not just process alive.

### Cost Optimization

- **Tiered storage**: Move cold data to S3 to reduce broker storage costs.
- **Spot instances**: Use for non-critical brokers (not recommended for production).
- **Right-sizing brokers**: Monitor CPU/disk/network, scale down over-provisioned clusters.
- **Compression**: Enable `compression.type=snappy` or `zstd` to reduce storage and network.
- **Retention tuning**: Shorter retention = less storage. Align with business needs.

---

## Tool Comparison Tables

### Web UIs for Kafka

| Tool | License | Best For | Pros | Cons |
|------|---------|----------|------|------|
| **Redpanda Console** | OSS | Modern teams | Best UI/UX, feature-rich | Redpanda branding |
| **AKHQ** | OSS | Full-featured | Schema registry + Connect | Java-based (heavier) |
| **Kafka UI** | OSS | Lightweight | Fast, modern | Fewer integrations |
| **Kafdrop** | OSS | Simple browsing | Very lightweight | Basic features only |
| **CMAK** | OSS | Legacy systems | Battle-tested | Slow maintenance |
| **Kpow** | Commercial | Enterprise | Production-ready support | Paid |
| **Control Center** | Commercial | Confluent shops | Deep integration | Expensive |

### Kafka Clients (Go)

| Client | Type | Best For | Pros | Cons |
|--------|------|----------|------|------|
| **confluent-kafka-go** | CGO (librdkafka) | Performance | Mature, fast | CGO dependencies |
| **Sarama** | Pure Go | Enterprise | Feature-complete | Complex API |
| **kafka-go** | Pure Go | Simplicity | No CGO, clean API | Less battle-tested |
| **franz-go** | Pure Go | Protocol coverage | Modern, fast | Smaller community |

### Prometheus Exporters

| Exporter | Best For | Metrics Coverage | Resource Usage |
|----------|----------|------------------|----------------|
| **kafka_exporter** | Consumer lag + topics | High | Low |
| **JMX Exporter** | Broker JVM metrics | Very High | Medium |
| **Kafka Minion** | Consumer groups | High | Low |
| **kafka-lag-exporter** | Lag-focused | Medium | Very Low |

---

## Contribute

Contributions are welcome!

- Fork the repo
- Add your tool/resource in the right section
- Keep descriptions short
- Only include active / credible / widely used things
- Prefer OSS, but widely used commercial tools/docs are ok (mark them clearly)

Please open a PR.

## License

[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/)
