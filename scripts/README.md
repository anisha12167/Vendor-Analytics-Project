# 📊 Vendor Performance Analysis – Retail Inventory & Sales

Analyzing vendor efficiency and profitability to support strategic purchasing and inventory decisions using **SQL, Python, and Power BI**.

---

## 📌 Table of Contents
- Overview  
- Business Problem  
- Dataset  
- Tools & Technologies  
- Project Structure  
- Data Cleaning & Preparation  
- Exploratory Data Analysis (EDA)  
- Research Questions & Key Findings  
- Dashboard  
- How to Run This Project  
- Final Recommendations  
- Author & Contact  

---

## 📖 Overview
This project evaluates vendor performance and retail inventory dynamics to generate strategic insights for purchasing, pricing, and inventory optimization. A complete data pipeline was developed using SQL for ETL operations, Python for data analysis and statistical testing, and Power BI for interactive dashboard visualization.

---

## 💼 Business Problem
Retail organizations must optimize vendor selection and inventory strategies to maximize profitability. This project focuses on:

- Identifying underperforming brands requiring promotional or pricing changes  
- Measuring vendor contributions to total sales and profit  
- Evaluating financial benefits of bulk purchasing  
- Detecting inefficiencies in inventory turnover  
- Statistically validating differences in vendor profitability  

---

## 📁 Dataset
The dataset consists of multiple CSV files containing:

- Sales Transactions  
- Vendor Information  
- Inventory Records  
- Purchase Data  

All raw datasets are stored inside the **`data/`** directory and ingested into a SQLite database for analysis.

---

## 🛠 Tools & Technologies
- **SQL** – CTEs, Joins, Aggregations  
- **Python**
  - Pandas  
  - NumPy  
  - Matplotlib  
  - Seaborn  
  - SciPy (Hypothesis Testing)  
- **SQLite** – Database Management  
- **Power BI** – Dashboard Visualization  
- **GitHub** – Version Control  

---

## 📂 Project Structure
Vendor-Analytics-Project/
│
├── notebooks/
│ ├── Exploratory Data Analysis.ipynb
│ └── Vendor Performance Analysis.ipynb
│
├── scripts/
│ ├── ingestion_db.py
│ └── get_vendor_summary.py
│
├── dashboard/
│ └── vendor_performance.pbix
│
├── README.md
└── requirements.txt


---

## 🧹 Data Cleaning & Preparation
The following preprocessing steps were performed:

- Removed transactions with:
  - Negative or zero gross profit
  - Negative or zero profit margins
  - Zero sales quantity
- Handled missing values and corrected data types
- Merged multiple tables for vendor-level performance metrics
- Generated calculated fields for profitability and inventory performance

---

## 📈 Exploratory Data Analysis (EDA)

### 🔍 Key Observations

#### Negative / Zero Values
- Minimum Gross Profit recorded: **-52,002.78**
- Negative and infinite profit margins observed due to loss-making transactions
- Presence of unsold inventory indicating slow-moving stock

#### Outlier Detection
- Freight costs reaching up to **257K**
- Large variation in purchase and selling prices

#### Correlation Insights
- Weak correlation between purchase price and profit
- Strong correlation between purchase quantity and sales quantity (**0.999**)
- Slight negative correlation between sales price and profit margin (**-0.179**)

---

## ❓ Research Questions & Key Findings

### 📌 Promotional Opportunities
- Identified **198 brands** with low sales but high profit margins

### 📌 Vendor Concentration Risk
- Top 10 vendors contributed **65.69%** of total purchases

### 📌 Bulk Purchasing Efficiency
- Bulk purchases resulted in approximately **72% unit cost savings**

### 📌 Inventory Turnover
- Approximately **$2.71M** worth of inventory remained unsold

### 📌 Vendor Profitability Comparison
- High-performing vendors average margin: **31.17%**
- Low-performing vendors average margin: **41.55%**

### 📌 Hypothesis Testing
Statistical testing confirmed a significant difference in profit margins between high-performing and low-performing vendors, indicating distinct pricing and operational strategies.

---

## 📊 Dashboard
The Power BI dashboard provides:

- Vendor-wise Sales & Profit Margin Analysis  
- Inventory Turnover Monitoring  
- Bulk Purchase Cost Savings Visualization  
- Vendor Performance Heatmaps  

📂 Dashboard File:
dashboard/vendor_performance.pbix

---

## ▶ How to Run This Project

### 1️⃣ Clone Repository
git clone https://github.com/anisha12167/Vendor-Analytics-Project.git

### 2️⃣ Install Required Libraries

### 3️⃣ Load Raw Data into Database

### 4️⃣ Generate Vendor Summary Table

### 5️⃣ Run Analysis Notebooks
- notebooks/Exploratory Data Analysis.ipynb  
- notebooks/Vendor Performance Analysis.ipynb  

### 6️⃣ Open Power BI Dashboard
- dashboard/vendor_performance.pbix  

---

##  Final Recommendations
- Diversify vendor portfolio to reduce supplier dependency
- Increase bulk purchasing for high-demand products
- Adjust pricing strategy for slow-moving high-margin products
- Implement targeted marketing strategies for low-performing vendors
- Improve inventory monitoring to reduce unsold stock

---

##  Author & Contact

**Anisha Saini**  
Aspiring Data Analyst  

📧 Email: v.saini685@gmail.com
🔗 GitHub: https://github.com/anisha12167
