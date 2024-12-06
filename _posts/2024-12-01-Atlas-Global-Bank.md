---
layout: post
title: Atlas Global Bank
excerpt: Identifying Investment Opportunities in Emerging Markets Through Macroeconomic Performance Analysis
image: /images/Smart_Energy_Building/Cover-photo.png
---

![Cover Photo]({{ site.baseurl }}/images/Smart_Energy_Building/Cover-photo.png){:width="700"}

## Background

In an increasingly competitive financial landscape, **Atlas Global Bank** seeks to optimize its global presence by expanding into emerging markets with strong investment potential. Recognizing that macroeconomic indicators can provide valuable insights into a country's economic health and growth prospects, the bank aims to identify regions where its products and derivates can thrive. This project leverages supervised and unsupervised machine learning techniques to analyze key economic indicators—such as GDP growth, consumption rates, inflation, unemployment, and foreign direct investment inflows—to segment countries based on economic performance. The goal is to provide data-driven insights that will guide strategic decisions on international expansion, ensuring a targeted approach to maximize return on investment.

## Data

The analysis utilized macroeconomic data sourced from the **World Bank's World Development Indicators (WDI)**. Additionally, the project referenced **Nasdaq's analysis of top emerging markets** to identify potential target countries. The data underwent rigorous cleaning and transformation processes to ensure accuracy and consistency, including handling missing values, managing outliers, and restructuring the data for effective year-over-year comparisons.

<p align="center">
<img src="images/Atlas_Global_Bank/world_bank_logo.png" width="600">
</p>

## Analysis

### Exploratory Data Analysis

The analysis began with an exploratory examination of the relationships between economic indicators. A primary hypothesis posited that an increase in a country's GDP growth would correlate with an increase in consumption growth, suggesting a positive relationship between economic expansion and consumer spending. 

<p align="center">
<img src="images/Atlas-Global-Bank/correlation_matrix_heatmap.png" width="600">
</p>

The results revealed a slope of 0.80; however, the data points are spread out. The MSE is 3.77, and the R² score is 0.73, indicating that the model explains 73% of the variation in consumption growth. Findings indicated a general positive trend; however, the relationship was not strictly linear. Factors such as inflation and unemployment also significantly influence consumption patterns—high inflation can erode purchasing power, while high unemployment can reduce overall economic activity.

<p align="center">
<img src="images/Atlas-Global-Bank/GDP_vs_Consumption_Growth_Regression.png" width="600">
</p>

### Clustering Analysis

To capture the complexities of economic data, the analysis adopted **k-means clustering**, an unsupervised machine learning technique. This approach segmented countries into distinct clusters based on multiple economic indicators. Three economic profiles emerged:

<p align="center">
<img src="images/Atlas-Global-Bank/gdp_vs_consumption_clusters.png" width="600">
</p>

- **Cluster 0 (Moderate Growth, Stable Economies):** Countries with consistent GDP growth, moderate savings rates, lower inflation, and stable trade growth. These economies offer stability and predictability, making them favorable for banking services and investment.

- **Cluster 1 (High Consumption, Varied GDP):** Countries with high consumption growth but economic volatility. While high consumption indicates potential demand for banking services, economic instability presents higher risks.

- **Cluster 2 (Low or Negative Growth):** Countries with low or negative GDP growth, high unemployment, and less attractive investment climates. These economies pose significant challenges for expansion.

<p align="center">
<img src="images/Atlas-Global-Bank/conclusion.png" width="600">
</p>

### Findings

Cluster 0 countries emerged as the most promising candidates for expansion, aligning with the bank's objective of targeting regions with strong investment potential and lower risk profiles. In contrast, Cluster 1 countries require cautious entry strategies, and Cluster 2 countries are unsuitable for immediate expansion.

## Recommendations

- **Prioritize Cluster 0 countries:** Focus on stable emerging markets with favorable economic conditions to optimize return on investment.
- **Approach Cluster 1 cautiously:** Conduct thorough market research and develop tailored strategies to mitigate risks.
- **Avoid Cluster 2 for now:** Due to challenging economic conditions, these markets are not recommended for immediate expansion.

<p align="center">
<img src="images/Atlas-Global-Bank/gdp_growth_by_country.png" width="600">
</p>

## Limitations and Future Work

This analysis primarily focused on macroeconomic indicators, excluding sector-specific data such as banking penetration rates or technological adoption levels. Future analyses should incorporate additional variables like interest rates and sector-specific trends to refine market potential assessments. A deeper examination of the competitive dynamics, customer behavior, and regulatory challenges within the banking sector of target countries will enhance the precision of investment strategies.

## Conclusion

By applying machine learning techniques to comprehensive economic data, the project provided actionable insights for **Atlas Global Bank's** international expansion strategy. Targeting stable emerging markets with favorable economic conditions will enable the bank to optimize its global presence and maximize returns. This data-driven approach ensures that expansion efforts are informed by a nuanced understanding of each market's economic profile, increasing the likelihood of successful market entry and sustained growth.
