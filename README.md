# Retail Sales Analytics & Revenue Forecasting Dashboard

A comprehensive data analytics project combining business intelligence dashboards with machine learning forecasting to analyze retail sales performance and predict future trends.

## Project Overview

This project demonstrates end-to-end data analytics capabilities, from exploratory data analysis to interactive dashboard creation and predictive modeling. Using 4 years of retail sales data (2014-2017), I built executive dashboards in Tableau and developed a Prophet-based forecasting model to predict 2018 sales performance.

**Live Dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/amrita.thapa/viz/RetailSalesPerformanceDashboard_17696505192980/Story1)

---

## Key Insights & Findings

### Business Performance
- **Total Sales (2014-2017):** $2.3M
- **Total Profit:** $286K
- **Overall Profit Margin:** 12.5%
- **Total Orders:** 5,009

### Critical Business Insights
1. **Technology dominates profitability** - Highest profit ($145K) with 37% margin on products like Copiers
2. **Furniture category underperforming** - Despite $742K in sales, only $18K profit (2.5% margin)
3. **Tables are unprofitable** - Losing $17.7K annually, the worst-performing sub-category
4. **Discount strategy issues** - Discounts over 30% result in negative profit margins
5. **West region outperforms** - 14.9% profit margin vs 7.9% in Central region
6. **Strong seasonality** - November-December peak accounts for significant annual revenue
7. **Year-over-year growth** - 89% profit increase from 2014 to 2017

### 2018 Forecast Results
- **Predicted Total Sales:** $869K
- **Peak Months:** November ($126K) and December ($113K)
- **Model Performance:** MAE of $2,287 on test set

---

## Technologies & Tools

**Data Analysis & Modeling:**
- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Prophet (Facebook's time series forecasting library)
- Scikit-learn (model evaluation)

**Business Intelligence:**
- Tableau Public 2025.3
- Interactive dashboards with drill-down capabilities

**Development Environment:**
- Jupyter Notebooks
- VS Code
- Virtual Environment (uv)
- Git version control

---

## Project Structure

```
Retail_Sales_forecasting/
├── data/
│   └── superstore.csv                    # Raw sales data
├── notebooks/
│   ├── 01_exploratory_analysis.ipynb     # EDA and insights
│   └── 02_sales_forecasting.ipynb        # Prophet forecasting model
├── outputs/
│   ├── figures/
│   │   └── monthly_sales_forecast.png    # Forecast visualization
│   └── processed_data/
│       ├── superstore_processed.csv      # Cleaned data
│       ├── monthly_forecast_2018.csv     # Forecast results
│       └── forecast_summary.csv          # Model metrics
└── README.md
```

---

## Dashboard Features

### Dashboard 1: Executive Summary
- **KPI Cards:** Total Sales, Profit, Margin, Orders at-a-glance
- **Sales Trend Analysis:** Monthly performance with trend line (2014-2017)
- **Category Performance:** Sales and profit comparison across product categories
- **Geographic Analysis:** Interactive US map showing state-level performance
- **Product Analysis:** Profitability by sub-category with winners and losers highlighted

### Dashboard 2: Sales Forecast 2018
- **Historical Context:** Full 2014-2017 performance baseline
- **12-Month Projection:** Prophet-based forecast with confidence intervals
- **Seasonal Patterns:** Captured Q4 peaks and seasonal trends
- **Interactive Visualization:** Dual-axis chart separating historical vs forecast data

---

## Analytical Approach

### 1. Exploratory Data Analysis
- Analyzed 9,994 transactions across 4 years
- Identified trends, seasonality, and anomalies
- Examined performance across categories, regions, segments, and time periods
- Investigated discount impact on profitability

### 2. Business Insights Development
- Calculated key metrics: profit margins, YoY growth, customer segments
- Identified underperforming products and categories
- Analyzed regional and seasonal patterns
- Developed actionable business recommendations

### 3. Forecasting Model
- **Model:** Facebook Prophet with multiplicative seasonality
- **Features:** Yearly and weekly seasonality patterns
- **Validation:** 3-month holdout test set (Oct-Dec 2017)
- **Performance:** 12% error on total sales prediction
- **Output:** Daily and monthly forecasts with confidence intervals

### 4. Dashboard Design
- Created clear visual hierarchy with KPIs at top
- Used color coding for quick insights (green for profit, red for loss)
- Implemented interactive filtering for drill-down analysis
- Designed for executive decision-making

---

## Business Recommendations

Based on the analysis, key recommendations include:

1. **Implement discount caps** - Limit discounts to maximum 20% to maintain profitability
2. **Review furniture strategy** - Investigate Tables category pricing and costs
3. **Focus on high-margin products** - Expand Copiers, Paper, and Accessories offerings
4. **Expand West region presence** - Leverage highest-performing region
5. **Optimize Q4 operations** - Prepare for seasonal peaks in November-December
6. **Target Home Office segment** - Best profit margin (14%) despite smallest volume

---

## Key Skills Demonstrated

- **Data Analysis:** EDA, statistical analysis, trend identification
- **Data Visualization:** Tableau dashboard design, storytelling with data
- **Machine Learning:** Time series forecasting, model evaluation
- **Business Intelligence:** KPI development, executive reporting
- **Python Programming:** Data manipulation, modeling, visualization
- **Communication:** Translating technical analysis into business insights

---

## Sample Visualizations

### Monthly Sales Trend
Shows 4-year historical performance with clear seasonality and growth trend.

### Profit by Sub-Category
Identifies top performers (Copiers: $55K) and problem areas (Tables: -$17K).

### Sales Forecast 2018
Prophet model projection showing continued growth with seasonal patterns.

---

## How to Run This Project

### Prerequisites
```bash
python 3.10+
uv (or pip)
```

### Setup
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/Retail_Sales_forecasting.git
cd Retail_Sales_forecasting

# Create virtual environment
uv venv

# Activate virtual environment
# Windows:
.venv\Scripts\activate
# Mac/Linux:
source .venv/bin/activate

# Install dependencies
uv pip install pandas numpy matplotlib seaborn jupyter prophet scikit-learn openpyxl
```

### Run Analysis
```bash
# Open Jupyter notebooks
jupyter notebook

# Navigate to notebooks/ folder and run:
# 1. 01_exploratory_analysis.ipynb
# 2. 02_sales_forecasting.ipynb
```

### View Dashboard
- Download Tableau Public Desktop
- Open the published workbook from [Tableau Public link]
- Or open the .twbx file if included in the repository

---

## Contact

**Amrita Thapa**
- Email: AmritaThapa2626@gmail.com
---

## Acknowledgments

- Dataset: Sample Superstore dataset (Kaggle/Tableau)
- Forecasting: Facebook Prophet library
- Tools: Tableau Public, Python, Jupyter

---

## License

This project is open source and available for educational and portfolio purposes.

---


*This project was created to demonstrate data analytics, business intelligence, and machine learning forecasting capabilities for data analyst and data science roles.*