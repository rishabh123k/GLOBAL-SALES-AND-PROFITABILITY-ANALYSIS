# 📊 Power BI GLOBAL SALES AND PROFITABILITY ANALYSIS Dashboard

### 🚀 Project Overview
This project showcases an **interactive Power BI Dashboard** built using a dataset of 700+ sales records.  
The goal was to analyze **sales, profit, and discount performance** across multiple countries, products, and time periods — turning raw data into meaningful business insights.

---

## 🧠 Objectives
- Analyze total **Sales**, **Profit**, and **Units Sold** by Country, Product, and Discount Band  
- Track **monthly and yearly sales trends**  
- Evaluate the **impact of discounts** on profit margins  
- Provide **interactive filters and KPIs** for dynamic insights  

---

## 🛠️ Tools & Technologies
- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Microsoft Excel / CSV Data Source**
- **Data Modeling and Visualization**

---

## 💡 Insights Derived
- Identified top-performing countries and products
- Analyzed seasonal trends in sales performance
- Found correlation between discounts and profit margin
- Visualized profitability distribution with color-coded conditional formatting

--- 

## 🧮 DAX Measures Used

```DAX
Total Sales = SUM('SalesData'[Sales])

Total Profit = SUM('SalesData'[Profit])

Total Gross Sales = SUM('SalesData'[Gross Sales])

Total Units Sold = SUM('SalesData'[Units Sold])

Average Discount % = 
DIVIDE(
    SUM('SalesData'[Discounts]),
    SUM('SalesData'[Gross Sales])
) * 100

Profit Margin % = 
DIVIDE(
    SUM('SalesData'[Profit]),
    SUM('SalesData'[Sales])
) * 100

Average Sale Price = AVERAGE('SalesData'[Sale Price])



