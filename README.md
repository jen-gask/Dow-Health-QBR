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
5. Performance analysis: Presentation deck created for the Reporting and Insights Manager to share at the next QBR that answers the requested questions and highlight KPI performance using the dashboard.

## Insights
- Both campaigns Benefit Updates and Health For All have very high CTR and low impressions. While both campaigns should be evaluated for any ad issues, they should both be given high priority for their top performing CTR and more resources should be invested in scaling these campaigns up.
- Summer Wellness Tips used to be a promising seasonal driver of signups but has slumped in recent years while CTR remains high. We should experiment look deeper into what the disconnect between clicks and signups.
- The Golden Years Security has impressions on the lower end and very low CTR while having the highest CPC. It also carries the lowest claim amount and highest cost per sign up. This campaign should be evaluated for delivery issues as well as copy and offer efficacy, potentially even sunsetting if there are no technical issues to be found. 
- Campaign with the best overall signup rate is Health For All campaign at 8.16%. Health For All is not so closely, following by Coverage Matters at 4.76%. Dow should seek to replicate the applicable campaign tactics across other campaigns.
- Most campaigns saw a spike in signup activity in April 2020 due to pandemic-related influx. These influxed represented apex performance for all but two campaigns which both saw their apex performance later in 2021. The campaigns are Compare Health Coverage in 2021 and Tailored Health Plans in September 2021, the latter is likely due to the proximity to open enrollment while the former is due to bigger investment into the Compare Health Coverage campaigns as claim amounts for this campaign also ballooned between December 2020 and February 2023.
