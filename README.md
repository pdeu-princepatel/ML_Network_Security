# 🛡️ Network Security Project for Phishing Data

A comprehensive **Machine Learning pipeline** designed to detect phishing attacks through automated **ETL (Extract, Transform, Load)** processes, **data validation**, and **data transformation** steps, implemented in Python. This project leverages modular design principles to ensure flexibility, scalability, and maintainability in detecting phishing-related anomalies in network data.

---

## 🚀 Key Features

- 📦 **End-to-End ML Pipeline**: From ingestion to transformation
- 📁 Modular architecture with reusable components
- 🧪 Data validation with schema checks
- 🔄 Scalable ETL pipeline
- 🐍 Written entirely in Python
- 🧾 Logging & exception handling for full traceability

---

## 🗂️ Project Structure


---

## 🔁 Pipeline Overview

Your `main.py` handles the following:

1. **Data Ingestion**  
   Loads data (likely from MongoDB or local CSV) and stores it in the project.

2. **Data Validation**  
   Validates ingested data against a predefined schema in `data_schema/`.

3. **Data Transformation**  
   Processes and transforms the clean data for model readiness (e.g., encoding, scaling).

All steps are modular and configurable via:
```python
from networksecurity.components import DataIngestion, DataValidation, DataTransformation
from networksecurity.entity.config_entity import (
    DataIngestionConfig, DataValidationConfig, DataTransformationConfig, TrainingPipelineConfig
)
