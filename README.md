🛒 Customer Shopping Behavior Analysis
📌 Project Overview

This project focuses on analyzing customer purchasing behavior using SQL and Power BI to uncover actionable business insights. It explores patterns in customer demographics, purchasing habits, subscription behavior, and discount usage to support data-driven decision-making.

The analysis answers key business questions such as:

Do subscribed customers spend more?
Which products receive the highest ratings?
How do discounts impact purchasing behavior?
What are the top-performing product categories?
🎯 Objectives
Analyze customer purchase patterns and revenue trends
Identify high-value customers and segments
Evaluate the impact of discounts and subscriptions
Provide insights for marketing and sales optimization
🧰 Tech Stack
SQL – Data querying and analysis
Power BI – Dashboard creation & visualization
Python (Jupyter Notebook) – Data preprocessing (if used)
Excel / CSV Dataset – Data source
📂 Project Structure
📁 Customer-Shopping-Behavior-Analysis
│
├── 📄 customer_behavior.sql        # SQL queries for analysis
├── 📊 customer_behaviour.pbix      # Power BI dashboard
├── 📓 Customer_Shopping_Behaviour_Analysis.ipynb  # Data analysis notebook
├── 📄 README.md                   # Project documentation
🔍 Key Analysis Performed
📊 1. Revenue Analysis
Revenue comparison by gender
Total revenue and average spending patterns
select gender, SUM(purchase_amount) as revenue
from customer
group by gender;

📎 Source:

💸 2. Discount Impact Analysis
Identified customers who used discounts but spent above average
Calculated discount usage percentage across products
⭐ 3. Product Performance
Top 5 products with highest average ratings
Most purchased items by category
🚚 4. Shipping Insights
Comparison of purchase behavior between Standard vs Express shipping
👥 5. Customer Segmentation

Customers are segmented into:

New Customers
Returning Customers
Loyal Customers
CASE
   WHEN previous_purchases = 1 THEN 'New'
   WHEN previous_purchases BETWEEN 2 AND 10 THEN 'Returning'
   ELSE 'Loyal'
END

📎 Source:

📈 6. Subscription Analysis
Compared:
Average spending
Total revenue
Customer count
Checked if repeat buyers are more likely to subscribe
🏆 7. Category-wise Insights
Top 3 products per category using window functions
Revenue contribution by age group
📊 Power BI Dashboard Features

The dashboard includes:

📌 Revenue KPI
📉 Funnel Chart (View → Cart → Purchase)
📊 Category-wise Revenue (Bar Chart)
📈 Sales Trend (Line Chart)
👥 Top Customers Table
💸 Discount Impact Visualization

<img width="1465" height="875" alt="image" src="https://github.com/user-attachments/assets/af630568-30b0-4f43-8e28-34e13483fc36" />

💡 Key Insights
Subscribed customers tend to generate higher total revenue
Discounts significantly influence purchasing behavior
Loyal customers contribute a major portion of revenue
Certain categories dominate sales volume and engagement
🚀 How to Run the Project
1️⃣ SQL Analysis
Import dataset into MySQL / PostgreSQL
Run queries from customer_behavior.sql
2️⃣ Power BI Dashboard
Open .pbix file in Power BI Desktop
Refresh dataset if needed
3️⃣ Notebook (Optional)
Run .ipynb file in Jupyter Notebook
📌 Future Improvements
Add predictive modeling (customer churn, recommendation system)
Deploy dashboard online (Power BI Service)
Integrate real-time data pipeline
👩‍💻 Author

Arunima Upreti

Aspiring Data Scientist | AI Trainer
Skilled in Data Analysis, Machine Learning & Visualization                                                                                                                              


