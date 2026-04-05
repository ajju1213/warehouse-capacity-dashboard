# 🏭 Warehouse Utilization Analytics Dashboard
Power BI solution to monitor warehouse capacity utilization across multiple categories (MAIN, ONLINE, RETURN, OVERALL), featuring overload detection, threshold tracking, and dynamic DAX-driven insights using SAP MB52 data.

## 📊 Project Overview

This Power BI dashboard provides end-to-end visibility into warehouse utilization at both PAN India and warehouse level using Microsoft Power BI and data from SAP MB52.

### 🚀 It enables:

- Monitoring of stock levels and pending dispatch across categories (MAIN, ONLINE, RETURN)  
- Capacity utilization tracking to measure warehouse efficiency  
- Identification of overloaded warehouses based on utilization thresholds  
- Daily risk monitoring with threshold alerts (90%+ utilization)  
- Dynamic KPI tracking for stock, dispatch, and capacity metrics  

### ⚙️ Solution Approach

The solution is built using a scalable folder-based ingestion approach, making it suitable for automated daily operational reporting.

---

## 🚀 Key Features

- 📂 Folder-based automatic data ingestion  
- 📅 Daily warehouse tracking  
- 📊 Category-wise analysis (MAIN / ONLINE / RETURN / OVERALL)  
- 📈 Capacity Utilization % with dynamic context  
- 🚨 Overload detection (>100%)  
- ⚠️ 90% threshold tracking (risk monitoring)  
- 🌍 Warehouse-level & PAN India insights  
- 🎯 KPI cards with gauge visuals  
- 🔄 Pending dispatch impact on utilization  
- 🟢 Status indicators (Safe / Warning / Overloaded)  

---

## 🛠 Tools & Technologies Used

- 🟡 Microsoft Power BI  
- 🔵 DAX (Data Analysis Expressions)  
- ⚙️ Power Query (ETL)  
- 🧩 Data Modeling (Star Schema)  
- 📂 Folder-based Data Ingestion  
- 📊 Excel (SAP MB52 Data Source)  

---

## 🧠 Core DAX Logic

- ⚙️ Dynamic measures using `HASONEVALUE` and `REMOVEFILTERS`  
- 📦 Category-level stock calculations (MAIN / ONLINE / RETURN)  
- 🔄 Combined OVERALL stock calculation (including dispatch impact)  
- ⚖️ Capacity vs Stock comparison for utilization analysis  
- 🚦 Threshold-based status classification (Safe / Warning / Overloaded)  

---
## 📊 Key Metrics

- 📦 Total Stock (Category-wise & Overall)  
- 📈 Capacity Utilization %  
- 🟢 Free Capacity  
- 🚚 Pending Dispatch Stock  
- 🚨 Overloaded Warehouse Count  
- ⚠️ 90%+ Utilization Tracking  
- 🧩 Category Contribution %  

## 🗂 Project Structure
```

warehouse-utilization-analytics/
│
├── Warehouse_Utilization_Dashboard.pbix
├── Sample_Data/
│   ├── Stock_Sample.xlsx
│   └── Pending_Dispatch.xlsx
├── screenshots/
│   ├── dashboard.jpeg
│   └── datamodel_view.jpeg
└── README.md
```
---
## 📷 Dashboard Preview

![Dashboard](screenshots/dashboard.jpeg)
![Data Model](screenshots/datamodel_view.jpeg)



---

## 📌 Business Logic

Capacity Utilization % =  
(Total Stock + Pending Dispatch) ÷ Capacity

Status Classification:
- >100% → Overloaded
- 75–100% → Warning
- <75% → Safe

---

## 🔄 Daily Refresh Process

1. Export MB52 from SAP
2. Save file in Raw Data folder
3. Open Power BI file
4. Click Refresh
5. Analyze utilization & overload risks

---

## 📚 Learning Outcomes

- 🧠 Built dynamic DAX measures with context handling  
- 📊 Implemented category-wise analytical data model  
- 📂 Designed scalable data ingestion pipeline  
- 🎯 Developed KPI-driven dashboard for operations  
- 💼 Applied business logic for warehouse optimization  

---

## ⚠ Disclaimer

This project uses sample data for demonstration purposes only.  
No confidential or real business data is included.

---

## 📬 Connect With Me

If you found this project useful, feel free to connect or reach out:

- 💼 LinkedIn: https://linkedin.com/in/ajay-pal-95a96510b  
- 📧 Email: ajaykumarpal1993@gmail.com  
   
