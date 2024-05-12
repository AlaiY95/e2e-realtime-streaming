# e2e-realtime-streaming
## Introduction

This project functions as an extensive tutorial on constructing a full-fledged end-to-end data engineering pipeline. It encompasses every phase, starting from data ingestion, proceeding through processing, and culminating in storage. It leverages a resilient technology stack comprising Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. The entire infrastructure is containerized with Docker, ensuring effortless deployment and scalability.

## System Architecture

![System Architecture](https://github.com/AlaiY95/e2e-realtime-streaming/blob/main/Data%20engineering%20architecture.png)

The project is designed with the following components:

- **Data Source**: We utilize the `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka**: and Zookeeper: Utilized for streaming data from PostgreSQL to the processing engine.
- **Control Center** and Schema Registry: Aiding in monitoring and schema management of our Kafka streams.
- **Apache Spark**: Utilized for data processing with its master and worker nodes.
- **Cassandra**: The storage destination for the processed data.

## Technologies

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/AlaiY95/e2e-realtime-streaming.git
    ```

2. Navigate to the project directory:
    ```bash
    cd e2e-realtime-streaming
    ```

3. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```
