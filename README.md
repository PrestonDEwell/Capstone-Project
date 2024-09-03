# Predictive Analytics for Energy Capacity and Supply Mismatches in Puerto Rico

## Overview
This project applies predictive analytics to forecast energy capacity and supply mismatches in Puerto Rico's energy grid under stress conditions. The analysis aims to enhance the accuracy of forecasting to improve planning and emergency response during high-stress events. The project uses time series data and grid performance capacity metrics to achieve these goals.

## Problem Statement
Puerto Rico’s energy grid often faces significant challenges during high-stress events, leading to mismatches in energy supply and capacity. The hypothesis driving this project is that predictive analytics, specifically using ARIMA models, can improve the accuracy of forecasting these mismatches, thereby aiding in better planning and emergency responses.

## Data Analysis Process
The analysis involved two primary datasets:

- Predicted hourly energy generation for various technologies over one year.
- Energy generation capacities under different scenarios.

### Steps:
1. **Data Preparation:** Used Pandas for data extraction, preparation, and manipulation. Standardized column names and resampled data to daily frequencies.
2. **Mismatch Calculation:** Calculated the energy supply and capacity mismatch for each energy type.
3. **Data Merging:** Merged the dataframes on technology type to create a comprehensive dataset with daily energy and supply mismatch data for 9 technology types.
4. **Forecasting:** Applied the ARIMA model to forecast future mismatches.

## Key Findings
- Significant mismatches were identified for technologies such as Utility Photovoltaics, Distributed Photovoltaics, and Diesel.
- The ARIMA model provided effective forecasts for future mismatches, offering valuable insights for infrastructure development and energy resource adjustments.

## Limitations
- **Scalability:** The tools used, such as Pandas and ARIMA, may struggle with very large datasets.
- **Data Scope:** The analysis was limited to one year of data, which was based on predictive models rather than real-world observations.

## Proposed Actions
- Use the analysis results for future infrastructure planning, especially in distributing generated energy more effectively.
- Consider implementing commensurate battery storage and other responsive energy resources to smooth out forecasted mismatches.

## Expected Benefits
- Improved reliability of Puerto Rico’s power grid during stress conditions.
- Potential reduction in operational costs associated with emergency energy distribution by 10-20% through proactive infrastructure upgrades and battery storage integration.

## Installation
To run this project, you will need:

- Python 3.x
- Pandas
- ARIMA model (part of the statsmodels library)
