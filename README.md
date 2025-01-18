# Coincidences Analyzer Agent

This repository provides a setup for deploying the Coincidences Analyzer Agent using Docker.

## Prerequisites

- Docker installed on your system.
- Access to the Docker image `amlabdr/coincidences_analyzer_agent:latest`.
- (Not required for runnin the GUI but required for working properly) A running message broker (e.g., activemq) accessible at the specified `BROKER_URL`.

## Quick Start

### 1. Clone the Repository
```bash
git clone <repo-url>
cd coincidences_analyzer_agent
```

### 2. Configure Environment Variables
You can modify the BROKER_URL default variables directly in the `run.sh` script if needed with the address of the ActiveMQ Broker and the name of the endpoint for the agent:

```bash
BROKER_URL="amqp://localhost:5672/"
ENDPOINT="coincidences_analyzer"
```

### 3. Run the Application
Make the script executable and run it:

```bash
chmod +x run.sh
./run.sh
```
