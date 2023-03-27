# DanishCrown_export_analysis

This repository contains data and analysis of trends in pigs exports over time for Danish Crown. The data used in this analysis is sourced from all_exports.csv, data given by Danish Crown.
# Data

all_exports.csv contains information about the number of pigs exported from Denmark to different countries. The data spans from June 2012 to November 2022.The data was cleaned by removing any missing or duplicate values, and the date column was parsed as a datetime object.
# Analysis

The analysis was performed using Python, with the following libraries:

- pandas
- numpy
- matplotlib
- statsmodels

First, the data was resampled to a monthly frequency and aggregated by summing the number of animals exported in each month. A time series plot of the data was then created to visualize the trends in pig exports over time. It was observed that the trend appeared to be relatively stable over time, with some seasonality.

Next, an ARIMA model was trained to forecast future trends in pig exports. The data was first reindexed to include future periods up to 4 years in the future. The ARIMA model was then trained on the resampled monthly data, with an order of (1, 1, 0). The model was used to forecast future trends in pig exports, and the results were plotted alongside the historical data.

# Results

- The average number of animals on each transport is: 398.8699634339482.
- From 2012 to 2022 the trendline has a stable growth.
- The top 5 countries where Danish Crown exported are: 
(Country)(Total nr. of animals exported)
1. DE    65611156
2. PL    54813954
3. IT     8392032
4. RO     1644849
5. HR     1440901
 
The analysis revealed that the number of pigs exported per month appeared to be relatively stable over time, with some seasonality. The ARIMA model forecasted that this trend is expected to continue in the future.

# Conclusion

In conclusion, the analysis suggests that pig exports from Denmark have been relatively stable over time, with some seasonality. The ARIMA model forecasted that this trend is expected to continue in the future. Further analysis could be performed to investigate the drivers of seasonality and any potential changes in the future.
