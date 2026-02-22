# 📊 Customer Churn Analysis – Power BI Project

This project focuses on analyzing customer churn to identify key factors influencing customer retention and churn behavior. The dashboard provides actionable insights for business decision-making.

---

## 🎯 Objectives

- Identify churn patterns and high-risk customer segments  
- Analyze customer behavior and retention metrics  
- Support data-driven strategies to reduce churn  

---

## 🛠️ Tools & Technologies

- Power BI  
- Excel  
- DAX  
- Power Query  

---

## 📈 Key Features

- Interactive Power BI dashboard  
- KPIs: Churn Rate, Retention Rate, Customer Segmentation  
- Filters and slicers for dynamic analysis  
- Clean and user-friendly visual design  

---

## 💻 Key DAX Measures

```DAX
Total Customers = 
COUNT('Customers'[CustomerID])

Churned Customers = 
CALCULATE(
    COUNT('Customers'[CustomerID]),
    'Customers'[Churn] = "Yes"
)

Churn Rate = 
DIVIDE(
    [Churned Customers],
    [Total Customers]
)
Retention Rate = 
1 - [Churn Rate]
```
## 🔎 Customer Segmentation Logic
```DAX
 Customer Segment = 
IF(
    'Customers'[Balance] > 100000,
    "High Value",
    "Regular"
)
```
## 🔄 Data Cleaning (Power Query)
```M
= Table.TransformColumnTypes(Source,{
    {"CustomerID", Int64.Type},
    {"Age", Int64.Type},
    {"Balance", type number}
})
```
📌 Insights Gained

Identified key churn drivers

Highlighted customer segments with higher churn risk

Suggested data-driven strategies to improve retention
