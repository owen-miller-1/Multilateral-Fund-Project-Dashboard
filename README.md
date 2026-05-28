# Multilateral Fund Project Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Vega](https://img.shields.io/badge/Vega--Lite-1F77B4?style=for-the-badge)
![ArcGIS](https://img.shields.io/badge/ArcGIS-2C7AC3?style=for-the-badge&logo=esri&logoColor=white)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## Overview

An interactive Power BI dashboard visualizing the impact of the 
[Multilateral Fund for the Implementation of the Montreal Protocol (MLF)](https://www.multilateralfund.org/) — 
a financial mechanism supporting developing countries in phasing out 
ozone-depleting substances and high global warming potential chemicals 
under the Montreal Protocol and Kigali Amendment.

Built as a side project to explore the fund's $4.3B+ in approved 
financing across 140+ countries from 1990 to present.

---

## Preview

<img width="2419" height="1363" alt="Screenshot 2026-05-26 105300" src="https://github.com/user-attachments/assets/444aac04-65dc-452b-8cc8-36dbf65ea388" />
<img width="2425" height="1355" alt="Screenshot 2026-05-26 110704" src="https://github.com/user-attachments/assets/18af6be9-5e8f-47ea-8d9c-486466fad394" />
<img width="2417" height="1354" alt="Screenshot 2026-05-26 105738" src="https://github.com/user-attachments/assets/c5a1d1f9-c90b-48c0-9216-3cfb3af2eba7" />


---

## Features

- **Interactive choropleth map** (ArcGIS) — explore project 
  coverage and intensity by country or region
- **Custom tooltip** — hover any country to see disbursement 
  progress, phase-out progress, and latest multi-year project
- **Drill-through Projects page** — country-level project list, 
  agency breakdown, project type breakdown, and cumulative 
  phaseout chart
- **Custom Deneb/Vega visuals** — project list cards and KPI 
  summary bar built with Vega spec
- **Dynamic unit toggle** — switch between ODP-tonnes and 
  CO2-eq tonnes across all relevant visuals
- **Active filters display** — shows currently applied 
  agency/period/type filters at a glance
- **Cumulative phaseout chart** — dual-axis area chart showing 
  ODP and CO2-eq phaseout from 1990 to present

---

## Pages

### Overview
Regional/country-level summary with interactive map, KPI cards, 
and slicers for region, country, period, and attributes.

### Project Details
Country-level drill-through showing full project list, agency 
and type breakdowns, and cumulative phaseout time series.

---

## Technical Stack

| Tool | Usage |
|---|---|
| Power BI Desktop | Report development |
| Deneb (Vega) | Custom project list and KPI bar visuals |
| ArcGIS Maps for Power BI | Choropleth map visual |
| DAX | Measures for KPIs, tooltips, dynamic labels |
| ChicletSlicer | Unit toggle (ODPt / CO2eqt) |

---

## Repository Structure
