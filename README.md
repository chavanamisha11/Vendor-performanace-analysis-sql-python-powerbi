# Vendor-performanace-analysis-sql-python-powerbi


# 🧾 Vendor Performance Analysis – Retail Inventory & Sales

*Analyzing vendor efficiency and profitability to support strategic purchasing and inventory decisions using SQL, Python, and Power BI.*

---

## 📌 Table of Contents

* [Overview](#overview)
* [Business Problem](#business-problem)
* [Dataset](#dataset)
* [Tools & Technologies](#tools--technologies)
* [Project Structure](#project-structure)
* [Data Cleaning & Preparation](#data-cleaning--preparation)
* [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
* [Research Questions & Key Findings](#research-questions--key-findings)
* [Dashboard](#dashboard)
* [How to Run This Project](#how-to-run-this-project)
* [Final Recommendations](#final-recommendations)

---

## 📊 Overview

This project evaluates vendor performance and retail inventory dynamics to generate insights for:

* Purchasing strategy
* Pricing decisions
* Inventory optimization

A full data pipeline is implemented using:

* SQL (ETL)
* Python (Analysis)
* Power BI (Visualization)

---

## 💼 Business Problem

Retail businesses often struggle with:

* Inefficient inventory management
* Vendor dependency risks
* Low-performing products

### Objectives:

* Identify underperforming brands
* Analyze vendor contribution to revenue
* Evaluate bulk purchasing benefits
* Detect inventory inefficiencies
* Compare vendor profitability statistically

---

## 📁 Dataset

* Multiple CSV files (`sales`, `vendors`, `inventory`)
* Stored in `/data/` folder
* Summary table created for analysis

---

## 🛠 Tools & Technologies

* **SQL** – Joins, CTEs, Filtering
* **Python** – Pandas, Matplotlib, Seaborn, SciPy
* **Power BI** – Dashboard & Visualization
* **GitHub** – Version control

---

## 📂 Project Structure

```
vendor-performance-analysis/
│
├── README.md
├── .gitignore
├── requirements.txt
├── Vendor Performance Report.pdf
│
├── notebooks/
│   ├── exploratory_data_analysis.ipynb
│   ├── vendor_performance_analysis.ipynb
│
├── scripts/
│   ├── ingestion_db.py
│   └── get_vendor_summary.py
│
├── dashboard/
│   └── vendor_performance_dashboard.pbix
```

---

## 🧹 Data Cleaning & Preparation

* Removed invalid records:

  * Gross Profit ≤ 0
  * Profit Margin ≤ 0
  * Sales Quantity = 0

* Created vendor-level summary tables

* Handled missing values and outliers

* Merged datasets

---

## 📈 Exploratory Data Analysis (EDA)

### Key Observations:

* Negative profit transactions detected
* Unsold inventory exists
* Outliers in freight and pricing

### Correlation Insights:

* Strong: Purchase Qty vs Sales Qty
* Weak: Purchase Price vs Profit
* Negative: Profit Margin vs Sales Price

---

## 🔍 Research Questions & Key Findings

1. **Low Sales, High Margin Brands**

   * ~198 brands identified → good for promotion

2. **Top Vendor Dependency**

   * Top 10 vendors contribute ~65% purchases

3. **Bulk Purchasing**

   * Up to 72% cost savings per unit

4. **Inventory Issues**

   * ~$2.71M unsold stock

5. **Vendor Profitability**

   * High vendors: ~31% margin
   * Low vendors: ~41% margin

6. **Hypothesis Testing**

   * Significant difference in vendor strategies

---

## 📊 Dashboard

Power BI dashboard includes:

* Vendor performance metrics
* Inventory turnover
* Profit margin analysis
* Heatmaps & trends

*(Add your dashboard image here)*

---

## ▶️ How to Run This Project

### 1. Clone repository

```bash
git clone https://github.com/yourusername/vendor-performance-analysis.git
```

### 2. Run data ingestion

```bash
python scripts/ingestion_db.py
```

### 3. Create summary table

```bash
python scripts/get_vendor_summary.py
```

### 4. Run notebooks

* exploratory_data_analysis.ipynb
* vendor_performance_analysis.ipynb

### 5. Open dashboard

* vendor_performance_dashboard.pbix

---

## ✅ Final Recommendations

* Diversify vendors to reduce risk
* Optimize bulk purchasing
* Improve pricing strategy
* Clear unsold inventory
* Boost marketing for low-performing brands

---

If you want next upgrade, I can:

* Add **GitHub badges (very important for portfolio)**
* Make it **ATS-friendly project description**
* Or create **one more strong project README** for your resume 🚀
