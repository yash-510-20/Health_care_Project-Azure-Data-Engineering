# Health_care_Project-Azure-Data-Engineering

## 🏥 Project Overview
End-to-End Azure Data Engineering project using real healthcare datasets.

## 🛠️ Technology Stack
- **Azure Data Factory (ADF)** — Data ingestion & orchestration
- **Azure Data Lake Storage Gen2 (ADLS)** — Cloud storage
- **Azure Synapse Analytics** — Spark processing + SQL analytics
- **PySpark** — Data transformation
- **GitHub** — Source control

## 🗺️ Architecture
```
CSV Files → ADF Pipeline → ADLS Bronze → Synapse Spark → Silver → Gold → Synapse SQL
```

## 📁 Layers
| Layer | Purpose |
|---|---|
| Bronze | Raw data exactly as received |
| Silver | Cleaned, validated, joined data |
| Gold | Star Schema — Fact + Dimension tables |

## ⭐ Star Schema
- Fact_Patient_Visit
- Dim_Patient (SCD Type 2)
- Dim_Doctor (SCD Type 2)
- Dim_Department
- Dim_Diagnosis
- Dim_Date

## 📊 Dataset
- 100 Patients
- 275 Hospital Visits
- 4,506 Diagnoses
- 109,282 ICD Codes
- 10 Doctors
- 10 Departments
