# Is the UFS Reforecast data useful for reforecasting hurricanes?
# Introduction:
In this project, I used a few different datasets and indices to determine if UFS reforecast data initialized on the first of every month was useful in reforecasting tropical cyclones in a specific region in the Atlantic for the 3 most active hurricane months in a 5 year period. 

I'm interested in this because tropical cyclones, including depressions and storms, bring intense precipitation and winds which are damaging to many tropical and subtropical regions along the western boundary of the Atlantic, and as the planet's temperatures continue to rise, so do the sea surface temperatures (which are the main energy source of tropical cyclones), leading to more intense and unpredictable hurricane seasons each year. If the model is able to reforecast these events, then future forecasting could better predict when and where tropical cyclones can occur and migrate to, and can help minimize - and prevent - damages. 

I used the following data in my exploration:
* Data from UFS: precipitation, surface temperature, and 500 hPa geopotential height daily data for August, September, October from 2011 to 2016. 
* Data from International Best Track Archive: hurricane tracks, wind speeds, and pressures for tropical cyclones within the lat/long bounds of UFS data during the specified months and years. 
* Data from Physical Sciences Laboratory: Hurricane Activity Index = monthly total of storms per month per year, Accumulated Cyclone Energy Index = monthly total of cyclone energy per month per year, Tropical North Atlantic Index = monthly SST anomalies in degrees celsius. 

# Analysis Approach: 
* calculate climatology by month/year 
    * for year climatology, looking for trends in increase/decrease in variables over the years   (expecting ts to warm up over time, more intense precipitation and z500 etc)
* calculate anomalies
* use HA index to determine highest months of TC activity
    * HA composites
* use ACE index to determine months of strongest TCs
    * ACE composites    
* use TNA index to determine correspondence of SST anomalies with TCs (like, the actual TC data, do composites of that with TNA index) (maybe? TC data is 3 hourly, but TNA is monthly)
    * TNA composites
* use TNA index to determine correspondence of SST anomalies with precipitation anomalies, z500 anomalies, and ts anomalies
    * TNA composites
* correlations and comparison plots with statistical significance
    * HA, ACE, TNA correlations
* linear regression
* temporal correlation coefficient (maybe?)
* see if the later reforecasts are less accurate (visual comparisons, correlations, etc) (maybe?)
* compare the tropical cyclone pressures to the UFS z500 levels (maybe?)

# Visualization of Initial Data: 

## Gridded Data:
### UFS Plots with the Corresponding Tropical Cyclones
[contours](contours.md)
### Tropical Cyclone Maximum Sustained Wind Speeds and Minimum Central Pressures
[hurricane_vars](hurricane_vars.md)

## Indices:
### Hurricane Activity Index
![haindex](https://user-images.githubusercontent.com/114028135/204729604-3605aa33-07fd-48a1-ba20-5364f88e8c75.png)


To do this, I need to find the month with the most storms and the month with the least storms for each year. 
### Accumulated Cyclone Energy Index
![aceindex](https://user-images.githubusercontent.com/114028135/204729725-6632743c-ef81-4870-ada5-bf0d35b8018e.png)
### Tropical North Atlantic Index
![tnaindex](https://user-images.githubusercontent.com/114028135/204729760-f11dcccf-7e06-4f88-a491-77006e4f0c1f.png)


# Climatology and Anomalies
[clims_anoms](clims_anoms.md)

# Composites:
## Hurricane Activity Composites
[ha_composites](ha_composites.md)
## Accumulated Cyclone Energy Composites
[ace_composites](ace_composites.md)
## TNA Composites
[tna_composites](tna_composites.md)
# Correlations:
## HA Correlation
[ha_correlations](ha_correlations.md)
## ACE Correlation
[ace_correlations](ace_correlations.md)
## TNA Correlation
[tna_correlations](tna_correlations.md)

# Linear Regression:
[linear_regression](linear_regression.md)

# Summary: What Did We Learn?

# Conda Environment

# References
