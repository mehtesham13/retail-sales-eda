# Retail Sales Exploratory Data Analysis

What drives revenue in a year of retail transactions? This notebook checks data quality, profiles customers and products, looks at sales over time and turns the results into business recommendations.

## Data

1,000 transactions from January 2023 to January 2024 with date, customer ID, gender, age, product category (Beauty, Clothing, Electronics), quantity, unit price and total amount.

## What the notebook covers

1. Data quality: missing values, duplicates, a check that quantity × price equals the total
2. Descriptive statistics, skewness and kurtosis
3. Customer demographics and product categories
4. Monthly and day-of-week sales trends
5. Correlations between variables
6. IQR outlier detection
7. Business insights and recommendations

## Findings

- **Total revenue $456,000**, average transaction $456. Every customer ID appears once, so the data supports no repeat-purchase analysis.
- **Unit price drives transaction value:** correlation 0.85 between price per unit and total amount.
- **Electronics earns the most** ($156,905, 34.4% of revenue). Clothing has the most transactions (35.1%).
- **May was the best month** ($53,150) and September the worst ($23,620), a 125% swing worth planning inventory around.
- **Saturday is the top day**, but weekdays still bring in 70% of revenue.
- **Customers aged 46–55 spend the most** in total ($100,690).
- Female and male customers spend almost the same per transaction ($457 vs $455).
- No outliers by the IQR rule and no data quality problems.

## How to run

```bash
git clone https://github.com/mehtesham13/Retail-Sales-Exploratory-Data-Analysis.git
cd Retail-Sales-Exploratory-Data-Analysis
pip install pandas numpy matplotlib seaborn scipy scikit-learn openpyxl
jupyter notebook "retail_sales_eda_comprehensive---.ipynb"
```

Course: CS667 Practical Data Science, Pace University

Author: Muhammad Ehtesham · [LinkedIn](https://www.linkedin.com/in/muhammad-ehtesham-dsa)
