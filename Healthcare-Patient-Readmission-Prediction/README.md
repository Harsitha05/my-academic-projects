# Healthcare Patient Readmission Prediction and Analytics Using Databricks

## 📌 Project Overview

This project focuses on predicting hospital readmissions among diabetic patients using Machine Learning and Big Data technologies on the Databricks Lakehouse platform.

The project uses the **Diabetes 130-US Hospitals dataset**, containing 101,766 patient encounters and 50 attributes. It follows the Medallion Architecture (Bronze, Silver, and Gold) for data processing, feature engineering, model development, and evaluation.

The complete workflow is automated using Databricks Jobs, and the results are presented through an interactive Databricks AI/BI Dashboard.

## 🎓 Project Background

This is an academic mini project completed as part of the Master of Data Science programme at St. Joseph's College (Autonomous), Tiruchirappalli.

It provided practical experience in data engineering, big data processing, machine learning, workflow automation, and dashboard development using Databricks.

## 🎯 Project Objectives

- Process and analyze large-scale healthcare data.
- Implement Medallion Architecture using Delta Lake.
- Clean and transform raw patient records.
- Perform feature engineering using PySpark and Spark ML.
- Build and compare machine learning classification models.
- Automate the complete workflow using Databricks Jobs.
- Develop an interactive dashboard for healthcare analytics.

## 📊 Dataset Description

**Dataset:** Diabetes 130-US Hospitals for Years 1999–2008

**Source:** UCI Machine Learning Repository

| Dataset Details | Information |
|---|---|
| Patient encounters | 101,766 |
| Distinct patients | 71,518 |
| Original attributes | 50 |
| Target variable | Readmitted |
| Target classes | NO, >30, <30 |

The dataset contains patient demographics, admission details, hospital utilization, diagnoses, laboratory results, medication information, and readmission outcomes.

## 🛠️ Technologies Used

- **Databricks:** Development and execution platform
- **Apache Spark & PySpark:** Distributed data processing
- **Delta Lake:** Data storage
- **Unity Catalog:** Data organization and governance
- **Spark MLlib:** Feature engineering and machine learning
- **Databricks Jobs:** Workflow automation
- **Databricks AI/BI Dashboards:** Data visualization

## Project Implementation – Five Stages

### Stage 1: Bronze Layer – Data Ingestion

- Loaded the raw healthcare dataset into Databricks.
- Read the CSV file using PySpark.
- Checked the dataset structure, schema, and record count.
- Stored the original data as a Delta table.

**Output Table:** `bronze_diabetic_data`

### Stage 2: Silver Layer – Data Cleaning

- Identified missing values and '?' placeholders.
- Replaced missing categorical values with 'Unknown'.
- Standardized invalid gender values.
- Checked and handled duplicate records.
- Converted age ranges into numerical values.
- Removed identifier columns to avoid data leakage.

**Output Table:** `silver_patient_data`

### Stage 3: Gold Layer – Feature Engineering

- Prepared data for machine learning.
- Applied StringIndexer and OneHotEncoder.
- Standardized numerical features.
- Used VectorAssembler to combine features.
- Built a 41-stage Spark ML pipeline.
- Generated a 2,543-dimensional feature vector.

**Output Table:** `gold_patient_features`

### Stage 4: Machine Learning Pipeline

- Split the dataset into 80% training and 20% testing data.
- Developed Multinomial Logistic Regression.
- Developed Random Forest classification.
- Evaluated both models using accuracy, precision, recall, and weighted F1-score.
- Selected the model with the higher weighted F1-score.

**Output Table:** `readmission_predictions`

### Stage 5: Workflow Automation and Dashboard

- Created a Databricks Job named `Healthcare_Readmission_ML_Pipeline`.
- Connected all four notebooks through dependent tasks.
- Executed the complete pipeline using Databricks serverless compute.
- Developed an AI/BI Dashboard for healthcare analytics.
- Presented readmission statistics, patient insights, and model performance.

## 🤖 Machine Learning Models

Two classification algorithms were implemented:

1. **Multinomial Logistic Regression**
2. **Random Forest Classifier**

## 📈 Model Performance Comparison

| Evaluation Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 58.51% | 54.27% |
| Weighted Precision | 54.70% | 29.45% |
| Weighted Recall | 58.51% | 54.27% |
| Weighted F1-score | 0.5327 | 0.3818 |

**Selected Model:** Logistic Regression

Logistic Regression achieved better performance across all reported evaluation metrics and was selected as the final model.

## 📊 Dashboard Highlights

The Databricks AI/BI Dashboard contains four pages:

- Data
- Executive Overview
- Patient & Hospital Analysis
- ML Model Performance

**Key Dashboard Findings:**

| KPI | Value |
|---|---:|
| Total Patient Encounters | 101,766 |
| Not Readmitted | 54,864 |
| Readmitted After 30 Days | 35,545 |
| Readmitted Within 30 Days | 11,357 |
| Overall Readmission Rate | 46.09% |

## 🔍 Key Findings

- The complete Medallion pipeline processed 101,766 encounters without losing records.
- The dataset contained three readmission categories: NO, >30, and <30.
- Logistic Regression outperformed Random Forest.
- The final Logistic Regression model achieved 58.51% accuracy and a weighted F1-score of 0.5327.
- All four Databricks Job tasks completed successfully in the three recorded runs.
- The dashboard reported an overall readmission rate of 46.09%.

## 🚀 Future Scope

- Handle class imbalance using class weights or SMOTE.
- Explore additional machine learning algorithms.
- Perform hyperparameter tuning and cross-validation.
- Improve prediction performance for early readmission cases.
- Register and track models using MLflow.
- Develop real-time prediction capabilities.

## 👩‍💻 Project Information

**Project Title:** Healthcare Patient Readmission Prediction and Analytics Using Databricks

**Project Type:** Academic Mini Project

**Programme:** Master of Data Science

**Institution:** St. Joseph's College (Autonomous), Tiruchirappalli

**Year:** 2026
