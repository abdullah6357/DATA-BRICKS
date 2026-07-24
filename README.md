# DATA-BRICKS
A Databricks Lakehouse project focused on United States GHG (Greenhouse Gas) Emissions Analysis.
This repository contains SQL queries, datasets, and a Lakehouse Dashboard for exploring and visualizing CO₂-equivalent emissions data across states and counties.
## Project Overview
The project analyzes U.S. emissions data (in million metric tons of CO₂e) with visualizations and aggregations including:
```
. Emissions per location (geospatial)
. Emissions per person
. State-level total emissions
. Top emitters by county/state
. Percentage contribution of top states to national total
```
## Repository Contents
1. Emissions Dashboard (Emissions Dashboard.lvdash.json)
```
. Lakehouse Dashboard configuration for Databricks.
. Includes multiple interactive visualizations:
. Symbol Map: Emissions by geographic location (latitude/longitude).
. Scatter Plot: Emissions per person vs. population.
. Pie Chart: Top states by emission share.
. Bar Chart: Top 10 counties by total emissions.

Built using datasets defined as SQL queries.
```
2. SQL Query Notebooks (.dbquery.ipynb)
These are Databricks SQL notebooks containing exploratory queries:
```
. Top 10 States by Total Emissions
. Top 10 States - Percentage Share & Cumulative Contribution (with CTEs for national totals)
. Top 10 Counties by Total Emissions ("County Shaming")
. Additional supporting queries for per-person emissions and location data.
```
All queries target the table emissions.default.emissions_data (or catalog emissions).
## Technologies Used
```
=> Databricks Lakehouse
=> SQL (Spark SQL)
=> Lakehouse Dashboards (.lvdash.json)
=> Geospatial visualization
=> Data aggregation & window functions
```


## Key Insights Available
```
. Which states and counties contribute the most to U.S. emissions.
. Emissions intensity per capita.
. Geographic distribution of emission sources.
. Concentration of emissions (top 10 states' share of national total).
```


