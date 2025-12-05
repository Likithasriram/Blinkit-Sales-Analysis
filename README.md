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

## 📐 Data Modeling (DAX Measures)

```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Item_Outlet_Sales])

Avg Sales = AVERAGE('BlinkIT Grocery Data'[Item_Outlet_Sales])

No of Items Sold = SUM('BlinkIT Grocery Data'[Quantity])

Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])

Contribution % = 
DIVIDE([Total Sales], CALCULATE([Total Sales], ALL('BlinkIT Grocery Data')))

Rating Weighted Sales =
SUMX('BlinkIT Grocery Data', 'BlinkIT Grocery Data'[Item_Outlet_Sales] * 'BlinkIT Grocery Data'[Rating])
---

**📊 Dashboard Overview**

🟨 Full Dashboard Screenshot
<img src="assets/A Blinkit screenshot.png" width="900"/>
**🔍 Close-Up Insights**

**⭐ 1. KPI Insights**

<img src="assets/KPI.png" width="500"/>

**Insights**

Total Sales: $1.20M+
Average Sales per item: $141

Total Items Sold: 8,500+

Average Rating: 3.92

**⭐ 2. Item Type Insights**

<img src="assets/item_type.png" width="500"/>

**Insights**

Fruits & Vegetables and Snacks dominate revenue

Household, Frozen Foods also perform strongly

Seafood, Breakfast, Hard Drinks underperform

**⭐ 3. Fat Content Insights**

<img src="assets/fat_content.png" width="450"/>

**Insights**

Low Fat items contribute the majority of total revenue

Strong customer preference for Low Fat categories

**⭐ 4. Fat by Outlet Tier**

<img src="assets/fat_by_outlet.png" width="500"/>

**Insights**

Tier 3 outlets outperform Tier 1 and Tier 2

Both Low Fat & Regular products sell highest in Tier 3

**⭐ 5. Sales Trend Over Time**

<img src="assets/outlet_establishment.png" width="500"/>

**Insights**

Sales show consistent growth over years

Major peaks in 2017 and 2020

**💡 Key Insights (Summary)**

**🔸 Sales Trends**

Clear growth trend with peaks in 2017 & 2020.

**🔸 Product Insights**

Low Fat items dominate sales.

Top categories: Fruits & Vegetables, Snacks, Household.

Least performing: Seafood, Hard Drinks, Breakfast.

**🔸 Outlet Insights**

Tier 3 outlets deliver the highest sales.

Medium-sized outlets outperform other sizes.

**🔸 Customer Behavior**

Overall customer ratings are strong at 3.92.

**🧭 Recommendations**

✔ 1. Expand in Tier 3 Locations

Strongest revenue potential.

✔ 2. Prioritize Medium-Sized Outlets

Highest sales performance → suitable for expansion.

✔ 3. Promote Low Fat Products

High demand → highlight in app + discount bundles.

✔ 4. Boost Performance of Low-Selling Categories

Use offers, rebranding, repositioning.

✔ 5. Improve Customer Experience

Better service in lower-rated outlets can improve retention.

**🛠 Tools & Technologies**

Power BI Desktop

Power Query

DAX

Excel

Data Modeling

Data Visualization

**📥 How to Use This Project**

1️⃣ Clone or download the repository
git clone https://github.com/yourusername/Blinkit-Sales-Analysis.git

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



**👤 Author**

Likhitha P
Data Analyst | Power BI | SQL | Excel | Python

📩 Email: likithasriramp@gmail.com
🔗 LinkedIn: www.linkedin.com/in/likitha-sriram1220
