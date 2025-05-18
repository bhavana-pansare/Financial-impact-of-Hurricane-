# Potential Financial Impact of Hurricane Ian on KDC Property Insurance

## Overview

This repository addresses the Analytathon 3 Challenge, analyzing the potential financial impact of Hurricane Ian on properties insured by KDC Property Insurance. The analysis includes calculating maximum potential destruction costs and identifying the most significantly impacted geographic areas using property data and hurricane path information.

## Project Objectives

* Calculate maximum inherent cost of property destruction.
* Identify the top 5 most affected ZIP codes by Hurricane Ian.
* Provide strategic insights for improved risk management.

## Data and Preprocessing

* **Property Data**: Property locations, sale prices, market values, and coverage details.
* **Hurricane Path**: Provided by NOAA.
* Filled missing data using Photon geolocator and ZIP code datasets.
* Removed extreme outliers by computing Interquartile Range (IQR).
* Handled duplicates by retaining the most recent entries.
* Conducted spatial joins to integrate hurricane path data with property locations.

## Analytical Approach

* Evaluated property values (highest of market value or sale price).
* Estimated financial exposure for building coverage, contents, and outbuildings.
* Focused on Single-Family Residences and Condominiums in regions with hurricane impact exceeding 60%.

## Exploratory Data Analysis (EDA)

* Visual analysis through log-scaled histograms and box plots for Sale Price and Market Value.
* Correlation heatmap to understand relationships between different property metrics.
* Mapped spatial distribution of high-risk properties.

## Results

* Identified top 5 ZIP codes with the highest hurricane impact, including ZIP codes: 33852, 34293, 33993, 33981, 33914.
* Developed an interactive dashboard visualizing the total financial exposure and geographic concentration of risk.

## Recommendations

* Reassessment of insurance policy coverage limits and premiums in high-risk ZIP codes.
* Property retrofitting initiatives to enhance structural resilience.
* Customer education programs on proactive hurricane preparedness.

## Technologies and Tools

* Python (Geopandas, Pandas)
* Spatial Data Analysis
* Geolocator APIs (Photon)
* Visualization (Matplotlib, Seaborn)
* Interactive Dashboards

## References

* NOAA Hurricane Ian Data
* Bucci et al. (2022). Hurricane Ian Report.
* Hauptman et al. (2024). Journal of Marine Science and Engineering.

---

Detailed methodologies and analyses are provided in notebooks and scripts included in this repository.
