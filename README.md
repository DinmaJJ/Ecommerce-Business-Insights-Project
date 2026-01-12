📊 E-commerce Business Insights & Analytics Project
📌 Project Description

This project is an end-to-end data analytics and business intelligence solution built using Python and SQL to analyze an e-commerce transactional dataset. It focuses on data cleaning, exploratory data analysis (EDA), feature engineering, analytical querying, visualization, and predictive modeling to extract actionable insights around customer behavior, revenue drivers, churn, and lifetime value (LTV).

🛠️ Tech Stack

- Programming: Python
- Data Analysis: Pandas, NumPy
- Data Visualization: Plotly
- Databases & Querying: SQL (SQLite)
- Modeling: Scikit-learn
- ETL & Data Cleaning: Custom Python pipelines
- EDA & Profiling: ydata-profiling

🔄 Data Pipeline & Methodology
1️⃣ Data Ingestion & Cleaning (ETL)

- Handled missing values, invalid records, and duplicates
- Normalized categorical fields (regions, payment methods, customer tiers)
- Engineered derived metrics such as:
    * Customer lifetime value (LTV)
    * Churn flags
    * Order frequency
    * Delivery delay metrics

2️⃣ Exploratory Data Analysis (EDA)

- Used ydata-profiling for automated dataset diagnostics
- Identified outliers in delivery time, revenue, and refunds
- Analyzed distributions of orders, customer spend, and ratings

3️⃣ SQL Analytics

- Wrote complex SQL queries to:
- Segment customers by spend and activity
- Analyze churn cohorts
- Identify top and bottom-performing products
- Validate Python-derived metrics

4️⃣ Visualization

- Interactive dashboards built with Plotly
- Visualized:
    * Revenue trends
    * Churn over time
    * Product performance
    * Regional profitability
    * Fulfillment delays vs customer ratings

📈 Key Analytical Findings
Customer Retention & Segmentation

- Churn is strongly correlated with:
    * Inactivity (>180 days)
    * High shipping costs
    * Lower credit tiers

- High LTV customers are predominantly:
    * Credit tiers A/B
    * Newsletter subscribers
      
- Revenue concentration observed among a small percentage of customers (Pareto effect).

Product Performance

- Identified high-margin, high-volume SKUs driving revenue
- Flagged loss-making products with negative revenue due to refunds or pricing errors
- Bottom-performing products identified using percentile ranking

Operations & Fulfillment

- Delivery delays have a strong negative impact on customer ratings
- On-time delivery rate (~65%) consistent across warehouses, indicating systemic inefficiencies
- Cash and PayPal show higher transaction failure rates compared to digital wallets

Financial Trends

- ~50% decline in sales and profits between 2024–2025
- USD dominates sales volume but yields lower margins compared to EUR and GBP
- Regional profitability varies significantly despite similar sales volumes

🤖 Predictive Modeling
Churn Prediction

- Model : Classification (Random Forect Classifier)

- Key predictors:
    * Customer inactivity
    * Shipping cost
    * Subscription status

- Performance:
    * Accuracy: 1.00

Customer Lifetime Value (LTV)
 
- Model : Regression (Random Forest Regressor)

- Strong predictors:
    * Purchase frequency
    * Average order value
    * Customer tenure

- Performance:
    * R² score: 0.99

📌 Business Recommendations

- Shift growth strategy from acquisition to retention and LTV optimization
- Introduce targeted loyalty programs for high-value customers
- Optimize logistics to reduce delivery delays
- Remove or reprice loss-making products
- Promote reliable digital payment methods
- Expand operations in high-margin regions and currencies

🚀 Future Improvements

- Enable real-time data ingestion for continuous analytics and model refresh.
- Automate reporting dashboards
- Introduce real-time churn monitoring
- Integrate recommendation systems
