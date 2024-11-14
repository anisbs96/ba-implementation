# Distributed System Fault Injection and Anomaly Analysis

This repository contains the setup, collected logs, notebooks, and results generated from fault injection experiments on a distributed system. The data and notebooks support the thesis sections, detailing steps for log generalization and difference, anomaly determination, and evaluation.

## Prerequisites

- **Python 3**: Ensure Python 3 is installed on your machine.
- **Jupyter Notebook**: Required to view and execute the `.ipynb` files. Install it by running `pip install jupyter` if not already installed.
- **requirements.txt**: The file lists all Python dependencies required to run the Jupyter notebooks. Install these dependencies by running the following command: `pip install -r requirements.txt`.

## Folder Structure

### 1. Collected_logs

This folder contains logs collected during various fault injection scenarios and the normal state. Each log file in this directory is mapped to a specific fault scenario and saved in CSV format, detailing the system’s responses during injected faults. These logs are essential inputs for the log generalization and difference and anomaly determination steps.

**File Mapping**:

- `fault_1.csv` - Logs collected during the first fault injection scenario targeting flink-master.
- `fault_2.csv` - Logs collected during the second fault injection scenario targeting flink-worker.
- `fault_3.csv` - Logs collected during the third fault injection scenario targeting kafka-broker.
- `fault_4.csv` - Logs collected during the fourth fault injection scenario targeting functions-service.
- `normal.csv`  - Logs collected during the normal state of the system running without any fault injection.

### 2. Notebooks

This folder includes Jupyter notebooks used to generate the thesis results and visualize findings from the log data. Each notebook corresponds to a specific section of the thesis:

- **4.4 Log_Generalization.ipynb** - Performs log generalization and difference analysis, preparing the raw log data for anomaly determination.
- **4.5 Anomaly_Determination.ipynb** - Applies an anomaly determination process on the generalized and enriched logs to identify potential anomalies.
- **5. Evaluation.ipynb** - Generates evaluation figures and tables used for the analysis to assess system behavior, resilience, and anomaly patterns based on the processed logs.

### 3. Results

This folder contains the processed logs and results generated from log generalization and difference and anomaly determination. It is organized into the following subfolders:

#### Anomaly_Determination

- Contains the logs resulting from the anomaly determination process.
- Files in this subfolder represent logs flagged as potentially anomalous, categorized based on different fault injection scenarios and component behaviors.

#### Log_Generalization

- Stores the logs generated at different phases of the log generalization and difference process.
- These logs capture the transformed versions of the original logs.
