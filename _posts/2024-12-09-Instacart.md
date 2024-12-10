---
layout: post
title: Customer Behavior Analysis
excerpt: Leveraging Data-Driven Insights to Refine Marketing Strategies in Online Grocery Sales
image: /images/Instacart/inst-logo.png
---

![Cover Photo]({{ site.baseurl }}/images/Instacart/inst-logo.png){:width="100"}

## Background

**Instacart**, a leading online grocery platform, wanted deeper insights into their customer base to strengthen their targeted marketing efforts. By analyzing when customers shop, what they buy, and how these behaviors differ across demographics, we aimed to help the marketing and sales teams make more informed decisions. Collaborating closely with these teams, we translated their high-level questions—such as identifying peak shopping times, understanding product popularity, and segmenting customers by loyalty and region—into concrete, data-driven tasks. This cross-functional approach ensured that insights were both actionable and closely aligned with Instacart’s strategic priorities.

## Data

The analysis was conducted using the **2017 Instacart Online Grocery Shopping Dataset** (obtained via Kaggle), along with a supplemental customer dataset. Together, these files contained millions of records detailing order history, product attributes, and basic customer characteristics. After thorough data cleaning—such as handling missing values and outliers, adjusting column types, and merging multiple tables—our final dataset was ready for exploratory analysis and visualization. 

<p align="center">
<img src="/images/Instacart/Customer_Profile_Distributions.png" width="800">
</p>

The scale of the data demanded careful attention to efficiency, ensuring that memory usage and processing time remained manageable. By employing best practices in data wrangling with **pandas**, **NumPy**, and other Python libraries, we prepared a dataset that accurately represented Instacart’s diverse customer base and their purchasing behaviors.

## Analysis

The analysis combined descriptive statistics, data visualizations, and the creation of customer segments based on factors like loyalty, spending habits, and order frequency. We examined patterns such as:

- **Peak Ordering Times:** Identified the busiest days and hours to support time-sensitive marketing campaigns.
  
<p align="center">
<img src="/images/Instacart/orders_by_hour_histogram.png" width="600">
</p>

- **Spending Patterns:** Investigated when customers spend the most money and how product pricing tiers could be simplified to target different audiences.

<p align="center">
<img src="/images/Instacart/filtered_prices_histogram.png" width="600">
</p>
 
- **Product Popularity:** Explored which departments—such as produce, dairy, or beverages—consistently lead in sales volume, and identified lower-performing categories for improvement.

<p align="center">
<img src="/images/Instacart/Product_Department_Sales2.png" width="600">
</p>

- **Customer Segmentation:** Grouped customers based on loyalty (e.g., frequent returners vs. occasional shoppers), age and family status (e.g., young parents vs. large families), and region to reveal nuanced differences in purchasing habits. For example, we found that certain customer segments gravitate toward bulk, staple items, while others show a preference for premium products.

<p align="center">
<img src="/images/Instacart/purchases_by_department_top_5_profiles_stacked.png" width="900">
</p>

Throughout the process, we communicated preliminary findings back to sales and marketing stakeholders. Their feedback guided us to refine our queries, dive deeper into certain trends, and adjust our visualizations for maximum clarity and impact.

### Findings

- **Time of Day & Day of Week:** Afternoon and late morning emerged as peak shopping times, suggesting that promotions and ads during quieter periods—like weekday evenings—could capture new attention.
- **Price Sensitivity & Loyalty:** Customers with higher loyalty tended to purchase more frequently but spent slightly less per item, possibly due to familiarity with Instacart’s offerings. Newer customers often purchased higher-priced items initially, creating an opportunity for upselling during early touchpoints.
- **Demographic & Regional Differences:** Some regions showed a higher prevalence of weekend bulk orders, while certain age and family-status groups favored specific product categories (e.g., young families leaning toward fresh produce and baby care items).
- **Product Category Opportunities:** While produce and dairy dominated sales, departments like alcohol, meat/seafood, and niche health items showed room for growth. This indicated that curated promotions, targeted recommendations, or partnering with certain suppliers could drive improvements in underperforming segments.

<p align="center">
<img src="/images/Instacart/top_product_pairs_horizontal.png" width="800">
</p>

## Recommendations

1. **Time-Targeted Campaigns:** Consider launching morning or late-night promotions, especially for high-margin products, to leverage quieter order periods.  
2. **Segment-Specific Offers:** Develop loyalty-based discount tiers or referral bonuses. For example, incentivize bulk-buying families on weekends or encourage new, high-spending customers to try additional premium products.  
3. **Simplify Price Ranges:** Introduce clear product price tiers (low, mid, high) to streamline marketing messages and help customers quickly identify the value proposition of promoted items.  
4. **Category-Focused Strategies:** Offer targeted deals in underutilized departments—like alcohol or specialty beverages—during times when their core audience is most active.

## Limitations and Future Work

Our analysis relied on historical data, without factoring in seasonal variations, emerging trends, or regional holidays. Integrating external data (e.g., weather patterns, cultural holidays) could further refine recommendations. Additionally, exploring more advanced modeling, such as propensity scoring or market basket analysis, might reveal new cross-selling opportunities. Ongoing stakeholder feedback and iterative testing will ensure that strategies remain aligned with shifting consumer dynamics and competitive pressures.

## Conclusion

This project demonstrates how translating broad business questions into structured, data-driven analysis can yield actionable insights. By leveraging Instacart’s sales and customer data, we identified peak shopping times, profitable customer segments, and opportunities for tailored marketing campaigns. Through close collaboration with marketing and sales teams, we ensured that these insights are ready to drive more effective, targeted strategies—ultimately enhancing the customer experience and improving business outcomes.
