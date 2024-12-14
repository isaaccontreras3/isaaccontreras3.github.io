---
layout: post
title: Optimizing Medical Staffing for Influenza Season
excerpt: Leveraging Data-Driven Forecasting to Allocate Resources and Support Vulnerable Populations
image: /images/Flu_Season/flu_logo.png
---

![Cover Photo]({{ site.baseurl }}/images/Flu_Season/flu_logo.png){:width="600"}

## Background

Each year, the **United States faces an influenza season** in which hospital admissions rise steeply. Particularly hard hit are vulnerable populations—older adults, pregnant women, young children, and those with chronic illnesses. To cope with this surge, a medical staffing agency supplies additional nurses, physician assistants, and doctors to healthcare facilities across all 50 states. However, with limited personnel available, the agency must optimize staffing allocation based on data-driven forecasts of flu surges.

This project’s objective: **Determine when to send additional staff, how many, and to which states** to meet seasonal spikes in demand while focusing on protecting vulnerable populations. Leveraging **CDC datasets** on influenza trends and **US Census data** on demographics, we built a comprehensive analysis that offers proactive measures—ensuring hospitals and clinics have sufficient coverage without overextending staffing budgets. Throughout this project, **data privacy and ethics remained a priority** as well PII was handled with the best and professional practices for data security and confidentiality. 

## Data

To accurately forecast staffing requirements, I combined two robust data sources: historical influenza death records from the CDC and detailed population demographics from the US Census Bureau. By merging these datasets, I captured age-based distributions (with special attention to children under five and adults over 65) to build comprehensive vulnerability indices. Where certain death counts were suppressed or under-reported, I employed **statistical imputation and comparative analysis** across similar states. These steps ensured a reliable, ethically sound data pipeline, free from PII.

[Data Limitations](https://u.pcloud.link/publink/show?code=XZ5cQ55ZpDvFtz50zNbj7gM2dQtbGVVDcNMX)

## Analysis

I performed a **time-series analysis** of historical flu surges from 2009–2017, detecting strong seasonal patterns peaking between December and February. Leveraging **descriptive statistics and forecasting techniques**, I modeled how flu waves would stress limited staffing resources. Next, I developed a vulnerability index by correlating flu mortality with demographic segments, revealing a 90%+ relationship between high-risk age groups and flu-related deaths. Incorporating advanced [Tableau Visualizations](https://public.tableau.com/app/profile/isaac.contreras/viz/2_10Final/Story1), I mapped per-state projections to identify where extra medical personnel could meaningfully reduce hospital strain. 

[Tableau Complete Presentation Link](https://public.tableau.com/app/profile/isaac.contreras/viz/2_10Final/Story1)
<p align="center">
<img src="/images/Flu_Season/flu_season.png" width="950">
</p>

## Findings

The results spotlighted Florida, Texas, California, and several northern states (notably New York and Illinois) as top priorities due to their larger populations of infants, seniors, and immunocompromised individuals. **My analysis indicates that allocating approximately 5,000 nurses and 1,020 doctors** across the seven most impacted states during peak weeks can maintain a stable 90% or better staff-to-patient ratio. This strategic deployment—timed two weeks before the typical outbreak—significantly mitigates bottlenecks at local healthcare facilities.
[Interim Report](https://u.pcloud.link/publink/show?code=XZFQEI0ZQ0W8IgoW8kQrm997dXaOKSyjgtGy)

## Recommendations

Based on these insights, I recommend proactively shifting staff into high-vulnerability regions ahead of expected spikes. Offering flu-shot incentives for at-risk demographics can further flatten the seasonal curve, cutting down emergency visits. Meanwhile, rotating employees between lower- and higher-risk states allows real-time adjustments if new hotspots emerge. I also emphasize cross-training staff for pediatric and geriatric needs and deploying data-driven dashboards to monitor resources, identify emerging hotspots, and ensure compliance with privacy guidelines.

## Conclusion

By marrying demographic data with historical flu trends, I delivered a targeted staffing plan that helps avoid both understaffing and over-allocation. This project demonstrates my ability to collect, clean, and integrate large datasets, perform statistical analyses, and craft actionable recommendations using compelling visual narratives. Leveraging these methods and my commitment to data ethics, I’m confident in my capacity to support stakeholders with clear, impactful insights—ultimately enhancing patient outcomes during influenza season.
