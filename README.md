# customer_behavior_analysis
This project leverages a retail company's consumer shopping data to identify key trends, optimize marketing strategies, and improve customer loyalty. It using Python,SQL and PowerBI


## 🛍️ Retail Customer Shopping Behavior Analysis

# 🌟 Overview
This project is an end-to-end data analysis initiative focused on uncovering key purchasing patterns, customer segments, and revenue drivers within a retail dataset. The goal is to provide actionable strategic recommendations to improve sales, customer engagement, and long-term loyalty.

The analysis answers the central business question:"How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?"

## 📊 Dataset

Source:Synthetic Retail Transactional Data
Size: 3,900 rows and 18 columns.
Key Features: Customer demographics (Age, Gender, Location, Subscription Status), purchase details (Category, Purchase Amount), and behavioral metrics (Review Rating, Discount Applied, Previous Purchases).

##🛠️ Tools and Technologies
1. Data Processing:
   Python, Pandas
2. Database:
   MySQL
3. Visualization:
   Power BI
4. Reporting:
   Gamma
   
## 🚀 Analysis Steps

This project followed a standard, robust data analysis workflow:

1.**Data Cleaning and Preparation (Python)**
   Loaded the dataset using Pandas.
   Performed Exploratory Data Analysis (df.info(), df.describe())
   .Handled missing values in Review Rating by imputing the median rating for the respective product categories.
   Feature Engineering: Created age_group bins and calculated the purchase_frequency_days.
   Standardized columns and ensured data consistency before loading into MySQL.
   
2. **Structured Analysis (MySQL)**
   The cleaned data was loaded into a MySQL database to simulate a transactional environment. Key SQL queries were executed to derive specific business insights,
   including:
   Revenue comparison by Gender.
   Identification of Discount-Dependent Products.
   Customer segmentation into New, Returning, and Loyal groups.
   Analysis of subscription impact on average spending and repeat purchases.
   
3. **Reporting and Visualization (Power BI)**
   Developed an interactive Customer Behaviour Analytics Dashboard to visualize core metrics.
   Key visualizations include: Total Revenue, Sales by Gender and Category, Percentage of Customers by Subscription Status, and Revenue by Age Group.

## ✨ Key Results and Recommendations

The analysis identified actionable levers for strategic improvement:

Finding------------------------------->Actionable Recommendation
1. High Revenue from Young Adults ($62K+)-------------------------->Target Young Adults with personalized, high-value campaigns and products.
2. 57% of Purchases Used Discount--------------------------------->Review the discount strategy. Introduce non-monetary incentives (e.g., early access, exclusive bundles) to protect profit margins.
3. Gender Revenue Disparity------------------------------->Investigate and potentially restructure marketing efforts to boost female customer engagement and spending.
4. Loyalty Program Opportunity---------------------------->Formalize a loyalty program to reward the existing 3,116 'Loyal' customers and incentivize 'Returning' customers to increase frequency.
  
  
## 💻 How to Run the Project

1. **Clone the Repository**
   ```bash
      git clone https://github.com/Mohitydv459/customer_behavior_analysis.git
      cd retail-customer-analysis
   ```
   
2. **Run Python Script**
   Ensure all required libraries (Pandas, SQL-connector) are installed (pip install -r requirements.txt).
   Execute the Python script to clean the data and load it into your local MySQL instance.
   
3. **Execute SQL Queries**
   Connect to your MySQL instance.
   Run the main script located at Scripts/SQL/customer_behaviour.sql to generate the core analytical results.
   
4. **View Dashboard**
   Open the primary dashboard file: Dashboard/customer_behaviour_visualization.pbix in Power BI Desktop.
   Refresh the data connection to point to your local MySQL instance.

