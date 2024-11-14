# Distributed System with Flink StateFun, and Redpanda (Kafka)

This repository sets up a distributed system architecture using Apache Flink, Flink StateFun, and Redpanda (Kafka-compatible message broker), along with a Functions service and a Redpanda Console for monitoring.

## Prerequisites

- Docker and Docker Compose installed on your machine.

## Architecture Overview

This setup includes the following services:

1. **Functions Service** - Custom service used to run application-specific logic.
2. **Flink Master** - Manages the Flink cluster and serves as the StateFun runtime master.
3. **Flink Worker** - Executes tasks managed by the Flink Master in the distributed setup.
4. **Kafka (Redpanda)** - Acts as a Kafka-compatible broker for data ingress and egress, facilitating message passing within the distributed system.
5. **Redpanda Console** - A console for monitoring and managing Redpanda.

## Configuration Files

This setup includes the following configurations:

1. **module.yaml** -  - This file configures StateFun's remote functions, specifying how Flink interacts with external functions and services.
2. **flink-conf.yaml** - This file contains general settings for Flink, such as memory allocation, job management, and networking settings.


## Getting Started

1. Clone the repository.

2. Run the following command to start all services:
    
   - docker-compose up -d

3. Run the following command to stop all services:

   - docker-compose down

## Accessing the Services

1. **Redpanda Console** -  -  http://localhost:8079 - For monitoring and managing Kafka topics, brokers, and messages.
2. **Flink Dashboard** - http://localhost:8081 - To monitor Flink jobs, task managers, and cluster performance.