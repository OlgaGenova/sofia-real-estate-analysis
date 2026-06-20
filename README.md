# Sofia Residential Real Estate Market Analysis

## Project Overview

This project analyzes Sofia's residential real estate market using apartment sale and rental listings, statistical methods, geospatial analysis, and mortgage scenario modeling.

The market data reflects publicly available listings as of June 2026.

## Reports

* [View Real Estate Market Analysis PDF report (ENG)](reports/imot_analysis_eng.pdf)
* [View Real Estate Market Analysis PDF report (RUS)](reports/imot_analysis_rus.pdf)

## Objective

The main objective is to assess the investment attractiveness of residential real estate across Sofia and answer the following questions:

* Which districts have the highest and lowest median prices per square meter?
* Which districts offer the highest gross rental yields?
* How do construction period and number of rooms affect relative property value?
* Which apartment types are more attractive for buy-to-let investment?
* How does housing affordability differ across districts?
* Can rental income cover mortgage payments under a standardized financing scenario?

## Code and Project Files

| File                                               | Description                                                                                                                                                          |
| -------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [`imot_analysis_v1.ipynb`](imot_analysis_v1.ipynb) | Main analytical notebook containing data preparation, exploratory analysis, statistical testing, visualizations, investment metrics, and mortgage scenario analysis. |
| [`geo_api_getting.ipynb`](geo_api_getting.ipynb)   | Geospatial data preparation using OpenStreetMap and the Overpass API. The resulting district geometries are used in the main analysis to build maps of Sofia.        |
| [`svg/`](svg/)                                     | Charts and maps used in the analytical notebook and final reports.                                                                                                   |


## Project Workflow

1. Collection of publicly available apartment sale and rental listings.
2. Data cleaning, type conversion, and feature engineering.
3. Calculation of sale and rental price per square meter.
4. Preparation and matching of Sofia district geometries using OpenStreetMap and the Overpass API.
5. Exploratory data analysis and visualization.
6. Statistical comparison of construction periods and apartment types.
7. Calculation of district-level rental yield and housing affordability.
8. Mortgage payment, coverage score, and monthly cash-flow modeling.
9. Business interpretation and preparation of the final reports.

## Key Findings

* Sofia's residential real estate market differs substantially across districts.
* Old housing stock has a higher relative value than transitional properties and new developments in the analyzed dataset.
* One-room and two-room apartments are the most attractive segment by gross rental yield.
* Some affordable districts offer stronger rental yields than premium central locations.
* Rental yield alone is not sufficient for evaluating investment attractiveness; mortgage payments and monthly cash flow should also be considered.

## Statistical Approach

The project combines exploratory data analysis with statistical testing. Because price-per-square-meter distributions were non-normal, medians and non-parametric methods were used for group comparisons.

## Data Sources

* Publicly available apartment sale and rental listings from [imot.bg](https://www.imot.bg/).
* Average salary data from Bulgaria's National Statistical Institute.
* Sofia district geometries from OpenStreetMap through the Overpass API.

## Data and Code Availability

The scraping code and collected CSV files are not publicly included in this repository. They can be provided upon request for technical review.


## Technologies

Python, pandas, NumPy, SciPy, statsmodels, scikit-posthocs, Matplotlib, Seaborn, GeoPandas, Jupyter Notebook, GeoJSON, OpenStreetMap, Overpass API, geojson.io.
::: 
