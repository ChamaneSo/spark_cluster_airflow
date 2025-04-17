# Docker Spark and Airflow Project

This project sets up a Docker environment for Apache Spark and Apache Airflow, including their respective user interfaces. 

## Project Structure

```
docker-spark-airflow
├── docker-compose.yml
├── spark
│   ├── Dockerfile
│   └── config
│       └── spark-defaults.conf
├── airflow
│   ├── Dockerfile
│   └── dags
│       └── example_dag.py
└── README.md
```

## Services

### Apache Spark
- **Dockerfile**: Contains instructions to build the Docker image for Spark.
- **Configuration**: The `spark-defaults.conf` file includes default settings for Spark applications.

### Apache Airflow
- **Dockerfile**: Contains instructions to build the Docker image for Airflow.
- **DAGs**: The `example_dag.py` file provides a sample workflow for demonstration purposes.

## Setup Instructions

1. Clone the repository:
   ```
   git clone <repository-url>
   cd docker-spark-airflow
   ```

2. Build and start the services using Docker Compose:
   ```
   docker-compose up --build
   ```

3. Access the user interfaces:
   - Apache Spark UI: [http://localhost:8080](http://localhost:8080)
   - Apache Airflow UI: [http://localhost:8081](http://localhost:8081)

## Usage

- You can add your own DAGs in the `airflow/dags` directory.
- Modify the Spark configuration in `spark/config/spark-defaults.conf` as needed.

## License

This project is licensed under the MIT License.