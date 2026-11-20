# PRODUCT REQUIREMENTS DOCUMENT (PRD)

# Amazon Books Budget & Financial Planning Analytics

**Version:** 2.0  
**Project Level:** Intermediate  
**Primary Domain:** Financial Analytics  
**Main Focus:** Budget & Financial Planning  
**Technology:** Python, Pandas, NumPy, Matplotlib, Plotly, Streamlit

---

## 1. Document Information

| Item | Description |
|---|---|
| Project Name | Amazon Books Budget & Financial Planning Analytics |
| Project Type | Data Analytics / Financial Analytics |
| Project Level | Intermediate |
| Primary Users | Data Analysts, Financial Analysts, Business Owners |
| Programming Language | Python |
| Dashboard | Streamlit |
| Data Strategy | Two independent datasets |

## 2. Product Overview

The project aims to develop a financial analytics system that supports budget planning, financial performance monitoring, budget variance analysis, and basic financial forecasting.

The system uses Python to process and analyze book-market and financial planning data. An interactive Streamlit dashboard will present financial KPIs, budget comparisons, expense breakdowns, and forecast results.

The project focuses on financial planning and decision support rather than simply describing book market trends.

## 3. Problem Statement

Businesses need to monitor their financial performance and manage budgets effectively.

However, financial information may be stored across different datasets, making it difficult to compare planned budgets with actual financial results.

This project addresses the following problems:

- Difficulty monitoring budget allocation and actual spending.
- Lack of visibility into budget variances.
- Difficulty identifying categories with excessive spending.
- Limited ability to understand revenue and expense trends.
- Difficulty using historical information to support future budget planning.

The proposed system will provide a centralized analytical dashboard to support these activities.

## 4. Product Goals & Objectives

### Main Goals

1. Understand and analyze financial data using Python.
2. Build a structured budget planning and monitoring workflow.
3. Compare planned budgets with actual financial performance.
4. Identify financial variances and potential budget risks.
5. Perform basic financial forecasting.
6. Present financial insights through an interactive dashboard.

### Learning Objectives

- Develop practical Python data analytics skills.
- Understand budgeting and financial planning concepts.
- Apply financial formulas and KPIs.
- Learn data visualization and dashboard development.
- Build a portfolio project relevant to Data Analyst and Financial Analyst roles.

## 5. Target Users & User Stories

### Target Users

**1. Financial Analysts**

Need to monitor budgets, compare actual results, and analyze financial performance.

**2. Data Analysts**

Need to process financial datasets, calculate KPIs, and communicate insights.

**3. Business Owners / Managers**

Need to understand spending patterns and make better budget allocation decisions.

**4. Students and Learners**

Need practical experience with financial data analysis and Python.

### User Stories

- As a Financial Analyst, I want to compare actual expenses with planned budgets so that I can identify overspending.
- As a Business Owner, I want to monitor revenue and expenses so that I can evaluate financial performance.
- As a Data Analyst, I want to visualize financial trends so that I can communicate insights.
- As a Manager, I want to review different financial scenarios so that I can prepare future budgets.

## 6. Functional Requirements

### FR-01: Data Loading

- Load the two datasets independently.
- Support the verified input formats, initially targeting CSV.
- Validate required columns and data types.
- Handle missing or invalid data.

### FR-02: Data Cleaning

- Remove or investigate duplicate records.
- Handle missing values.
- Standardize financial values and date formats.
- Validate numeric fields and financial units.
- Preserve original raw datasets.

### FR-03: Budget Planning

- Organize budget information by period and category.
- Calculate planned revenue and expenses.
- Support monthly and quarterly budget analysis.
- Calculate budget allocation percentages.
- Allow users to explore budget scenarios.

### FR-04: Budget vs Actual Analysis

- Compare budgeted and actual amounts.
- Calculate absolute variance.
- Calculate variance percentage.
- Identify over-budget and under-budget categories.
- Display results by time period and category.

### FR-05: Financial Performance Analysis

- Analyze revenue and expenses.
- Calculate profit where valid cost and revenue data exist.
- Calculate profit margin where applicable.
- Compare financial performance across periods.
- Identify major expense categories.

### FR-06: Financial Forecasting

- Analyze historical financial trends.
- Build a basic forecasting model.
- Forecast revenue and expenses where sufficient historical data exists.
- Provide best-case, base-case, and worst-case scenarios.
- Display assumptions and limitations.

### FR-07: Interactive Dashboard

- Display financial KPIs.
- Provide filters by period and category.
- Visualize budget versus actual results.
- Display financial trends and forecast results.
- Present key analytical observations.

## 7. Non-functional Requirements

- The system should have a clear and understandable interface.
- Data processing should be reproducible.
- Financial calculations should be consistent and validated.
- The system should handle missing and invalid records gracefully.
- Dashboard components should respond to user filters.
- Code should be modular and maintainable.
- Project documentation should explain data sources, metrics, and assumptions.

## 8. Data Requirements

### Dataset A – Amazon Books Sales / Market Data

Potential fields:

- Book Name
- Author
- Genre
- Price
- Rating
- Reviews
- Year
- Units Sold or Sales Revenue, if available

Purpose:

