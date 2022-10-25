# Relationship between ENSO and Summer Temperature and Precipitation Anomalies over CONUS 
 
### Loren Doyle
#### CLIM 680 - Fall 2022

## Introduction

I am interested in observing the precipitation and surface temperature reforecast data over the contiguous United States (CONUS), for JJA (June, July, August) 2011-2017 to see if there is a correlation of these variables' anomalies with El Nino and La Nina years in the reforecasts, and to compare that data with neutral years. This is an extension of the research I'm doing with Dr. Stan as part of my GRA.

## Background Information

My GRA project is investigating the prediction of extreme events in precipitation and temperature over CONUS during boreal summer using UFS P7 with Dr. Stan. It is a continuation of the paper "Prediction of extreme events in precipitation and temperature over CONUS during boreal summer in the UFS coupled model" by Krishnamurthy, V; Stan, C. (10.1007/s00382-021-06120-0.)

For this class, I am interested specifically in the JJA data from 2011 to 2017 over CONUS, and exploring whether there is a correlation in anomalies that align with ENSO. The reason I am interested in exploring this correlation is because this is a research area that has been extensively studied, so there are lots of resources to pull information from and compare results with. Furthermore, if summer temperature and precipitation anomalies can become better predicted in general by models like UFS, then including a correlation to ENSO could help predict future ENSO events by following these trends.

Some reference papers I've considered for this project:
* https://link.springer.com/article/10.1007/s00382-021-06120-0 (Prediction of extreme events in precipitation and temperature over CONUS during boreal summer in the UFS coupled model)
* https://hess.copernicus.org/articles/26/4233/2022/ (Quantifying overlapping and differing information of global precipitation for GCM forecasts and El Niño–Southern Oscillation)
* https://www.nature.com/articles/s41612-018-0013-0 (The sub-seasonal to seasonal prediction project (S2S) and the prediction of extreme events)
* https://journals.ametsoc.org/view/journals/mwre/149/9/MWR-D-21-0020.1.xml (Tropical Origins of Weeks 2–4 Forecast Errors during the Northern Hemisphere Cool Season)
* https://ui.adsabs.harvard.edu/abs/2021AGUFM.A43H..01M/abstract (Improving S2S precipitation forecasts in UFS through Tropical Nudging and Explainable Machine Learning)


## Data

The datasets I'm using are:
* UFS Prototype 7 Reforecast data: UFS P7 is one of the experimental versions of the UFS Global Coupled Model (GCM), which contains S2S reforecast data, and includes variables for atmosphere, land, sea ice, and ocean waves. The retrospective runs were from 2011-2018, and initialized on the 1st and 15th of every month (168 forecasts in total), with a forecast length of 35 days and output frequency of 6 hours. The data is on a global grid.
  * The dataset is in the format of netCDF files, and I imported them from COLA. The COLA data was downloaded by Hedanqiu Bai, and was pre-processed for precipitation ['precip'], temperature ['ts'], and 500hPa geopotential height ['z500'] for the corresponding days of each month as hourly steps, then run over a daily mean. https://vlab.noaa.gov/web/ufs-r2o/gcm-prototypes

* NOAA Optimum Interpolation SST v2: NOAA OISST v2 contains monthly means of global SST data which is collected from in situ and satellite observations, as well as simulated SST data from sea-ice cover, and run through an interpolation analysis model (OISST v2). The data was collected from 1981-2020. From 1981-1989 the weeks are centered on Sundays, from 1990-2020 the weeks are centered on Wednesdays. The data is on a global grid.
  * The dataset is in the format of netCDF files, imported from COLA. https://psl.noaa.gov/data/gridded/data.noaa.oisst.v2.html


## Proposed Analysis
I plan to do the following analysis:
* Calculate climatology and anomalies of precipitation and surface temperature over CONUS using P7
* Calculate climatology and anomalies of SST in ENSO regions 
* Construct plots of climatologies and anomalies for all three variables
* Specify years corresponding with El Nino, La Nina, Neutral
* Construct correlation matrix of SST anomalies with P7 variable anomalies
* Calculate significance of features



