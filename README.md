# Customer Behaviour Analysis 🛍️

## 📌 Project Overview
This project analyzes a customer shopping dataset to uncover patterns in consumer behavior, purchasing trends, and platform engagement. The goal is to derive actionable business insights that can help optimize inventory, marketing strategies, and customer retention programs.

The analysis follows a full data pipeline: **Data Cleaning → Exploratory Data Analysis (EDA) → Feature Engineering → Statistical Correlation → Database Integration (MySQL)  →  Visulization(Power Bi)**

## ❓ Business Problem
The retail business faces challenges in understanding its diverse customer base. Key questions addressed in this analysis include:
1.  **Customer Value:** Do subscription models actually drive higher spending or loyalty?
2.  **Demographic Targeting:** Which age groups and genders generate the most revenue?
3.  **Inventory Planning:** How does demand for specific categories (e.g., Clothing vs. Footwear) shift across seasons?
4.  **Rating Drivers:** Is there a relationship between shipping speed, spending levels, and customer satisfaction ratings?

## 🚀 Analysis Steps


1. **Data Cleaning and Preparation (Python)**
   - Loaded the dataset using Pandas.
   - Performed Exploratory Data Analysis (df.info(), df.describe())-
   - Handled missing values in Review Rating by imputing the mean rating for the respective product categories.
   - Feature Engineering: Created age_group bins and calculated the purchase_frequency_days.
   - Standardized columns and ensured data consistency before loading into MySQL.
   
2. **Structured Analysis (MySQL)**
   *The cleaned data was loaded into a MySQL database to simulate a transactional environment. Key SQL queries were executed to derive specific business insights,
   including:*
   - Revenue comparison by Gender.
   - Identification of Discount-Dependent Products.
   - Customer segmentation into New, Returning, and Loyal groups.
   - Analysis of subscription impact on average spending and repeat purchases.
   
3. **Reporting and Visualization (Power BI)**
   - Developed an interactive Customer Behaviour Analytics Dashboard to visualize core metrics.
   - Key visualizations include: Total Revenue, Sales by Gender and Category, Percentage of Customers by Subscription Status, and Revenue by Age Group.

## 📊 Key Insights & Findings
* **Loyalty Program Gap:** Surprisingly, **Subscribers and Non-Subscribers have nearly identical average spending** (~$59-60). The current subscription model does not significantly increase basket size.
* **Demographics:** Spending is evenly distributed across age groups. There is **no strong linear correlation** between a customer's age and their purchase amount or frequency.
* **Seasonal Trends:** **Spring** is the peak season for sales. While "Clothing" sells well year-round, "Footwear" sees a slight dip in the Fall.
* **Shipping & Satisfaction:** Customers using **Standard Shipping** gave higher average ratings (3.82) compared to **Store Pickup** (3.71), suggesting potential issues with the pickup experience.
* **Spending Behavior:** High-value transactions (> $70) differ slightly in satisfaction, with "High Spenders" giving better ratings on average than "Medium Spenders."

## 🛠️ Tools and Technologies
1. Data Processing:
   - Python, Pandas
2. Database:
   - MySQL
3. Visualization:
   - Power BI

## 📂 Dataset Description
The dataset consists of **3,900 records** with **19 columns**, including:
* **Customer Details:** `Customer ID`, `Age`, `Gender`, `Location`, `Subscription Status`
* **Transaction Details:** `Purchase Amount`, `Payment Method`, `Discount Applied`, `Frequency of Purchases`
* **Product Info:** `Item Purchased`, `Category`, `Size`, `Color`, `Season`
* **Feedback:** `Review Rating`, `Shipping Type`






