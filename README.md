# 📊 Blinkit Sales Performance Analysis – Power BI Dashboard  
A complete end-to-end data analytics case study analyzing Blinkit's grocery sales using Power BI, DAX, & Power Query.

![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Made With](https://img.shields.io/badge/Made%20With-Power%20Query%20%7C%20DAX%20%7C%20Power%20BI-blue)

---

## 🚀 Project Overview  
This project presents an interactive **Power BI dashboard** analyzing Blinkit’s sales across outlet types, item categories, fat content groups, and customer ratings.

It highlights:

- Key KPIs  
- Sales trends  
- Category performance  
- Outlet performance  
- Consumer preferences  
- Actionable insights & recommendations  

This project showcases skills in **data cleaning, modeling, visualization, DAX, and business analysis.**

---

## 🎯 Business Questions Answered  
- Which item categories contribute most to sales?  
- Which outlet locations (Tier 1/2/3) perform best?  
- Do Low Fat or Regular products impact sales differently?  
- What is the trend of sales over the years?  
- What outlets or categories underperform?  
- What business improvements can be recommended?

---

## 🧹 Data Cleaning & Preparation  
Performed using **Power Query**:

- Removed duplicates & missing values  
- Cleaned inconsistent labels (Low Fat, Regular)  
- Corrected data types  
- Cleaned Outlet Size & Location Tier fields  
- Prepared a clean analysis-ready dataset  

---
## 🔢 Key DAX Measures

```DAX
-- Basic KPIs
Total Sales = SUM('BlinkIT Grocery Data'[Item_Outlet_Sales])

Avg Sales = AVERAGE('BlinkIT Grocery Data'[Item_Outlet_Sales])

No of Items Sold = SUM('BlinkIT Grocery Data'[Quantity])

Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

-- Contribution %
Contribution % =
DIVIDE([Total Sales], CALCULATE([Total Sales], ALL('BlinkIT Grocery Data')))

-- Weighted revenue by rating
Rating Weighted Sales =
SUMX(
  'BlinkIT Grocery Data',
  'BlinkIT Grocery Data'[Item_Outlet_Sales] * 'BlinkIT Grocery Data'[Rating]
)

---



## 📊 Dashboard Overview

🟨 Full Dashboard Screenshot

<img src="assets/A Blinkit screenshot.png" width="900"/>

## 🔍 Close-Up Insights

### ⭐ 1. KPI Insights

<img src="assets/KPI.png" width="500"/>

**Insights**
- Total Sales: **$1.20M+**
- Average Sales per Item: **$141**
- Total Items Sold: **8,500+**
- Average Rating: **3.92**


###⭐ 2. Item Type Insights

<img src="assets/item_type.png" width="300"/>

**Insights**
- **Fruits & Vegetables** and **Snacks** generate the highest revenue.
- **Household** and **Frozen Foods** show strong performance.
- **Seafood**, **Breakfast**, and **Hard Drinks** are the lowest-performing categories.
- Consider targeted marketing or repositioning for underperforming categories.

###⭐ 3. Fat Content Insights

<img src="assets/fat_content.png" width="350"/>

**Insights**
- **Low Fat** items contribute the majority of revenue.
- Clear customer preference for Low Fat products.
- Regular products show lower overall performance but still contribute meaningfully.
- Opportunity exists for promotions on Regular products to increase balance.


###⭐ 4. Fat by Outlet Tier

<img src="assets/fat_by_outlet.png" width="300"/>

**Insights**
- **Tier 3** outlets outperform Tier 1 & Tier 2 in total sales.
- Both **Low Fat** and **Regular** items sell highest in Tier 3 stores.
- Tier 1 & Tier 2 outlets show lower conversion, indicating improvement potential.
- Opportunity to expand product variety in Tier 3 stores for even higher gains.


###⭐ 5. Sales Trend Over Time

<img src="assets/outlet_establishment.png" width="500"/>

**Insights**
- Sales show consistent year-over-year growth.
- Revenue peaks appear in **2017** and **2020**.
- Seasonal patterns suggest higher demand during festival periods.
- Stable growth trend indicates strong customer retention and product acceptance.

## 💡 Key Insights (Summary)

### 🔸 Sales Trends
- Consistent upward sales trend, with major peaks in **2017** and **2020**.

### 🔸 Product Insights
- **Low Fat** items dominate revenue.
- Top-performing categories: **Fruits & Vegetables**, **Snacks**, **Household**.
- Underperforming categories: **Seafood**, **Hard Drinks**, **Breakfast**.

### 🔸 Outlet Insights
- **Tier 3** outlets generate the highest sales.
- Medium-sized outlets outperform small and large outlets.

### 🔸 Customer Behavior
- Strong overall customer satisfaction with an average rating of **3.92**.


## 🧭 Recommendations
- ✔ **Expand in Tier 3 locations** — strongest revenue potential.
- ✔ **Focus on medium-sized outlets** — best performance for scaling.
- ✔ **Promote Low Fat products** — high demand; ideal for bundles or discounts.
- ✔ **Improve low-performing categories** — use marketing offers or repositioning.
- ✔ **Enhance customer experience** — improve service in lower-rated stores.

## 📝 Project Summary

This project provides a complete sales performance analysis for Blinkit using Power BI.  
It covers data cleaning, modeling, and visualization to uncover trends across product categories, outlet tiers, fat content, and customer ratings.  
Interactive dashboards enable business users to identify top-performing segments, understand customer behavior, and make data-driven decisions.

The project demonstrates strong analytical thinking, dashboard storytelling, and end-to-end BI development — from raw data to actionable insights.

## 🛠 Tools & Technologies

- **Power BI Desktop**
- **Power Query** (Data Cleaning & Transformation)
- **DAX** (Measure Creation & KPI Development)
- **Excel** (Initial Data Exploration)
- **Data Modeling** (Star Schema, Relationships)
- **Data Visualization & Storytelling**


## 🧠 Skills Demonstrated

- ✔ Data Cleaning & Transformation (Power Query)
- ✔ Data Modeling & Relationship Design
- ✔ DAX Measure Creation (KPIs, Calculations, Contribution %)
- ✔ Exploratory Data Analysis (EDA)
- ✔ Power BI Dashboard Design & Layout Structuring
- ✔ Advanced Data Visualization Techniques
- ✔ Business Insight Extraction & Storytelling
- ✔ KPI Tracking & Performance Analysis
- ✔ Problem-Solving using Sales & Operations Data
- ✔ End-to-End BI Project Development


##📥 How to Use This Project

1️⃣ Clone or download the repository
git clone: https://github.com/Likithasriram/Blinkit-Sales-Analysis.git

2️⃣ Open the .pbix file in Power BI Desktop

Make sure Power BI is updated.

3️⃣ Explore dashboard with slicers

Filter by outlet size, item type, fat content, etc.

## 📁 Project Files



Blinkit-Sales-Analysis/
│
├── Blinkit_Dashboard.pbix
├── Blinkit_Project_Report.pdf
├── README.md
└── assets/
      ├──  Blinkit screenshot.png
      ├──  KPI.png
      ├──  fat_content.png
      ├──  item_type.png
      ├──  fat_by_outlet.png
      └──  outlet_establishment.png



##👤 Author

Likhitha P
Data Analyst | Power BI | SQL | Excel | Python

📩 Email: likithasriramp@gmail.com
🔗 LinkedIn: www.linkedin.com/in/likitha-sriram1220
