# 🚀 End-to-End Cloud Analytics & Machine Learning Pipeline

An enterprise-grade, end-to-end data pipeline built from scratch, integrating **Azure SQL**, **Python (Scikit-Learn / Pandas)**, and **Power BI** to analyze web traffic performance, marketing spend, and sales drivers.

---

## 📊 Dashboard Preview
> dashboard_screenshot.png

---

## 🛠️ Tech Stack & Architecture
* **Cloud Database:** Microsoft Azure SQL Server (`TrafficDB`)
* **Data Ingestion & Automation:** Python, Pandas, SQLAlchemy, ODBC Driver 18 for SQL Server
* **Machine Learning:** Scikit-Learn (Linear Regression model for feature importance & predictive analysis)
* **Advanced Analytics:** SQL Window Functions (`AVG() OVER` for rolling 7-day averages, ranking metrics)
* **Business Intelligence:** Power BI Desktop (Executive KPI cards, DAX measures, custom KPI ratios, tile slicers)

---

## 🔄 Project Pipeline Workflow

1. **Cloud Provisioning & Security:** 
   * Provisioned an Azure SQL database and configured network firewall rules to securely handle dynamic client IP routing.
2. **Data Generation & Ingestion:** 
   * Generated 90 days of structured mock web traffic and sales metrics in Python and programmatically pushed them straight into Azure via SQLAlchemy.
3. **Analytics & Machine Learning:** 
   * Queried data back to compute 7-day moving averages and top-performing conversion days using advanced SQL.
   * Trained a Scikit-Learn regression model to evaluate feature impacts (pageviews, bounce rates, and marketing spend) on actual sales.
4. **Business Intelligence (Power BI):** 
   * Connected Power BI directly to the Azure cloud database.
   * Developed explicit **DAX measures** (`Total Revenue`, `Total Pageviews`, `ROAS`, `Rev per 1K Views`, and `7-Day Rolling Averages`) and built an executive-ready visual canvas complete with interactive button slicers.

---

## 📈 Key Dashboard Metrics
* **Total Revenue (`₹307.14K`):** Evaluated dynamically alongside ad spend[cite: 5].
* **ROAS (`6.49`):** Measures overall marketing efficiency[cite: 5].
* **Rev per 1K Views (`328.71`):** Standard traffic monetization metric[cite: 5].
* **Rolling 7-Day Averages:** Smooths out daily noise to highlight true business trajectory.
