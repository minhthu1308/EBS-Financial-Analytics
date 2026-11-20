# Amazon Books Budget & Financial Planning Analytics

**A Python-based Financial Analytics Project**

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow)

## 1. Project Overview

Amazon Books Budget & Financial Planning Analytics is a financial analytics project developed using Python.

The project focuses on budget planning, financial performance monitoring, budget variance analysis, and basic financial forecasting.

It uses two independent real-world datasets:

- **Dataset A – Amazon Books Sales / Market Data:** Provides book market information for exploring pricing, sales-related characteristics, and business context.
- **Dataset B – Budget & Actual Financial Data:** Supports budget planning, actual financial performance monitoring, and financial analysis.

The project aims to transform raw financial data into meaningful insights through data processing, financial calculations, and an interactive Streamlit dashboard.

## 2. Problem Statement

Businesses need to monitor financial performance and manage budgets effectively.

However, comparing planned budgets with actual financial results can be challenging when financial information is stored across different datasets.

This project addresses several problems:

- Difficulty monitoring budget allocation and actual spending.
- Limited visibility into budget variances.
- Difficulty identifying categories with excessive spending.
- Challenges in understanding revenue and expense trends.
- Limited use of historical data for future budget planning.

## 3. Project Objectives

- Analyze and process real-world datasets using Python.
- Develop a structured budget planning workflow.
- Compare budgeted and actual financial performance.
- Calculate financial variances and relevant KPIs.
- Analyze revenue and expense trends.
- Implement basic financial forecasting.
- Build an interactive dashboard for financial monitoring and decision support.

## 4. Key Features

### Budget Planning
- Organize budgets by financial category and period.
- Analyze monthly and quarterly budget allocation.
- Calculate budget distribution percentages.
- Explore different budget scenarios.

### Budget vs Actual Analysis
- Compare budgeted and actual revenue.
- Compare budgeted and actual expenses.
- Calculate absolute and percentage variances.
- Identify over-budget and under-budget categories.

### Financial Performance Analysis
- Analyze revenue and expense trends.
- Calculate profit and profit margin when supporting data is available.
- Identify major expense categories.
- Compare financial performance across periods.

### Financial Forecasting
- Analyze historical financial trends.
- Forecast revenue and expenses when sufficient data is available.
- Develop best-case, base-case, and worst-case scenarios.
- Document forecasting assumptions and limitations.

### Interactive Dashboard
- Financial KPI monitoring.
- Budget allocation visualization.
- Budget vs actual comparison.
- Financial performance charts.
- Forecasting visualization.

## 5. Dataset

The project uses two independent analytical datasets.

| Dataset | Purpose |
|---|---|
| Amazon Books Sales / Market Data | Book market and business context analysis |
| Budget & Actual Financial Data | Budget planning and financial performance analysis |

**Data principles:**

- Use real-world data sources.
- Document dataset sources and data collection methods.
- Validate data quality before analysis.
- Preserve original raw datasets.
- Keep the two datasets independent unless a valid common key and compatible definitions exist.
- Do not treat book prices as actual revenue.
- Do not assume revenue represents profit.

Detailed dataset information will be documented in the `docs/` directory.

## 6. Financial KPIs

The project will implement relevant financial metrics, including:

| KPI | Description |
|---|---|
| Total Budgeted Revenue | Planned revenue |
| Actual Revenue | Recorded revenue |
| Total Budgeted Expenses | Planned expenses |
| Actual Expenses | Recorded expenses |
| Absolute Variance | Difference between actual and budgeted values |
| Variance Percentage | Relative difference between actual and budgeted values |
| Actual Profit | Revenue minus expenses, when valid data is available |
| Profit Margin | Profit as a percentage of revenue, when applicable |
| Budget Allocation | Percentage of budget assigned to each category |

All calculations will be documented and validated.

## 7. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical calculations |
| Matplotlib / Seaborn | Data visualization |
| Plotly | Interactive visualization |
| Streamlit | Dashboard development |
| Jupyter Notebook | Data exploration and experimentation |
| VS Code | Development environment |
| Git / GitHub | Version control |

## 8. Project Structure

```text
amazon-books-budget-analytics/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_budget_planning.ipynb
│   ├── 04_variance_analysis.ipynb
│   └── 05_financial_forecasting.ipynb
│
├── src/
│   ├── data_processing/
│   ├── financial_analysis/
│   └── utils/
│
├── dashboard/
│   ├── app.py
│   └── pages/
│
├── docs/
│   ├── PRD.md
│   └── data_dictionary.md
│
├── requirements.txt
├── README.md
└── .gitignore
```

## 9. Installation & Setup

### Step 1: Clone the repository

```bash
git clone <repository-url>
```

### Step 2: Navigate to the project directory

```bash
cd amazon-books-budget-analytics
```

### Step 3: Create a virtual environment

```bash
python -m venv venv
```

### Step 4: Activate the environment

Windows:

```bash
venv\Scripts\activate
```

### Step 5: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 6: Run the dashboard

```bash
streamlit run dashboard/app.py
```

*Note: The application will be runnable after the corresponding development components have been implemented.*

## 10. Expected Dashboard

The dashboard is planned to contain five main pages:

1. **Financial Overview** – Key financial KPIs and overall budget performance.
2. **Budget Planning** – Budget allocation and planning scenarios.
3. **Budget vs Actual** – Financial variance analysis.
4. **Financial Performance** – Revenue, expenses, profit, and financial trends.
5. **Financial Forecasting** – Historical trends and future financial projections.

## 11. Project Roadmap

- [ ] Phase 1: Dataset Research & Validation
- [ ] Phase 2: Data Understanding & Exploration
- [ ] Phase 3: Data Cleaning & Preprocessing
- [ ] Phase 4: Budget Planning Analysis
- [ ] Phase 5: Budget vs Actual Analysis
- [ ] Phase 6: Financial Performance Analysis
- [ ] Phase 7: Financial Forecasting
- [ ] Phase 8: Interactive Dashboard Development
- [ ] Phase 9: Testing, Documentation & Finalization

## 12. Project Documentation

- Product Requirements Document (PRD)
- Dataset Documentation
- Data Dictionary
- Financial KPI Definitions
- Analysis Results and Business Insights

---

**Project Status:** In Development

**Primary Focus:** Budget & Financial Planning Analytics

**Project Level:** Intermediate
