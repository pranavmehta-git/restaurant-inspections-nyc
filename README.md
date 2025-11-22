# NYC Restaurant Inspection Equity Analysis

This project investigates whether restaurant inspection intensity varies across income levels in New York City census tracts. Using DOHMH inspection data (2019–2023) merged with American Community Survey (ACS) socioeconomic indicators, the analysis explores whether low-income neighborhoods receive disproportionately more inspections per square mile or per capita.

## 📂 Repository Structure

nyc-restaurant-inspection-equity/
├── analysis.Rmd              # Full reproducible analysis
├── scripts/                  # Data prep & helper scripts
├── data/                     # Raw and cleaned datasets
├── figures/                  # Maps, plots, statistical visuals
└── results/                  # Regression output & tables

## 📊 Research Questions

1) Do low-income census tracts receive more frequent restaurant inspections?

2) Is inspection intensity correlated with:

- Median household income
- Poverty rates
- Racial/ethnic composition
- Population density?

3) What geographic patterns emerge when comparing inspection density per square mile?

## 🔧 Methods & Data

### Data Sources

- NYC DOHMH Restaurant Inspection Data (2019–2023)
  *Publicly available via NYC Open Data.*
- American Community Survey (ACS) 2021 5-year estimates
  *via tidycensus.*

### Key Variables

#### Outcome:

- Inspections per 1,000 residents

#### Explanatory:

- Median household income
- Poverty rate
- Race/ethnicity shares
- % foreign-born
- Population density

#### Statistical Methods

- Exploratory data analysis
- Spatial joins with census tract polygons
- OLS regression with controls

Geospatial visualization (sf, ggplot2)
