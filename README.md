# 📊 Telco Customer Churn Analysis – Project Summary

📁 Dataset:
Telco-Customer-Churn

Contains details such as: customerID, gender, SeniorCitizen, tenure, Contract, PaymentMethod, TotalCharges, Churn, etc.

Total rows: 7043

⚙️ Tools Used:
| Tool         | Purpose                                       |
| ------------ | --------------------------------------------- |
| **Python**   | EDA, feature insights, initial visualizations |
| **SQLite**   | SQL-based metric calculations inside Python   |
| **Power BI** | KPI tracking, dashboards, slicers/filters     |


📌 Key KPIs (Calculated in Power BI / SQL):
| KPI                      | Value                                             |
| ------------------------ | ------------------------------------------------- |
| 🧑‍🤝‍🧑 Total Customers | 7043                                              |
| 📉 Churn Rate            | 27%                                               |
| 💸 Lost Revenue          | ₹2.86 Million                                     |
| ⏳ Average Tenure         | 32.37 months                                      |
| 📈 Avg. Monthly Charges  | ₹64.76                                            |


🔍 Power BI Insights:

🔹 Churn by Demographics

Senior Citizens churn less (41.68%) than younger users.

Females have more churn with Bank Transfer, while males churn more with Electronic/Mailed Checks.

🔹 Contract and Services Impact

Month-to-Month with Fibre Optic contract shows highest churn (2128 customers).

Tech Support absent → High churn in males.

StreamingTV & Movies impact churn moderately; no-internet users show least churn.

🔹 Payment Behavior

Electronic Check users churn more (₹1.56M in revenue).

Users with PhoneService + Electronic Check have 2139 churns.

🔹 Partner/Dependent Impact

With Partner + 1/2 year contract = more churn.

No partner + Month-to-Month = lesser churn.

🔹 Combined Insights

OnlineBackup + No OnlineSecurity = 3498 users → potential vulnerability.

Paperless Billing + StreamingMovies + No InternetService shows least churn (113 users).

🧮 SQL (Using SQLite in Python)

Queries executed:

Churn Rate calculation

Total Revenue lost due to churn

Churn by Senior Citizen

Churn distribution by Contract and PaymentMethod

All SQL operations performed using sqlite3 in Python.


📈 Python Visualizations

Using Seaborn/Matplotlib:

Boxplots (TotalCharges vs Churn)

Countplots (Churn vs Gender, Contract, PaymentMethod)

Correlation heatmap

Pie charts (Service usage & Churn impact)

Heatmaps for multivariate relations

📌 Dashboard Layout (Power BI)

KPIs at the Top:

Total Customers, Churn Rate, Revenue, Services per Customer

Visual Rows:
Churn by Gender, Senior Citizen, Contract

Charges & Tenure Distributions

Churn by Services (StreamingTV, Movies, Tech Support)

Slicers:

Gender, Contract, Services, Churn filter

✅ Conclusion:

This Telco Churn project provides actionable business insights to reduce churn, target at-risk customer groups, and improve customer retention strategies. Insights are validated using Python, SQL, and Power BI dashboards — making this project interview-ready and industry-relevant.