- Analyze book pricing and market characteristics.
- Explore potential sales and revenue drivers.
- Provide business context for financial planning.

### Dataset B – Budget & Actual Financial Data

Required or target fields:

- Date / Period
- Financial Category
- Budgeted Revenue
- Actual Revenue
- Budgeted Expense
- Actual Expense
- Other relevant financial values, if available

Purpose:

- Budget planning.
- Budget versus actual comparison.
- Variance analysis.
- Financial forecasting.

**Data policy:**

- The datasets are independent analytical sources.
- Do not combine records unless a valid common key and compatible definitions exist.
- Do not assume book price represents revenue.
- Do not assume revenue represents profit.
- If synthetic budget data is used, label it clearly as simulated data.
- Document source, currency, units, date coverage, and metric definitions.

## 9. Scope & Limitations

### In Scope

- Financial data cleaning and processing.
- Budget planning analysis.
- Budget versus actual analysis.
- Variance analysis.
- Revenue and expense analysis.
- Basic financial forecasting.
- Interactive Streamlit dashboard.
- Financial reporting and business insights.

### Out of Scope

- Real-time Amazon financial data integration.
- Access to confidential Amazon internal financial records.
- Automated accounting or bookkeeping.
- Tax calculation and legal financial advice.
- Investment recommendations.
- Advanced financial risk modeling.
- Claims about actual Amazon profitability without supporting data.

### Limitations

- Analysis quality depends on dataset completeness and reliability.
- Historical data may not represent current market conditions.
- Forecasts are estimates, not guaranteed future results.
- Profit analysis requires appropriate cost and revenue data.

## 10. Acceptance Criteria

The project will be considered complete when:

1. Both datasets can be loaded and processed independently.
2. Data cleaning and validation steps are documented.
3. Financial metrics are calculated correctly.
4. Budget and actual values can be compared.
5. Variance and variance percentages are calculated correctly.
6. Financial trends can be visualized.
7. Basic forecasting is implemented with documented assumptions.
8. The dashboard provides interactive filters.
9. Financial insights are supported by data.
10. README and project documentation are available on GitHub.

## 11. Dashboard Requirements

The dashboard will contain five main pages.

### Page 1 – Financial Overview

Display:
- Total Budgeted Revenue
- Actual Revenue
- Total Budgeted Expenses
- Actual Expenses
- Actual Profit, if valid data is available
- Overall Budget Performance

### Page 2 – Budget Planning

Display:
- Budget allocation by category.
- Monthly and quarterly budgets.
- Planned revenue and expenses.
- Budget distribution charts.
- Budget scenario inputs or comparisons.

### Page 3 – Budget vs Actual

Display:
- Budget versus actual comparison.
- Absolute variance.
- Variance percentage.
- Over-budget categories.
- Under-budget categories.
- Monthly variance trends.

### Page 4 – Financial Performance

Display:
- Revenue trends.
- Expense trends.
- Profit and profit margin, where supported.
- Expense breakdown.
- Financial performance by period and category.

### Page 5 – Financial Forecasting

Display:
- Historical financial trends.
- Forecast revenue.
- Forecast expenses.
- Forecast budget requirements.
- Best-case, base-case, and worst-case scenarios.
- Forecast assumptions and limitations.

### Dashboard Filters

- Date / Period
- Financial Category
- Dataset Source
- Genre, where applicable
- Author, where applicable

Filters must only affect the relevant dataset and dashboard components.

## 12. Technical Requirements

### Technology Stack

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data processing |
| NumPy | Numerical calculations |
| Matplotlib / Seaborn | Statistical visualization |
| Plotly | Interactive charts |
| Streamlit | Interactive dashboard |
| Jupyter Notebook | Exploration and experimentation |
| VS Code | Development environment |
| Git / GitHub | Version control |

### System Architecture

Data Input → Data Validation → Data Cleaning → Financial Calculations → Financial Analysis → Forecasting → Dashboard.

### Proposed Project Structure

```text
amazon-books-budget-analytics/
│
├── data/
│   ├── raw/
│   │   ├── amazon_books.csv
│   │   └── budget_actual.csv
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
│   │   ├── data_loader.py
│   │   └── data_cleaning.py
│   │
│   ├── financial_analysis/
│   │   ├── budget_analysis.py
│   │   ├── variance_analysis.py
│   │   ├── performance_analysis.py
│   │   └── forecasting.py
│   │
│   └── utils/
│       └── financial_metrics.py
│
├── dashboard/
│   ├── app.py
│   └── pages/
│       ├── 01_financial_overview.py
│       ├── 02_budget_planning.py
│       ├── 03_budget_vs_actual.py
│       ├── 04_financial_performance.py
│       └── 05_forecasting.py
│
├── docs/
│   ├── PRD.md
│   └── data_dictionary.md
│
├── requirements.txt
├── README.md
└── .gitignore
```

### Development Principles

- Keep raw and processed data separate.
- Use modular Python functions.
- Avoid hardcoding financial values.
- Document financial formulas.
- Validate calculation results.
- Clearly distinguish actual, budgeted, and forecast values.
- Keep dataset sources and assumptions transparent.

---

**End of PRD – Version 2.0**
