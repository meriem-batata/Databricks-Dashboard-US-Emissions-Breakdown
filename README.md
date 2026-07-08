# 🇺🇸 US Emissions Breakdown — Databricks Dashboard

My first Databricks project: analysis and visualization of greenhouse gas (GHG) emissions across the United States at the county level, using data from the **EPA (Environmental Protection Agency)** collected in 2023.

## 📊 Dashboard Overview

![Dashboard overview](images/dashboard_overview.png)

The dashboard cross-references total emissions with population by county, highlighting the relationship between population density and per-capita emissions.

![Top 10 emitting states and counties](images/dashboard_top_counties.png)

**Key insight:** the top 10 emitting states (TX, FL, OH, IL, GA, MO, CA, TN, PA, NC) alone account for **51% of total emissions nationwide**, with Texas leading at 20.6%. At the county level, Maricopa County (AZ) and Harris County (TX) are the top emitters, each at nearly 9.7–9.8 million tons of CO2e.

## 🎯 Project Goals

- Ingest and clean a county-level emissions dataset (3,143 U.S. counties)
- Build exploratory visualizations (map, scatter plot, pie chart, ranking)
- Identify factors correlated with emissions (population, energy consumption, sector activity)
- Publish an interactive dashboard in Databricks

## 🗂️ Data

The [`Emissions_Data_2023.csv`](Emissions_Data_2023.csv) file contains, per county:
- Geographic information (state, county, coordinates)
- Population and employment
- Energy consumption (electricity, natural gas) in MWh / TcF, per capita
- GHG emissions in metric tons of CO2e
- Fuel consumption and vehicle miles traveled
- Number of buildings and area

**Source:** U.S. Environmental Protection Agency (EPA), 2023

## 🛠️ Tech Stack

- **Databricks** (notebooks + dashboard)
- **PSQL** for data processing
- **Databricks Dashboards (Lakeview)** for visualization

## 📁 Repo Structure

```
.
├── README.md
├── Emissions_Data_2023.csv
└── images/
    ├── dashboard_overview.png
    └── dashboard_top_counties.png
```

## 💡 What I Learned

- Getting hands-on with the Databricks environment (notebooks, clusters, dashboards)
- Building geospatial and statistical visualizations from raw data
- Interpreting trends (correlation between population and per-capita emissions)
