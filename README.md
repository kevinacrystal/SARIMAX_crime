# Project 6: NYPD Crime Analysis and Prediction

## Problem Statement

This project aims to explore the incidence of crime in New York City and attempt to predict the incidence of future crime using correlated features and time series models.

## Executive Summary
### Methodology:
Crime data was collected from NYC Open Data's [NYPD Complaint Data Historic dataset](https://data.cityofnewyork.us/Public-Safety/NYPD-Complaint-Data-Historic/qgea-i56i). Weather data was collected from NOAA's [Daily Summaries Station Details for Central Park, NY](https://www.ncdc.noaa.gov/cdo-web/datasets/GHCND/stations/GHCND:USW00094728/detail).

The data was cleaned and merged, and predictive modeling was done using ARIMA, SARIMA, and SARIMAX models. SARIMAX was modeled using maximum daily temperature as an exogenous feature. Each model was subjected to a grid search to determine optimal parameters.


### Contents:
- [01_EDA_and_Cleaning](https://github.com/kevinacrystal/SARIMAX_crime/blob/master/01_Cleaning_and_EDA.ipynb)
- [02_Modeling](https://github.com/kevinacrystal/SARIMAX_crime/blob/master/02_Modeling.ipynb)
- [03_Mapping](https://github.com/kevinacrystal/SARIMAX_crime/blob/master/03_Choropleth_Maps.ipynb)

## Conclusions and Recommendations

Using maximum temperature improved the predictive ability of the SARIMAX model. By using an exogenous feature such as maximum temperature, which can be more accurately predicted than crime itself, it may be possible to improve predictions of crime incidence.
