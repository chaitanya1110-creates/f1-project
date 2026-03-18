# 🏎️ F1 Data Engineering Pipeline

An automated end-to-end data pipeline that fetches Formula 1 driver statistics and race data via API, processes it using PySpark, and visualizes the results on a live dashboard.

🔗 **Live Project Site:** [View the F1 Leaderboard Here](https://chaitanya1110-creates.github.io/f1-project/)

---

## 🛠️ Tech Stack
* **Language:** Python (PySpark)
* **Platform:** Azure Databricks
* **Automation:** GitHub Actions
* **Frontend:** HTML/CSS (GitHub Pages)

## 🏗️ Project Architecture
1.  **Ingestion:** Python scripts pull real-time racing data from the Ergast API (or similar).
2.  **Transformation:** Data is cleaned and aggregated using **PySpark** on Databricks to calculate career points, wins, and podium percentages.
3.  **Loading:** The processed data is converted to JSON/CSV and pushed to this repository.
4.  **Deployment:** GitHub Pages automatically updates the frontend leaderboard based on the latest data.

## 📂 Repository Contents
* `/notebooks`: Contains the Databricks notebooks used for ETL (Extract, Transform, Load).
* `/data`: The processed output used by the website.
* `index.html`: The frontend interface for the project.

## 🚀 How to Run
1.  **Databricks Setup:** Import the notebooks found in the `/notebooks` folder into your Databricks workspace.
2.  **Cluster Config:** Ensure you are using a cluster with Spark 3.x support.
3.  **API Keys:** (If applicable) Add your API credentials to Databricks Secrets.
4.  **Run Pipeline:** Execute the notebooks in order (Ingestion -> Transformation).

---
*Created by Chaitanya Samudra*
