# Sales Data Cleaning and Forecasting Analysis

### Overview
This project demonstrates a full data analysis workflow — from **cleaning** to **forecasting future sales** — using Python and the *Superstore Sales Dataset* (Kaggle).  
It combines data cleaning, exploratory analysis, and a SARIMAX time series model to predict future sales trends.

---

### Project Objectives
1. Detect and remove duplicate and inconsistent records.  
2. Standardize date and text formats for clean, structured data.  
3. Handle missing values and basic outlier adjustment.  
4. Visualize key performance metrics and regional sales trends.  
5. Build a simple yet effective **SARIMAX forecasting model** for future sales.  
6. Document and reproduce the workflow end-to-end.

---

### Folder Structure
sales-data-cleaning/
│
├── data/ → raw and cleaned datasets
├── notebooks/ → Jupyter notebooks
│ ├── 01_Superstore_Data_Cleaning_and_Trend_Analysis.ipynb
│ └── 02_Sales_Forecasting.ipynb
├── results/ → charts, forecasts, summary reports
├── src/ → reproducible scripts
├── requirements.txt
└── README.md


---

### Tools & Libraries
- Python 3  
- pandas, numpy  
- matplotlib  
- statsmodels (SARIMAX)  
- scikit-learn  
- JupyterLab  

---

### Key Results

#### Data Cleaning
- Removed duplicates and standardized date formats for **9,994 records**.  
- Clean dataset saved as UTF-8 (`data/clean_superstore.csv`).  
- Charts generated:  
  - `sales_by_region.png`  
  - `monthly_sales_trend.png`

#### Forecasting
- Built a **SARIMAX (p,d,q)** model for monthly sales.  
- Achieved low forecast error (MAE < 10% of mean sales).  
- Predicted the next **6 months** of sales with confidence intervals.  
- Files generated:  
  - `sales_forecast_next6months.csv`  
  - `forecast_summary.txt`  
  - forecast chart (`results/` folder)

---

### How to Run
1. Clone the repository  
  
   git clone https://github.com/<tu-usuario>/sales-data-cleaning.git
   cd sales-data-cleaning

Create a virtual environment

python -m venv .venv
.\.venv\Scripts\Activate.ps1   # (Windows PowerShell)
pip install -r requirements.txt

Run the cleaning script

python .\src\clean_and_analyze.py
Open JupyterLab and explore the notebooks


jupyter lab
01_Superstore_Data_Cleaning_and_Trend_Analysis.ipynb

02_Sales_Forecasting.ipynb

Example Insights
Top Region: West — highest total sales.

Top Category: Technology — strongest revenue driver.

Peak Month: November — clear seasonal pattern.

Forecast: Positive growth trend expected over the next 6 months.



Author



Claudia Liehr

Big Data \& Business Analyst

insightiqx@gmail.com

🌐 github.com/insightiqx

