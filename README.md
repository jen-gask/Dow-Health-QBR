# Dow Health Quarterly Business Review
## Background
Dow Health is a healthcare company with a strong consumer component. Interested in having a dashboard for future quarterly business review meetings, the Reporting and Insights Manager requested a resource that explores the impact of marketing campaign categories used starting in 2019 reporting up until the term to-date.

### Goal
Provide a dashboard that can answer the following:
- What are the values for the most important marketing and signup metrics?
- What are the to-date value for key marketing metrics, signup metrics, and claim metrics for each campaign category?
- What are the overall trends by category for signups and claim amounts? How are these distributed across categories?
- How does performance compare across categories?
- Can we slice all of the above by plan, state, and category type?

## Process/Methodology
1. Requirements: The initial request lists metrics that require agreed upon definitions, dimensions defined, and timeline/prioritization. Meet with the R & I Manager to clarify metric definitions, dimensions, and timelines/prioritization.
2. Create a template: Build out a rough proof of concept dashboard draft in a spreadsheet based on asks, to share with the stakeholder and align on the look before building out the full dashboard. Created callout boxes for north star metrics, tables for values reporting, line graph for KPI trends over time, area graph for KPI over dimension over time, bar graphs for KPI comparisons, and included fitering to segment on dimension. 
3. Import the data for review and cleaning: Using BigQuery, extracted and loaded 3 tables for exploration to understand the columns, structure, relationships, formatting, and prepare for cleaning. Found that the tables were essentially already ready for analysis. The analysis would require the creation of additional metrics not listed to be added in Tableau during dashboard build: cost per click (CPC), click through rate(CTR), cost-per-impression, cost per signup, signup rate, sign up count. 
4. Dashboard build: Loaded the tables into Tableau, built the appropriate table relationships and began EDA. Created new calculated fields to add the KPIs within Tableau. Built big numbers to show the KPI snapshots, followed the rest of the template plan adjusting for size and giving each metrics area a specific section of the dashboard.

## Summary
While several campaigns demonstrate strong click-through rates (CTR), not all are converting efficiently, and others show signs of declining effectiveness or inefficiency. Strategic next steps include scaling high performers, revisiting underperformers for copy and offer revisions, and leveraging lessons from the top-converting campaigns across the portfolio.

## Insights
Overall
- Most campaigns peaked in April 2020 due to pandemic-related demand, which drove a spike in signups. But two campaigns, *Compare Health Coverage* and *Tailored Health Plans*, hit their highest performance later in 2021. The former coincided with increased investment, and the latter aligned with open enrollment. The performance of these campaigns and highlights the importance of timing and budget alignment.
Strong Conversions
- *Health For All* leads with an 8.16% signup rate and one of the highest CTRs despite low impressions. It should be prioritized for additional resources and potentially serve as a model for other campaigns.
- With a 4.76% signup rate, *Coverage Matters* shows strong performance. Elements from both this and *Health For All* should be analyzed and replicated where applicable.
Scaling CTR
- Both *Health For All* and *Benefit Updates* combine high CTR with low impressions. These campaigns are opportunities for better utilization and should be scaled after confirming there are no delivery issues.
Summer CTR-Signup Disconnect
- *Summer Wellness Tips* used to drive strong seasonal signups, but that’s slowed down in recent years. CTR is still high, so interest is there, but fewer people are converting. It’s worth digging into why that might be: messaging misalignment, timing, and targeting could all be factors.
Golden Years Underperformance
- *Golden Years Security* features the lowest CTR, the highest CPC, and the lowest claim amount. With low impressions and no clear external reason for underdelivery, a full review of its delivery, copy, and offer is recommended. If no improvement potential is found, consider sunsetting.


## Resources
Dashboard: [Here](https://public.tableau.com/views/DowHealthQBR/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
<div class='tableauPlaceholder' id='viz1750810839756' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Do&#47;DowHealthQBR&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a>
