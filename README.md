# Real-Time-Streaming-with-Kafka-and-Python

This repository contains a submission for my Data Engineering course, focused on real-time streaming and processing of messages using **Apache Kafka**. This lab covers the setup, message production, and consumption pipelines using Python clients to simulate and process streaming data.

---

### Business Problem

Real-time data processing is crucial in many modern applications such as fraud detection, live dashboards, and recommendation engines. Apache Kafka is a popular streaming platform that enables ingestion and distribution of real-time events. This lab aimed to simulate a real-world pipeline where data is streamed from producers and handled by consumer applications in real-time.

---

### Project Objectives

- Set up Kafka producers and consumers using Python (`kafka-python` library)
- Simulate a stream of input messages (e.g., transaction records)
- Transform and process streaming data using Python logic
- Demonstrate message publication and subscription across Kafka topics
- Validate stream ingestion, transformation, and output

---

###  Solution Approach

1. **Kafka Configuration**
   - Launched a local Kafka broker with Zookeeper
   - Created topics for test stream and final output

2. **Message Production**
   - Simulated transaction events using a Kafka producer
   - Streamed messages into Kafka topics using custom JSON payloads

3. **Message Consumption & Processing**
   - Developed a Kafka consumer to listen for topic messages
   - Parsed and transformed incoming events using Python
   - Logged and printed event summaries for verification

4. **Integration Testing**
   - Verified end-to-end functionality:
     - Producer → Kafka Topic → Consumer

---

###  Business Value

- **Real-Time Monitoring**: Simulates a robust real-time alerting or logging system
- **Scalable Architecture**: Kafka's decoupled design supports massive throughput
- **Extendability**: The logic can be extended to Spark Streaming, Flink, or ML inference pipelines

---

###  Challenges Encountered

- Managing Kafka broker setup and local networking
- Handling malformed messages and consumer timeouts
- Ensuring message order and avoiding duplication

---
