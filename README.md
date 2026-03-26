# walmart-sales-analytics-sql-powerbi
End-to-end Walmart Sales Analytics project using SQL and Power BI. Includes data cleaning, transformation, and interactive dashboards to analyze sales trends, store performance, and business drivers.
# 🛒 Walmart Sales Analytics (SQL + Power BI)

## 📌 Project Overview

This project is an end-to-end **Retail Sales Analytics solution** built using the Walmart Sales dataset. It focuses on analyzing **sales trends, store performance, holiday impact, and key business drivers** using SQL and Power BI.

The project demonstrates strong capabilities in **data cleaning, transformation, and visualization**, enabling data-driven decision-making for retail businesses.

---

## 🎯 Objectives

* Analyze weekly and monthly sales trends
* Compare holiday vs non-holiday sales performance
* Identify top-performing stores
* Understand external factors (temperature, fuel price, CPI, unemployment)
* Provide actionable business insights

---

## 🛠️ Tech Stack

* **SQL (MySQL)** → Data cleaning, transformation, feature engineering
* **Power BI** → Dashboard development & visualization
* **Power Query** → Data preparation
* **DAX** → KPI calculations and measures

---

## 📂 Dataset

* Source: Walmart Sales Dataset [https://www.kaggle.com/datasets/mikhail1681/walmart-sales](Kaggle)
* Features:

  * Store ID
  * Weekly Sales
  * Holiday Flag
  * Temperature
  * Fuel Price
  * CPI
  * Unemployment Rate
  * Date

---

## 🗄️ SQL Data Processing

### 🔹 Database & Table Creation

* Created structured database and table for raw data storage

### 🔹 Data Cleaning & Transformation

* Converted string date into proper DATE format
* Extracted:

  * Month
  * Year
  * Day name
* Created **holiday_type** column
* Handled null and duplicate checks

### 🔹 Feature Engineering

* Added derived columns:

  * `month_name`
  * `year`
  * `day_name`
  * `holiday_type`

### 🔹 View Creation

* Created a clean dataset using SQL view:

```sql
CREATE VIEW sales_cleaned AS
SELECT 
    store,
    order_date,
    weekly_sales,
    holiday_type,
    temperature,
    fuel_price,
    cpi,
    unemployment,
    month_name,
    year,
    day_name
FROM walmart_sales;
```

---

## 📊 Dashboard Features

### 🔹 Executive Overview

* Total Sales: $6.7B
* Avg Weekly Sales: $1.05M
* Avg CPI: 171.58
* Total Stores: 45
* Holiday Sales %: 7.5%

---

### 🔹 Key Visualizations

* 📈 Sales Trend Over Time
* 📅 Monthly Sales Trend
* 🏬 Top 10 Performing Stores
* 🎯 Holiday vs Non-Holiday Sales
* 🌡️ Temperature vs Sales (Scatter Plot)
* 📊 Store Contribution (Waterfall Chart)
* 🔥 Sales Heatmap (Store vs Month)
* 📉 Store Performance Rank Trend

---

## 🧠 Key Insights

* Majority of sales occur during non-holiday periods
* Certain stores consistently outperform others
* Seasonal trends impact sales significantly
* External economic factors influence sales behavior
* Sales distribution is concentrated among top-performing stores

---

## 🔄 Project Workflow

1. Data Collection (Kaggle dataset)
2. Database Creation (MySQL)
3. Data Cleaning & Transformation (SQL)
4. Feature Engineering (SQL)
5. Data Visualization (Power BI)
6. Insight Generation

---



## 📁 Repository Structure

```id="v2k9pz"
├── data/                # Raw dataset
├── sql/                 # SQL scripts
├── dashboard/           # Power BI (.pbix file)
├── images/              # Dashboard screenshots
└── README.md
```

---

## 🚀 How to Run the Project

1. Import dataset into MySQL
2. Execute SQL scripts for data cleaning & transformation
3. Connect Power BI to SQL database
4. Build or open the dashboard file
5. Explore insights

---

## 📌 Future Enhancements

* Add predictive sales forecasting
* Build machine learning model
* Deploy dashboard online
* Add real-time data integration

---

## 🤝 Contributions

Contributions are welcome! Feel free to fork and improve the project.

---

## 📧 Contact

* LinkedIn: (https://www.linkedin.com/in/shreya-patil-322177306/)
* Email: (patilshreya055@gmail.com)

---

⭐ If you found this project useful, consider giving it a star!
