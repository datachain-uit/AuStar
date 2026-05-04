# Project Demonstration

This directory contains documentation and evidence regarding the operational deployment of the Vitamin D prediction application and its supporting big data pipeline.

## 1. Application Demonstration

The demonstration focuses on the end-to-end functionality of the medical prediction system:

- Interactive dashboard for medical professionals to manage patient records and input clinical parameters.
- Real-time inference using a Stacking ensemble learning model to identify Vitamin D deficiency risks.
- Validation of data entry and secure processing of patient information within the clinic management module.

## 2. Pipeline Demonstration

The pipeline demonstration illustrates the lifecycle of big data used for training and refining prediction models:

- Real-time ingestion of clinical events and data streams using Python-implemented Apache Kafka.
- Distributed data processing, feature engineering, and data enrichment using Apache Spark.
- Implementation of SVM-SMOTE techniques to address class imbalance in the medical training sets.
- Automated workflow orchestration, including model re-training and monitoring cycles, via Apache Airflow.
- Verification of data persistence and storage architecture within Amazon S3.

## 3. Deployment and Execution

Procedures for reproducing the demonstrated environment:

- Launching the integrated system stack using Docker Compose for local environments.
- Configurations for deploying services within a scalable Kubernetes cluster.
- Integration of system monitoring tools to track application health and model performance metrics.
