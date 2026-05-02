# Project 4: Real-Time Anomaly Detection & Alerting System (IoT / Time-Series)

## Project Overview

Develop a cloud‑based anomaly detection system for streaming IoT sensor data. The system must detect anomalies in real time, trigger alerts, and provide analytics dashboards.

## Dataset: PRIDE (Personal Risk Detection) Dataset

![PRIDE Dataset](images/images_3.jpeg.webp)

### Dataset Description

We define personal risk detection as the timely identification of when someone is in the midst of a dangerous situation, for example, a health crisis or a car accident, events that may jeopardize a person's physical integrity. We work under the hypothesis that a risk-prone situation produces sudden and significant deviations in standard physiological and behavioural user patterns. These changes can be captured by a group of sensors, such as the accelerometer, gyroscope, and heart rate.

The PRIDE (Personal Risk Detection) dataset is built with the help of 18 test subjects and a period of data collection of one week each, 24 h per day; the normal conditions dataset (NCDS) is built in this manner. Next, to build the anomaly conditions dataset (ACDS), the same 18 test subjects collaborate in another process to gather data under specific abnormal or stressful conditions. The scenarios include activities such as running several meters, going up and down the stairs of a several-floor building as fast as possible, simulating a fight, and so on.

### Dataset Sources

- **IEEE DataPort**: [PRIDE Dataset - IEEE DataPort](https://ieee-dataport.org/documents/pride-personal-risk-detection-dataset)
- **Azure Blob Storage**: [Download PRIDE Dataset](https://prideproject.blob.core.windows.net/pridedataset/PRIDE%20dataset-20260502T121502Z-3-001.zip?sp=r&st=2026-05-02T19:09:41Z&se=2026-08-01T03:24:41Z&spr=https&sv=2025-11-05&sr=b&sig=FClSrULjVFNIga5MjkEdsXZ%2BjCy%2F39cJoU3p1wSVZlg%3D)

## Milestone 1: Data Collection, Preprocessing, and Exploration

### Objectives

• Collect real or simulated time‑series IoT data
• Preprocess and explore seasonal patterns and noise

### Tasks

1. **Data Collection:**
   a. Ingest data from multiple sensors (temperature, pressure, etc.) via simulated streams or public IoT datasets.
   b. Store raw data in Azure Data Lake or Blob Storage.

2. **Data Preprocessing:**
   a. Handle missing values, smoothing, and window segmentation.
   b. Create engineered features (lag features, rolling means).

3. **Exploratory Data Analysis (EDA):**
   a. Analyze trends, seasonal effects, and noise patterns.
   b. Identify baseline normal behavior and potential anomalies.

### Deliverables

• Cleaned and Structured Time‑Series Dataset
• Data Preprocessing Pipeline Documentation
• EDA Report with Visualizations

## Milestone 2: Model Development & Evaluation

### Objectives

• Train reliable anomaly detection models suitable for streaming data

### Tasks

1. **Model Development:**
   a. Implement models such as LSTM Autoencoders, Isolation Forests, or Prophet‑based threshold detection.

2. **Evaluation:**
   a. Evaluate using precision, recall, F1‑score for anomaly classes.
   b. Test on held‑out test sets and synthetic anomalies.

3. **Optimization:**
   a. Adjust thresholds and retrain pipelines for robustness.

### Deliverables

• Trained Anomaly Detection Models
• Model Evaluation Report

## Milestone 3: Advanced Techniques & Cloud Integration

### Objectives

• Deploy the model in real time on Azure

### Tasks

1. **Cloud Deployment:**
   a. Use Azure Stream Analytics and Azure Functions for real‑time scoring.
   b. Containerize model inference with Docker deployed through Azure Container Instances.

2. **REST API:**
   a. Build a REST API for real‑time anomaly scoring.

3. **Integration:**
   a. Integrate with Azure Event Hubs for stream ingestion.

### Deliverables

• Deployed Real‑Time Anomaly Detection Service
• Real‑Time API Endpoints

## Milestone 4: MLOps, Monitoring, & Dashboard

### Objectives

• Implement production‑grade monitoring, alerts, and retraining automation

### Tasks

1. **MLOps Tracking:**
   a. Track model versions and experiments with MLflow or Azure ML.

2. **Monitoring:**
   a. Use Azure Monitor and custom metrics for drift and performance monitoring.

3. **Dashboard:**
   a. Build a dashboard (Power BI or Grafana) showing anomaly rates in real time.

4. **Retraining Plan:**
   a. Set up scheduled retraining pipelines triggered by drift detection.

### Deliverables

• Monitoring & Alerting Setup
• Dashboard & KPI Visualization
• MLOps Pipeline Documentation

## Milestone 5: Final Documentation & Presentation

### Objectives

• Summarize and demonstrate end‑to‑end solution

### Tasks

1. **Final Report:**
   a. Document pipeline, deployment, challenges, and business impact.

2. **Presentation:**
   a. Live demo of streaming anomaly detection with alerts and dashboards.

3. **Future Enhancements:**
   a. Propose edge deployment optimization or predictive maintenance features.

### Deliverables

• Final Project Report
• Final Presentation Deck
• Future Improvements Document
