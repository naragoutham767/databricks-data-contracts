# Data Contract Compliance & Validation System

This project demonstrates a dynamic **data contract validation system** built on **Databricks Delta Lake**.  
It ensures vendor data feeds adhere to schema, constraint, and frequency rules using a config-driven approach.

## 🚀 Features
- Dynamic schema and constraint validation from JSON config.
- Auditable data ingestion pipeline using Delta Lake.
- Automatic compliance report generation.
- Designed for multi-partner, multi-schema data feeds.

## 🏗️ Architecture
```
Partner Source → Raw Zone (S3/ADLS)
                ↓
          Validation Layer (PySpark)
                ↓
         Harmonized Zone (Delta)
                ↓
     Compliance Reports (Delta + SQL)
                ↓
        Power BI / QuickSight
```

## 🧠 How to Run
1. Update `configs/partner_contracts.json` with your partner definitions.
2. Upload sample data into `sample_data/` or external location (e.g., S3 path).
3. Run notebooks in order (01–05).
4. View compliance results in Databricks SQL or BI dashboard.

---
© 2025 Goutham Nara | Senior Specialist Data Engineer
