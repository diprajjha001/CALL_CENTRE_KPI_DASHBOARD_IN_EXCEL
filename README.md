# 📊 Call Center Performance Dashboard (Excel Project)

## 📌 Project Overview
This project is an **interactive Call Center Dashboard built using Microsoft Excel**.  
It analyzes call center operations for the year **2025**, providing actionable insights into call volume, revenue, call duration, and customer satisfaction.

The dashboard helps management **monitor performance, identify inefficiencies, and improve customer experience** using data-driven KPIs.

---

## 🗂️ Dataset Description
**Source File:** `call_center_sample_data_2025.xlsx`

### Key Data Fields
- Call Number
- Customer ID
- Call Duration (mins)
- Purchase Amount
- Satisfaction Rating
- Representative
- Date of Call
- Day of Week
- Duration Bucket
- Gender, Age, City

---

## 📈 KPIs Displayed on the Dashboard

| KPI | Description |
|----|------------|
| **Total Call Count** | Total number of calls handled |
| **Total Revenue** | Sum of purchase amounts generated |
| **Total Call Duration** | Total time spent on calls (minutes) |
| **Average Satisfaction Rating** | Mean customer satisfaction score |
| **5-Star Calls** | Number of calls rated 5 stars |

---

## 🧮 Excel Formulas Used

### 1️⃣ Total Call Count
```excel
=COUNTA('call_center_sample_data_2025'!A:A)
Counts all non-empty Call Numbers.

2️⃣ Total Revenue
=SUM('call_center_sample_data_2025'!F:F)
Adds all purchase amounts.

3️⃣ Total Call Duration
=SUM('call_center_sample_data_2025'!C:C)
Calculates total call handling time.
4️⃣ Average Satisfaction Rating
=AVERAGE('call_center_sample_data_2025'!G:G)

Finds the mean customer satisfaction score.

5️⃣ 5-Star Call Count
=COUNTIF('call_center_sample_data_2025'!J:J,5)

Counts calls with a rounded rating of 5.

🔄 Data Processing & Excel Functions
Helper Columns
Rating Rounded
=ROUND([@[Satisfaction Rating]],0)

Duration Bucket
=IFS(
C2<=30,"0–30 mins",
C2<=60,"30–60 mins",
C2<=120,"1–2 hours",
C2>120,"More than 2 hours"
)

📊 Pivot Tables Used
The PIVOTS sheet contains multiple pivot tables:
Examples:
Calls by Day of Week
Revenue by City
Average Rating by Representative
Call Volume by Duration Bucket
Pivot Settings Used:
Values summarized by SUM, COUNT, AVERAGE
Report Layout: Tabular Form
Number Formatting applied
Filters connected to slicers

🎛️ Dashboard Interactivity
Excel Features Used
Slicers for:
City
Gender
Day of Week
Representative
Pivot Charts
Column Charts
Bar Charts
Donut Charts
Card-style KPI visuals
Consistent color theme & icons
All slicers are connected to multiple pivot tables using:

Report Connections
🚀 Business Problems Solved
❌ Problems

No visibility into call center performance
Difficult to track customer satisfaction
Manual reporting was time-consuming
No way to compare agent performance

✅ Solutions Provided

Real-time KPI monitoring
Identification of peak call days & long calls
Performance comparison across agents & cities
Better decision-making using customer ratings

🛠 Tools & Technologies

Microsoft Excel
Pivot Tables & Pivot Charts
Slicers
Advanced Excel Formulas
Dashboard Design Best Practices

📌 Final Outcome

This Excel dashboard transforms raw call center data into clear, interactive, and decision-ready insights, helping stakeholders improve efficiency, revenue, and customer satisfaction.

📁 Repository Structure
📦 Call-Center-Dashboard
 ┣ 📊 call_center_sample_data_2025.xlsx
 ┣ 📄 README.md
✨ Author

Excel Data Analytics Project
