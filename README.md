<<<<<<< HEAD
# New-York-Taxi-Data-Pipline-
Build a scalable data pipeline for extracting, processing, and analyzing New York Yellow Taxi Trip data from 2019, and load processed data into ClickHouse for further analysis.
=======
# New-York-Taxi-Data-Pipeline-
Build a scalable data pipeline for extracting, processing, and analyzing New York Yellow Taxi Trip data from 2019, and load processed data into ClickHouse for further analysis.


Documentation:
    Your repository must include a README.md file that contains:
        Project Overview: A brief description of the project and its objectives.
        Environment Setup: Detailed instructions on how to set up the development environment, including any required software installations, environment variables, and dependencies.
        Running the Project: Step-by-step instructions on how to run your scripts and the data pipeline, including how to execute the data extraction, processing, loading, and analysis components.
        Pipeline Orchestration: Explanation of how to set up and trigger the Apache Airflow DAGs.

        nyc-taxi-data-pipeline/
│
├── dags/
│   └── nyc_taxi_dag.py
│
├── scripts/
│   ├── data_extraction.py
│   ├── data_processing.py
│   ├── data_loading.py
│   └── data_analysis.py
│
├── docker-compose.yml
├── requirements.txt
└── README.md

>>>>>>> e1d24b12bd2a1bf5dc93f72f26cd16a8d9eef7b4


Documentation
# NY Taxi Data Pipeline

## Project Overview
This project processes New York Taxi Trip data for the year 2019, deriving analytical insights, and loads the processed data into ClickHouse for further analysis.

## Environment Setup
### Requirements
- Docker
- Apache Spark
- Python Libraries: requests, retrying, pyspark, clickhouse_driver, airflow

### Setup Instructions
1. Install Docker and Docker Compose.
2. Setup Apache Spark:
    - Download and install Apache Spark from the official website.
3. Setup ClickHouse:
    - Run `docker run -d --name some-clickhouse-server --ulimit nofile=262144:262144 yandex/clickhouse-server`.
4. Setup Apache Airflow:
    - Follow Airflow installation instructions from the official website.

## Running the Project
### Data Extraction
- Run the data download script: `python download_data.py`

### Data Processing
- Run the Spark processing script: `python process_data.py`

### Data Loading
- Run the data loading script: `python load_data.py`

## Pipeline Orchestration
### Setup Airflow
- Follow the Airflow setup instructions.
- Place the DAG file in the Airflow DAGs directory.
- Trigger the DAG from the Airflow UI.

