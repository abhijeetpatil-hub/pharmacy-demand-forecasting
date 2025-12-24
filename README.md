📊 Pharmacy Demand Forecasting & Inventory Intelligence System
📌 Business Problem

Pharmacies often face stock-outs of fast-moving medicines and overstocking of slow-moving or expiry-sensitive items.
Both situations lead to revenue loss, expiry losses, and poor patient service.

This project aims to forecast medicine demand using historical sales data to support data-driven inventory and reorder decisions in a retail pharmacy setup.

🎯 Project Objective

Analyze historical pharmacy sales data

Forecast future medicine demand

Support reorder-level planning

Reduce stock-outs and expiry risk

Provide insights through a Power BI dashboard

🗂 Dataset Overview

Source: Simulated / pharmacy-style transactional sales data

Time Period: Multi-month historical data

Key Columns:

Date

Medicine Name

Category

Quantity Sold

Sales Value

The dataset represents realistic pharmacy sales patterns suitable for operational decision-making.

🛠 Tools & Technologies Used

Excel – Initial data inspection

Python

Pandas (data cleaning & transformation)

Matplotlib / Seaborn (EDA & visualization)

Scikit-learn (forecasting model)

Power BI – Interactive dashboard & KPI visualization

🔄 Methodology (End-to-End Flow)
1️⃣ Data Cleaning & Preparation

Removed missing and inconsistent values

Converted date columns into proper datetime format

Aggregated daily sales into monthly demand

Created derived features such as:

Monthly sales trend

Medicine-level demand

2️⃣ Exploratory Data Analysis (EDA)

Identified top-selling medicines

Analyzed seasonal demand patterns

Compared category-wise sales contribution

Observed demand volatility across months

3️⃣ Demand Forecasting

Built a forecasting model using historical sales data

Predicted future medicine demand

Generated forecasts to assist inventory planning

4️⃣ Model Evaluation

T### 📐 Forecast Evaluation

The forecasting model was evaluated using standard regression metrics:

- **MAE:** 48.89 units  
- **RMSE:** 56.28 units  
- **MAPE:** 115.98%

📌 **Interpretation:**  
While MAPE appears high due to low-volume medicine sales (which inflate percentage errors), absolute metrics such as MAE and RMSE provide a more realistic measure of forecast accuracy for inventory planning.

The model serves as a **baseline forecasting approach**, suitable for identifying demand trends and supporting reorder-level decisions.


5️⃣ Visualization & Dashboarding

Created a Power BI dashboard with:

Total Sales KPI

Monthly Demand Trend

Top Medicines by Demand

Category-wise Contribution

Forecast vs Actual comparison

📈 Key Insights

A small group of medicines contributes to a large share of total demand

Certain categories show clear seasonal demand patterns

Forecasting enables proactive reorder planning instead of reactive purchasing

Demand prediction can significantly reduce stock-out risk for fast-moving medicines

💡 Business Impact

This system can help a real pharmacy to:

Improve medicine availability

Optimize reorder cycles

Reduce expired stock losses

Support data-driven inventory decisions

Increase customer satisfaction and revenue stability

📊 Dashboard Preview

<img width="1920" height="1080" alt="DASHBOARD (2)" src="https://github.com/user-attachments/assets/23317c88-afdf-4a4a-9228-346750e02352" />
The Actual vs Predicted demand plot helps visually assess forecast bias and variability, confirming areas where the model underestimates or overestimates demand.


visuals/pharmacy_demand_dashboard.png


(Uploading a Power BI dashboard image here will greatly improve recruiter engagement.)

📁 Project Structure
pharmacy-demand-forecasting/
│
├── data/
│   ├── raw_sales_data.csv
│   └── cleaned_sales_data.csv
│
├── notebooks/
│   └── demand_forecasting_analysis.ipynb
│
├── models/
│   └── forecasting_model.pkl
│
├── powerbi/
│   └── pharmacy_demand_dashboard.pbix
│
├── visuals/
│   └── dashboard_preview.png
│
└── README.md

🚀 Future Enhancements

Implement advanced time-series models (ARIMA / Prophet)

Add automatic reorder-level recommendations

Integrate expiry-based inventory risk

Deploy dashboard for real-time access
“Future work includes time-series models (ARIMA/Prophet) and SKU-level forecasting.”
🧠 Why This Project Matters

This project demonstrates the ability to:

Combine domain knowledge (pharmacy) with analytics

Solve a real operational business problem

Work across the full data lifecycle

Translate data into actionable decisions

👤 Author

Abhijeet Patil
Data Analytics | Data Science | Healthcare & Pharmacy Domain
