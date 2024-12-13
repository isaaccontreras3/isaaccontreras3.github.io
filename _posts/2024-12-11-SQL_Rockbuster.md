---
layout: post
title: Adapting to the Streaming Era
excerpt: SQL Data-Driven Insights to Guide the Strategic Transition of an Online Video Service
image: /images/SQL_Rockbuster/rockbuster_logo.png
---
![Cover Photo]({{ site.baseurl }}/images/SQL_Rockbuster/rockbuster_logo.png){:width="500"}

## Background

Rockbuster Stealth LLC, once a global chain of movie rental stores, now faces a digital era dominated by streaming giants. To secure their foothold, they plan to leverage existing film licenses and pivot to an online video rental platform. As the Data Analyst on the BI team, I distilled high-level business questions—ranging from top-performing markets to customer segmentation—into data-driven insights. This guided stakeholders in refining content acquisition, pricing strategies, and promotional campaigns for a more competitive 2020 launch.

## Data

The analysis leveraged a **relational database** containing Rockbuster’s historical rental data, inventory details, customer demographics, payment records, and country/city-level information. Data was sourced from multiple CSV files and loaded into a **PostgreSQL** database using industry-standard ETL processes. This relational schema allowed for complex **SQL** queries, **JOINs**, and **OLAP**-style aggregations.

[ERD Diagram](https://u.pcloud.link/publink/show?code=XZw2OI0Zq1iIMgwH4fHcVu8K5AX6pyJ02mX7):
<p align="center">
<img src="/images/SQL_Rockbuster/ERD-extraction.png" width="800">
</p>

Key aspects of data handling included:

- **Data Wrangling & Cleaning:** Ensured accurate data types, managed null values, and standardized field formatting.
- **Entity-Relationship Diagrams & Data Dictionaries:** Created documentation to maintain data integrity and transparency.
- **Efficient Query Design:** Used indexing and well-structured queries to handle large datasets and improve performance.

By combining **CRUD operations**, **complex joins**, **nested subqueries**, and **common table expressions (CTEs)**, I performed exploratory and diagnostic analyses to reveal meaningful patterns. The data ultimately served as a reliable basis for building visualizations and generating insights.

## Analysis

The analysis centered on uncovering revenue drivers, identifying high-value customers, and understanding geographic trends. By examining which countries and cities yielded the most profit, pinpointing segments with strong lifetime value, comparing purchasing power across regions, exploring top-performing film categories, and evaluating rental durations alongside pricing strategies, we ensured the findings would directly inform strategic decisions for the online video launch. Throughout the process, I leveraged a combination of SQL joins, CTEs, subqueries, and filtering techniques to efficiently extract and transform data. This data-driven approach enabled the BI team to move from broad, high-level questions to actionable insights grounded in empirical evidence.
[Queries Made](https://github.com/isaaccontreras3/SQL_Rockbuster_Stealth_LLC/tree/master/02%20Queries%20%26%20Analysis)

<p align="center">
<img src="/images/SQL_Rockbuster/Financial-Snapshop-RB.png" width="800">
</p>

### Findings

- **Global Revenue Leaders:** India, China, and the U.S. drove revenue, with cities like London and Saint-Denis emerging as prime targets for early promotions. [Tableau Dashbord of Leader Category by Revenue](https://public.tableau.com/app/profile/isaac.contreras/viz/LeaderCategorybyRevenue/CategorybyRevenueinCounrty)
- **High-LTV Customers:** Cities like London, Udaipur, and Aurora hosted customers with exceptional lifetime value, supporting personalized loyalty initiatives.  
- **Purchasing Power vs. Revenue:** While Asia topped raw revenue, Europe and Africa showed higher purchasing power, signaling untapped market potential.  
- **Regional Content Preferences:** Sports dominated India and the U.S., while Animation thrived in China, emphasizing the need for region-specific content strategies.

## Recommendations

1. **Target High-Performing Markets:** Launch initial promotions in India, China, and the U.S. to capitalize on existing demand.  
2. **Personalize Offers for High-LTV Customers:** Develop loyalty programs and exclusive deals for top-value customers in key cities to drive retention.  
3. **Expand in Underutilized Regions:** Tailor content and pricing to European and African markets, leveraging their high purchasing power for growth.  
4. **Localize Content Acquisition:** Invest in regionally preferred categories—such as Sports in India and the U.S., and Animation in China—to boost engagement and viewer satisfaction.  
5. **Refine Pricing & Rental Duration:** Align pricing models and rental periods (around 5 days) with consumer habits, encouraging longer engagement and optimized revenue streams.

<p align="center">
<img src="/images/SQL_Rockbuster/PurPower_vs_Reve.png" width="800">
</p>

[Complete Case Study Sent to Client](https://u.pcloud.link/publink/show?code=XZ2fy55ZsAsJmyyqAX7rPxc3QYs52klSPFsk)

## Limitations and Future Work

This analysis is based on historical data and may not fully account for seasonal events, cultural holidays, or emerging industry trends. Integrating external data sources—such as weather patterns, local festivities, and competitor analyses—could enhance the precision of insights. Future efforts might include deploying machine learning models for advanced predictive analytics, implementing recommendation systems, and continuously refining our approach based on stakeholder feedback and evolving market conditions.

## Conclusion

By effectively utilizing SQL in an OLAP environment and performing comprehensive ETL tasks, we transformed Rockbuster’s historical data into strategic guidance. The resulting insights shaped recommendations for targeted marketing, personalized retention efforts, content localization, and pricing optimization. As Rockbuster Stealth LLC transitions into the online video rental space, these data-driven strategies will help the company adapt swiftly and compete more effectively in a rapidly changing digital entertainment landscape.
[Complete Case Study Sent to Client](https://u.pcloud.link/publink/show?code=XZ2fy55ZsAsJmyyqAX7rPxc3QYs52klSPFsk)
