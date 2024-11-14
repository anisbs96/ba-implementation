# Distributed System using Apache Flink and Apache Kafka

This repository contains the core files, components, and logging resources for a distributed system used to study and analyze fault tolerance and anomaly detection. The repository is organized into subfolders, each serving a specific role in the system's setup, operation, and logging of fault injection scenarios.

## Folder Structure

### 1. Components

The **Components** folder contains all resources related to the system's components, including configuration files, Docker setups, and any necessary documentation to initialize and run the distributed system's core services. This folder includes:

- Configuration files for setting up services.
- Docker Compose files for containerizing and orchestrating services.
- Documentation on each component's purpose, configuration, and interconnections within the distributed system.

For detailed instructions on each component and setup procedures, refer to the `README.md` located within the `Components` folder.

### 2. Logging

The **Logging** folder includes resources related to log collection and management. This folder is structured to store logs generated during fault injection experiments and to document the log generalization and difference and anomaly determination stages. It contains:

- **Collected_logs**: A folder containing logs collected from various fault injection scenarios, essential for the analysis of system responses.
- **Notebooks**: Jupyter notebooks used for processing the logs and generating insights. Each notebook corresponds to specific stages in the log analysis, such as log generalization, anomaly determination, and evaluation.
- **Results**: A folder containing processed logs and outputs from the log analysis phases, organized into subfolders for `Anomaly_Determination` and `Log_Generalization`.

For more information on log collection, processing, and analysis, refer to the `README.md` in the `Logging` folder.

## Getting Started

1. **Set up the Components**:
   - Follow the instructions in the `Components` folder to set up and initialize the distributed system components.

2. **Run the Logging Analysis**:
   - After setting up and running the components, collect the logs in the `Collected_logs` folder.
   - Follow the instructions in the `Logging` folder to execute the Jupyter notebooks and generate analysis results.