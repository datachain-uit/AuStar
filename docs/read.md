# Documentation

This directory contains comprehensive technical documentation regarding the system architecture, cloud deployment procedures, and demonstration instructions for the Vitamin D prediction project.

## 1. architecture.md

Provides a detailed technical overview of the system's structural design and component interactions:

- Microservices architecture overview focusing on Java Spring Boot backend and React frontend.
- Data pipeline design incorporating Apache Kafka for real-time ingestion and Apache Spark for distributed processing.
- Machine Learning architecture detail, including Stacking ensemble configurations and SVM-SMOTE implementation.
- Storage strategy utilizing Amazon S3 for data lake operations and PostgreSQL for relational data management.

## 2. cloud_deployment_guide.md

A technical manual for deploying and scaling the application stack within cloud environments:

- Container orchestration guidelines for Kubernetes deployment.
- Step-by-step instructions for provisioning data infrastructure (Kafka, Spark, Airflow).
- Configuration of CI/CD pipelines through GitHub Actions for automated build and deployment.
- Management of environment variables and cloud-native security configurations.

## 3. demo_instructions.md

Practical guidance for accessing and evaluating the system demonstrations:

- User manual for the web-based Vitamin D prediction dashboard.
- Instructions for viewing the system operation video and navigating the feature set.
- Procedures for executing the end-to-end data pipeline demonstration.
- Guidelines for using provided test datasets to verify model inference results.
