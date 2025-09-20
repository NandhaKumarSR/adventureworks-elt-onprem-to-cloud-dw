# adventureworks-elt-onprem-to-cloud-dw

End-to-end pipeline using azure services - extracting AdventureWorks data from on-prem SQL Server, structured using medallion architecture, and visualized for enterprise reporting.

## 🚀 Overview

![project Architecture](./documentation/project-architecture.png)

- **Extract**: AdventureWorks data from on-prem SQL Server
- **Load**: Raw data ingested into Azure Data Lake (Bronze layer) via ADF
- **Transform**: Business logic applied in Databricks notebooks (Silver & Gold layers)
- **Model**: Views created in Azure Synapse Analytics
- **Visualize**: Power BI dashboard for customer insights
- **Automate**: Azure Logic App triggers Power BI dataset refresh post-pipeline

## 🧰 Tech Stack

- Azure Data Factory (ADF)
- Azure Databricks (ADB)
- Azure Synapse Analytics (ASA)
- Azure Logic Apps (ALA)
- Power BI
- GitHub (version-controlled repo)

## 📁 Repository Structure

```
adventureworks-etl-bi/
├── adb/                        # Azure Databricks notebooks (.ipynb)
├── adf/                        # Azure Data Factory pipeline templates
├── ala/                        # Azure Logic Apps templates
├── sql/                        # SQL scripts
├── pbi/                        # Power BI assets and dataset
├── documentation/
│   └── documentation.md        # Detailed architecture and walkthrough
│   └── screenshots/            # Project screenshots
├── LICENSE                     # MIT License
├── README.md                   # Project overview and repo guide
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
