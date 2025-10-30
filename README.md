# Sales Data Cleaning, Forecasting & Customer Segmentation

### Overview
This repository showcases a full analytics workflow on the **Superstore Sales Dataset (Kaggle)** — from data cleaning to predictive modeling and customer segmentation.  
It demonstrates how to extract, transform, visualize, and model business data using Python, following best practices for reproducibility and clarity.

---

### Project Objectives
1. Clean and structure raw sales data for analysis.  
2. Visualize key performance metrics and regional trends.  
3. Forecast future sales using **SARIMAX** time series modeling.  
4. Segment customers using **RFM analysis** and **K-Means clustering**.  
5. Communicate actionable insights with visuals and documentation.

---

### Folder Structure
sales-data-cleaning/
│
├── data/ → raw and cleaned datasets
├── notebooks/ → Jupyter notebooks
│ ├── 01_Superstore_Data_Cleaning_and_Trend_Analysis.ipynb
│ ├── 02_Sales_Forecasting.ipynb
│ └── 03_Customer_Segmentation.ipynb
├── results/ → charts, forecasts, segmentation summaries
├── src/ → reproducible scripts
├── requirements.txt
└── README.md


---

### Tools & Libraries
- Python 3  
- pandas, numpy  
- matplotlib, seaborn  
- statsmodels (SARIMAX)  
- scikit-learn (K-Means)  
- JupyterLab  

---

## **1. Data Cleaning & Trend Analysis**
- Removed duplicates and standardized date formats for 9,994 records.  
- Generated visuals:  
  - `sales_by_region.png`  
  - `monthly_sales_trend.png`  
- Clean dataset saved as `data/clean_superstore.csv`.

---

## **2. Sales Forecasting (SARIMAX)**
- Built and tuned a SARIMAX model to forecast monthly sales.  
- Achieved a low Mean Absolute Error (MAE < 10% of mean sales).  
- Predicted the next 6 months of sales and exported:  
  - `sales_forecast_next6months.csv`  
  - `forecast_summary.txt`

---

## **3. Customer Segmentation (RFM + K-Means)**
- Calculated **Recency**, **Frequency**, and **Monetary Value** for each customer.  
- Scaled the variables and applied **K-Means clustering (k=4)**.  
- Identified four customer segments based on purchasing behavior:
  - **Cluster 0:** High-value, frequent, recent buyers.  
  - **Cluster 1:** Inactive or one-time customers.  
  - **Cluster 2:** Moderate buyers with medium recency.  
  - **Cluster 3:** New or reactivated customers.  
- Visuals generated:
  - `segmentation_scatter.png`  
  - `monetary_by_cluster.png`  
- Results saved to:
  - `customer_segments.csv`  
  - `segmentation_summary.txt`

---

### How to Run
1. Clone the repository  
   
   git clone https://github.com/<tu-usuario>/sales-data-cleaning.git
   cd sales-data-cleaning

Create and activate a virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt

Run the main script
python .\src\clean_and_analyze.py

Open JupyterLab and explore the notebooks
jupyter lab

01 → Cleaning & Trend Analysis

02 → Sales Forecasting

03 → Customer Segmentation

Example Insights
Top Region: West — highest total sales.

Top Category: Technology — strongest revenue driver.

Peak Month: November — clear seasonal pattern.

High-Value Customers: Frequent and high-spending buyers concentrated in specific regions.

Forecast: Steady growth trend expected over the next 6 months.


Author



Claudia Liehr

Big Data \& Business Analyst

insightiqx@gmail.com

🌐 github.com/insightiqx

