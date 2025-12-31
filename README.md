# WarehouseForge | Snowflake ELT Pipeline with dbt and Airflow

Welcome to the Snowflake ELT Pipeline project! 🚀 This repository showcases a complete end-to-end data pipeline built using cutting-edge technologies, including Snowflake, dbt (Data Build Tool), and Apache Airflow. Dive into the details to see how modern data engineering practices can transform and orchestrate data efficiently.


## Architecture Diagram

![Architecture Diagram](https://github.com/DivineSamOfficial/Snowflake-ELT-Pipeline-with-dbt-and-Airflow/blob/main/Images/ELT_snw-dbt-airflow.jpg)

## Airflow DAG

![Airflow DAG](https://github.com/DivineSamOfficial/Snowflake-ELT-Pipeline-with-dbt-and-Airflow/blob/main/Images/Screenshot%202024-07-25%20at%2012.30.16%E2%80%AFAM.png)

## Data Flow Diagram

![DataFlowDiag](https://github.com/DivineSamOfficial/Snowflake-ELT-Pipeline-with-dbt-and-Airflow/blob/main/Images/DataFlowDiag.png)

## Project Overview

This project implements a complete ELT workflow using the **TPCH Orders** table from Snowflake’s sample database. Raw data is loaded directly into Snowflake and transformed using **dbt models** to produce analytics-ready datasets. The entire pipeline is orchestrated with **Apache Airflow**, ensuring automated, repeatable, and observable execution.

### Key Components

1. **Data Source**:
   - **TPCH Orders Table**: Source data derived from Snowflake’s built-in TPCH sample dataset, representing transactional order records.

2. **Data Storage**:
   - **Snowflake**: Serves as the central data warehouse for raw, staging, and transformed datasets.

 **Data Transformation**:
   - **dbt (Data Build Tool)**:
     - **Source Definitions**: Explicit declaration and management of raw source tables.
     - **Staging Models**: Intermediate models to clean, standardize, and prepare raw data.
     - **Transformed Models**: Fact tables and analytical models designed for reporting and downstream consumption.
     - **Macros**: Reusable transformation logic, including business calculations such as discounted pricing.
     - **Testing & Data Quality**: Generic and singular tests to validate data integrity and business rules.

4. **Data Orchestration**:
   - **Apache Airflow**: Orchestrates dbt executions, manages task dependencies, and handles scheduling and retries.

---



Happy data engineering! 🌟
