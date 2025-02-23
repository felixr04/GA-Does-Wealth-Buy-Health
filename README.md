# Investing In Health

Life expectancy is often used as a key indicator of a nation’s overall well-being, yet significant disparities exist across countries and income groups. While it is widely known that wealthier nations tend to have higher life expectancies, the role of government health spending in mitigating inequalities in longevity is less clear. We will try to uncover this relationship because it is crucial for shaping national policy, especially in countries with high income inequality

Economic inequality, which for our puposes we will be using the Gini coefficient, has been linked to deaths and health, but whether increased public health investment can counteract this effect is still unclear. In countries where inequality is high, we can predict that low income individuals have less access to health clinics and foods rich in nutrition.

This project aims to analyze if government health spending influences life expectancy in countries with varying levels of income inequality. Using publicly available datasets from Gapminder, this study will explore trends over time, assess correlations between public health expenditure and life expectancy, and evaluate whether higher spending helps close the longevity gap between high- and low-income populations. The findings could provide insights into the effectiveness of policy implentations of the United Nations and help in reducing health disparities and improving overall quality of life.


# Data Dictionary

The date that we are using for this project is from gapminder.org. Gapminder is a non-profit organization that wants to change the way people think about the world by using data driven insights. Their resources are used by many people to help them understand the world through data.

*https://www.gapminder.org/*

Below you will find the data dictionary for the merged and cleaned dataset, merged_health_data.



|Feature|Type|Dataset|Description|
|---|---|---|---|
|country|object|merged_health_data|Name of the nation|
|year|int|merged_health_data|Year of observation|
|life_expectancy|float|merged_health_data|Life expectancyof a newborn if the current mortality rates at different ages were to stay the same throughout its lifetime. (In years)|
|gni_per_capita|float|merged_health_data|Total value of a country's income, both foriegn and domestic in US dollars.|
|gini_coefficient|float|merged_health_data|Measure of income inequality. Ranges from 0-100 with 100 being most ineaquality and 0 being least.|
|percent_gov_health_spending|float|merged_health_data|Government health spending as a percent of total government spending|


# Executive Summary
  

## Project Overview  
This project explores the relationship between government health spending, income inequality, and life expectancy. The goal is to determine whether increased public health investment mitigates the negative effects of inequality on longevity.  

## Problem Statement  
Income inequality is widely believed to impact health outcomes, particularly life expectancy. However, the extent to which government health spending counteracts these effects remains unclear. By analyzing global data, this project aims to uncover patterns and provide insights into the role of government health investment.  

## Methodology  
- **Data Sources:** Four datasets spanning from 1800 to 2100, containing statistics on life expectancy, Gini coefficient (income inequality), government health spending, and Gross National Income (GNI) per capita. The Data is provided to us via Gapminder.  
- **Data Cleaning:** Standardized country names, handled missing values, converted financial figures, and filtered for relevant years (1990–2010).  
- **Exploratory Data Analysis (EDA):** Used correlation analysis, scatter plots, and regression models to explore relationships between key variables.  
- **Statistical Analysis:** Calculated correlation coefficients and p-values to assess statistical significance.  

## Key Findings  
1. **Income inequality negatively correlates with life expectancy (-0.41).** Countries with greater income disparity tend to have lower average lifespans.  
2. **Government health spending positively correlates with life expectancy (0.65).** Nations that allocate more public funds to healthcare generally have longer life expectancies.  
3. **No significant relationship between inequality and health spending.** This suggests that simply increasing health budgets may not directly address the effects of inequality.  
4. **Visualizations highlight trends and key countries** A bubble chart of global data (filtered for clarity) shows key countries with different spending levels and life expectancies. Regresional visualizations help showcase relationships and trends between variables.  

## Conclusion & Implications  
While greater government health spending is linked to longer life expectancy, it does not appear to directly reduce the impact of income inequality on health outcomes. Policymakers should consider complementary strategies, such as improving healthcare accessibility, preventive care, and nutritional care to address the health consequences of inequality.  

## Next Steps  
- **Deeper Causal Analysis:** Use advanced modeling to better understand if our correlations are causal.  
- **Additional Health Indicators:** Incorporate metrics such as infant mortality, disease burden, or access to healthcare to provide a more comprehensive view of public health outcomes.  
- **Policy Simulations:** Estimate the impact of potential interventions, such as universal healthcare expansion or income redistribution policies.  

