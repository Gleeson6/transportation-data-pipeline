# transportation-data-pipeline
End-to-end data pipeline using Medallion Architecture (Bronze, Silver, Gold) with PySpark, Lakeflow, and S3, supporting incremental and continuous data processing.



# 🚀 Transportation Data Pipeline (Lakehouse Architecture)

## 📌 Overview
This project simulates a real-world cab transportation system and implements an end-to-end data pipeline using Medallion Architecture (Bronze, Silver, Gold).

The pipeline supports **incremental and full data loads** and runs as a **continuous pipeline**, automatically processing new data.

---

## 🏗️ Architecture

![Architecture](architecture/architecture.png)

---

## ⚙️ Tech Stack
- PySpark  
- Databricks (Lakeflow Declarative Pipelines)  
- AWS S3 (Data Lake)  
- Delta Lake  
- Unity Catalog  

---

## 🔄 Pipeline Design

### 🥉 Bronze Layer
- Ingests raw data from S3  
- Handles corrupt records  
- Adds metadata (file name, ingestion timestamp)

### 🥈 Silver Layer
- Cleans and transforms data  
- Builds calendar dimension  
- Adds business logic (holidays, weekdays, etc.)

### 🥇 Gold Layer
- Aggregations and analytics  
- Provides business-ready data  
- Used for dashboards and reporting  

---

## 🔁 Data Loading Strategy

- **Full Load** → Initial data ingestion  
- **Incremental Load** → Processes only new or updated data  

---

## 🔄 Continuous Pipeline
- Automatically processes new data  
- Event-driven architecture  
- Efficient incremental processing  

---

## 📊 Use Cases
- Trip trend analysis  
- Weekend vs weekday demand  
- Holiday-based insights


---

## 🎯 Key Highlights
- End-to-end data pipeline design  
- Medallion Architecture implementation  
- Incremental + continuous processing  
- Real-world simulation using S3 and Databricks  

---

---

## 📁 Project Structure

