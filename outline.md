# Relationship between ENSO and Temperature and Precipitation Anomalies over CONUS 
 
### Loren Doyle
#### CLIM 680 - Fall 2022

## Introduction

I am using UFS Prototype 7 reforecast data for Precipitation and Temperature over the contiguous United States 
(CONUS), initialized July 1st 2011-2017 to see if there is a correlation between midsummer precipitation and temperature 
anomalies with El Nino and La Nina years in the reforecasts, and to compare that data with neutral years. 

## Data

UFS P7 is one of the experimental versions of the UFS Global Coupled Model (GCM), which contains S2S reforecast data, and 
includes variables for atmosphere, land, sea ice, and ocean waves. The retrospective runs were from 2011-2018, and initialized 
on the 1st and 15th of every month (168 forecasts in total), with a forecast length of 35 days and output frequency of 6 hours. 
The dataset is in the format of netCDF files, and I imported them from COLA. The COLA data was downloaded by Hedanqiu Bai, 
and was pre-processed for precipitation ['precip'], temperature ['ts'], and 500hPa geopotential height ['z500'] for the corresponding 
days of each month as hourly steps, instead of the 35 day forecasts.

    https://vlab.noaa.gov/web/ufs-r2o/gcm-prototypes


## Proposed Analysis
I plan to do the following analysis:
* Calculate climatology and anomalies of precipitation and surface temperature
*
### Functions
I will create a set of functions in `clim_utils.py` for doing common tasks used throughout my analysis, including:
* Labelling plots
* calculating climatology and anomalies
* etc.

### Conda Environment

The environment.yml file is provided to define the environment needed to run all codes.
