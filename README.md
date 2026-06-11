# Multilateral Fund Project Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Vega](https://img.shields.io/badge/Vega--Lite-1F77B4?style=for-the-badge)
![ArcGIS](https://img.shields.io/badge/ArcGIS-2C7AC3?style=for-the-badge&logo=esri&logoColor=white)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## Overview

An interactive Power BI dashboard visualizing the impact of the 
[Multilateral Fund for the Implementation of the Montreal Protocol (MLF)](https://www.multilateralfund.org/), a financial mechanism supporting developing countries in phasing out ozone-depleting substances and high global warming potential chemicals under the Montreal Protocol and Kigali Amendment.

Built as a personal project to explore the fund's $4.3B+ in approved financing across 140+ countries from 1990 to present.


## Why I built it
I have been working at the MLF Secretariat for about two years, and my role includes several data management and analysis tasks. My interest in data visualization and science communication led me to take the fund's publicly available progress report, a static excel file, and turn it into something that lets a general audience feel the scale of what the Montreal Protocol has achieved.


## Preview
<img width="2065" height="1149" alt="MLF Dashboard gif2" src="https://github.com/user-attachments/assets/27bf4377-c0c9-4bb7-9743-99ecc67c2df8" />


## Features

- **Interactive choropleth map**: ArcGIS visual used to explore project coverage and intensity by country or region. Users can click directly on the map to filter the page, or use the slicers on the left to break down the data. 
- **Custom tooltip**: hover any country to see disbursement progress, phase-out progress, and latest multi-year project approved. 
- **Drill-through Projects page**: country-level project list, agency breakdown, project type breakdown, and cumulative phaseout chart. Users can apply necessary filters, and select the image of the globe/country to drill through to a more detailed project page. 
- **Custom Deneb/Vega visuals** : project list cards and KPI summary bar built with Vega spec.
- **Dynamic unit toggle**: switch between ozone depleting potential (ODP) tonnes and CO2-equivalent tonnes across all relevant visuals.
- **Active filters display**:  shows currently applied agency/period/type filters at a glance.
- **Cumulative phaseout chart**: dual-axis area chart showing ODP and CO2-eq phaseout from 1990 to present. 

## Data source
This dashboard was built using data sourced from the Multilateral Fund Secretariat consolidated progress report (Document UNEP/OzL.Pro/ExCom/97/11), publicly available at https://www.multilateralfund.org/.

## Data enhancements
Before building the dashboard, I enhanced the data in a few ways: 

- Created a lookup table mapping countries to latitude/longitude coordinates and flag image URLs, enabling the choropleth map and flag display throughout the dashboard. 
- Added columns aggregating certain variables such as budget and expenditures for easy use in visuals.
- Cleaned and restructured data to ensure compatibility with Power BI's data model and enable efficient processing across visuals.
- Applied additional transformations including field categorization, custom sort ordering, and column renaming for consistency across visuals.


## Pages
### Overview
Regional/country-level summary with interactive map, KPI cards, and slicers for region, country, period, and attributes.

### Project Details
Country-level drill-through showing full project list, agency and type breakdowns, and cumulative phaseout time series.


## Technical Stack

| Tool | Usage |
|---|---|
| Power BI Desktop | Report development |
| Deneb (Vega) | Custom project list and KPI bar visuals |
| ArcGIS Maps for Power BI | Choropleth map visual |
| DAX | Measures for KPIs, tooltips, dynamic labels |
| ChicletSlicer | Unit toggle (ODPt / CO2eqt) |

## Repository Structure


