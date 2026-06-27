# 📊 E-Commerce Sales Data Transformation & Modeling using Power BI

## 🚀 Project Summary

This project demonstrates a complete **data transformation and data modeling workflow** using **Microsoft Power BI**. 
The objective was to transform raw E-Commerce sales data into a clean, structured, and analysis-ready model by applying data cleaning, 
transformation, aggregation, and relationship modeling techniques in **Power Query** and **Power BI**.

The final data model is optimized for business reporting and serves as a strong foundation for building interactive dashboards and 
supporting data-driven decision-making.

---

## 📌 Problem Statement

Raw business data often contains inconsistent formatting, duplicate records, missing values, and disconnected datasets, 
making accurate analysis difficult.

This project addresses these challenges by preparing multiple datasets, integrating them into a unified data model, and 
ensuring data quality for effective business reporting.

---

## 📂 Dataset

The project consists of three datasets:

| Dataset               | Description                                |
| --------------------- | ------------------------------------------ |
| 📄 **List of Orders** | Customer and order-level sales information |
| 📄 **Order Details**  | Product-level transaction details          |
| 📄 **Sales Target**   | Monthly sales targets by category          |

---

# ⚙️ Data Preparation

### ✔ Data Import

* Imported multiple CSV files into Power BI.
* Loaded datasets into Power Query Editor.

### ✔ Data Cleaning

* Limited the Orders dataset to the first 500 records.
* Converted appropriate columns to Date and Fixed Decimal data types.
* Standardized customer names using Proper Case.
* Handled missing values and duplicate records.

### ✔ Data Transformation

* Created **Location** by combining City and State.

  **Location = [city]&", "&[State]**
  
* Calculated **Profit Margin (%)** by using formula.

  **Profit Margin = [Profit] / [Amount]**
  
* Created a **Profit Status** column using business rules
    Condition	Status
  
       Profit < 0	Loss
  
       Profit = 0	Break-Even
  
       Profit > 0	Profit
  
* Merged Orders and Order Details using **Order ID**.
  
* Sorted and filtered data for business analysis.

### ✔ Data Aggregation

Generated summary tables including:

* Order Count for each order
  
* Average Profit($) by Category
  
             Furniture   - 9.46
  
             Clothing    - 11.76
  
             Electronics - 34.07


* Total Amount by Sub-Category
  
* Monthly Sales Target Summary

---

# 🔗 Data Modeling

Created relationships between datasets to enable efficient reporting.

| Relationship                   | Key            |
| ------------------------------ | -------------- |
| List of Orders → Order Details | Order ID (1:*) |
| Order Details → Sales Target   | Category (*:*) |

---

# 📈 Business Value

The prepared data model enables:

* 📌 Sales performance analysis
* 📌 Profitability analysis
* 📌 Regional sales analysis
* 📌 Category-wise performance tracking
* 📌 Monthly sales target monitoring
* 📌 Reliable business reporting

---

# 🛠️ Tools & Technologies

* Microsoft Power BI
* Power Query Editor
* Data Modeling
* CSV Files

---

# 💡 Skills Demonstrated

* Data Cleaning
* Data Transformation
* Power Query
* Data Modeling
* Data Aggregation
* Relationship Modeling
* Business Analysis
* Power BI

---

# 📷 Data Model Preview


<img width="1395" height="547" alt="image" src="https://github.com/user-attachments/assets/ee235b0f-b466-461c-aa91-09183f78d575" />








# 📁 Repository Structure

```
📦 E-Commerce-Sales-PowerBI
│
├── 📄 README.md
├── 📄 E-Commerce Sales.pbix
├── 📄 Data Transformation & Modeling Report.pdf
├── 📁 Dataset
│   ├── List of Orders.csv
│   ├── Order Details.csv
│   └── Sales Target.csv
└── 📁 Images
    └── Dashboard.png
```

---

## 🎯 Key Takeaways

* Prepared and transformed raw E-Commerce data into an analysis-ready model.
* Applied Power Query transformations to improve data quality and consistency.
* Built relationships across multiple datasets for accurate reporting.
* Generated business-ready summaries to support interactive dashboard development.

---

## 👤 Author

**Sabana Asmi**

**Aspiring Data Analyst**

**Skills:** Excel • SQL • Power BI • Python
