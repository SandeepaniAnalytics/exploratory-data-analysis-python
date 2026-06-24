# 📊 E-Commerce Exploratory Data Analysis (EDA)

### Exploratory Data Analysis Project | Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-blue?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-teal?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

---

## 📄 Project Overview

An **Exploratory Data Analysis (EDA)** of a cleaned e-commerce orders dataset of **1,200 transactions** across **14 fields**, conducted in Python (pandas, numpy,  matplotlib, seaborn). 

---

## 🎯 Purpose of the Project

The purpose of this EDA is to turn a clean but static dataset into meaningful insight:

- 📐 Calculate descriptive statistics (mean, median, skewness) for all numeric fields
- 📈 Identify trends over time and across categories
- 🔍 Detect outliers and understand what's driving them
- 🔗 Examine relationships between order attributes and order outcomes
- 🧾 Answer a specific business question: what's behind the cancellation rate?

---

## 🛠️ Analysis Process

-  **Data Overview** - Loaded 1,200 rows × 14 columns, checked dtypes and missing values → **0 duplicate OrderIDs**, **0 duplicate TrackingNumbers**, **11 returning customers**
-  **Data Quality Checks** - Verified `TotalPrice = Quantity × UnitPrice` for every row, checked `Quantity` never exceeds `ItemsInCart`, confirmed no non-positive values → all checks passed
-  **Univariate Analysis** - Distribution, skewness, and IQR-based outlier counts for `Quantity`, `UnitPrice`, `ItemsInCart`, `TotalPrice`; value counts and bar charts for all categorical fields
-  **Time-Based Analysis** - Monthly orders, revenue, and average order value trends; day-of-week order patterns
-  **Relationships Between Variables** - Order value by Product and ReferralSource; OrderStatus breakdown by PaymentMethod and Product; order value by CouponCode
-  **Correlation Analysis** - Heatmap of numeric variable relationships
-  **Customer-Level Summary** - Orders, total spend, and average order value per customer; spend distribution
-  **Executive Summary** - Problem statement, methodology, key findings, and recommendations on the cancellation question

---

## 📊 Key Results

- ✅ **1,200** orders analyzed, **0** structural data issues found
- ✅ **1,189** unique customers; **11** are returning customers (~0.9%)
- ✅ **25.8%** of orders had no coupon applied (CouponCode = "No Coupon")
- ⚠️ **20.8%** overall order cancellation rate
- 🔎 Cancellation rate does not vary meaningfully by payment method, product, referral source, or coupon usage — **no single factor in this dataset explains the cancellation rate**

---

## 🧰 Tools Used

- **Python** (pandas, numpy)
- **Matplotlib** & **Seaborn** for visualization
- **Jupyter Notebook**

---

**Prepared by:** Sandeepani Rathnayake
