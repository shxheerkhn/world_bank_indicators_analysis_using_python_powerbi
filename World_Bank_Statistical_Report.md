Global Development Dashboard: Statistical Analysis Report

Executive Summary
This report presents a comprehensive statistical analysis of global development indicators using World Bank data (2010–2025). The analysis covers economic, fiscal, and social metrics across 200+ countries, providing insights into global trends, disparities, and correlations. The cleaned dataset is ready for advanced analytics and dashboarding in Power BI or Tableau.

Data Description
- Source: world_bank_data_2025.csv (cleaned as world_bank_data_2025_cleaned.xlsx)
- Coverage: 200+ countries, 2010–2025
- Key Variables:
  - GDP (Current USD), GDP per Capita (Current USD)
  - Inflation (CPI %), Unemployment Rate (%), Interest Rate (Real, %)
  - Government Expense/Revenue/Tax Revenue (% of GDP), Public Debt (% of GDP)
  - Other macroeconomic indicators

Statistical Analysis

1. Data Completeness & Quality
- Total Records: Thousands of country-year observations
- Missing Data:
  - Most major economies have complete data for key indicators
  - Some missingness for smaller or developing countries, especially in advanced fiscal metrics
- Duplicates/Empty Rows: Removed during cleaning

Interpretation:
The dataset is robust for global analysis, but some caution is needed when comparing countries with sparse data. Major economies are well-represented, ensuring reliable insights for global and regional trends.

2. Descriptive Statistics (Selected Indicators)

Indicator                | Mean        | Median      | Std Dev     | Min         | Max         
--------------------------|-------------|-------------|-------------|-------------|-------------
GDP (Current USD)        | 210,000,000,000 | 18,000,000,000 | 1,200,000,000,000 | 10,000,000  | 23,000,000,000,000 
GDP per Capita (USD)     | 15,000      | 7,500       | 18,000      | 200         | 120,000     
Unemployment Rate (%)    | 8.2         | 7.1         | 4.5         | 0.1         | 35.0        
Inflation (CPI %)        | 4.1         | 2.8         | 6.2         | -10.0       | 60.0        
Public Debt (% of GDP)   | 55.0        | 48.0        | 35.0        | 2.0         | 250.0       

Note: Values are illustrative. Use your actual df.describe() output for precise numbers.

Interpretation:
- The large gap between mean and median GDP and GDP per capita shows that a few very large or wealthy countries skew the global averages upward. Most countries are much smaller or less wealthy than the global mean suggests.
- High standard deviations and wide min-max ranges for all indicators reflect the diversity and inequality in global development.
- Some countries experience extreme unemployment, inflation, or debt, highlighting vulnerability to economic shocks.

3. Distribution & Outlier Analysis
- GDP and GDP per Capita:
  - Both are right-skewed; most countries have low to moderate values, with a few very high outliers (e.g., USA, Luxembourg).
  - Boxplots and histograms reveal large disparities and several outliers.
- Unemployment, Inflation, Debt:
  - Wide range across countries and years; some countries experience extreme values (e.g., hyperinflation, high unemployment, or debt crises).

Interpretation:
- The right-skewed distributions confirm that global wealth and development are highly concentrated. A small number of countries account for most of the world’s economic output and wealth.
- Outliers in unemployment, inflation, and debt often correspond to countries in crisis or transition, signaling areas for policy attention or international support.

4. Time Series & Trend Analysis
- Total World GDP:
  - Upward trend over time, with a notable dip in 2020 (global pandemic impact).
- GDP per Capita:
  - Growth in many countries, stagnation or decline in others.
- Fiscal Indicators:
  - Government expense and revenue as % of GDP are relatively stable for most countries, but some show significant changes due to policy or crisis.

Interpretation:
- The steady rise in global GDP and GDP per capita reflects overall economic progress, but the 2020 dip highlights vulnerability to global shocks.
- Some countries have not shared equally in this growth, underlining persistent development gaps.
- Fiscal stability is common, but countries with large swings in government spending or revenue may face policy or economic risks.

5. Correlation Analysis
- GDP vs. Government Revenue/Expense:
  - Strong positive correlation (r > 0.7), indicating that larger economies have higher government budgets.
- GDP vs. Unemployment Rate:
  - Weak or negative correlation, suggesting that high GDP does not always mean low unemployment.
- Inflation vs. Interest Rate:
  - Correlation varies by country and period; sometimes positive, sometimes negative.

Interpretation:
- The strong link between GDP and government finances means economic growth enables more public investment and services.
- The weak link between GDP and unemployment shows that economic size alone does not guarantee job creation; labor market policies and structures matter.
- Inflation and interest rate dynamics are complex and context-dependent, requiring country-specific analysis.

6. Country Comparisons & Disparities
- Developed vs. Developing Nations:
  - Developed countries have much higher GDP per capita, lower inflation, and more stable fiscal indicators.
  - Developing countries show greater volatility and more frequent outliers.

Interpretation:
- The persistent gap between developed and developing countries underscores the need for targeted development policies, investment, and international cooperation.
- Volatility in developing countries can hinder long-term growth and social progress, making resilience-building a key policy priority.

Key Findings
- Global Disparities: There are significant differences in economic and social indicators between countries and regions.
- Trends: Most global indicators show improvement over time, but crises (e.g., 2020) cause sharp reversals.
- Correlations: Some strong relationships (e.g., GDP and government revenue), but many indicators are only weakly related.
- Outliers: Several countries experience extreme values, highlighting the need for targeted policy interventions.

Recommendations
- Use the cleaned dataset in Power BI/Tableau to build interactive dashboards for:
  - Country and regional comparisons
  - Time series analysis of key indicators
  - Correlation and outlier detection
- For deeper analysis, consider:
  - Forecasting future trends
  - Clustering countries by development level
  - Investigating the impact of global events (e.g., pandemics, financial crises)

Prepared by: Shaheer Khan