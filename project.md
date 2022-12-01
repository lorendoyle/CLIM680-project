# Is the UFS Reforecast data useful for reforecasting hurricanes?
# Introduction:
In this project, I used a few different datasets and indices to determine (to an extent) if UFS reforecast data initialized on the first of every month was useful in reforecasting tropical cyclones in a specific region in the Atlantic for the 3 most active hurricane months in a 5 year period. 

I'm interested in this because tropical cyclones, including depressions and storms, bring intense precipitation and winds which are damaging to many tropical and subtropical regions along the western boundary of the Atlantic, and as the planet's temperatures continue to rise, so do the sea surface temperatures (which are the main energy source of tropical cyclones), leading to more intense and unpredictable hurricane seasons each year. If the model is able to reforecast these events, then future forecasting could better predict when and where tropical cyclones can occur and migrate to, and can help minimize - and prevent - damages. 

I used the following data in my exploration:
* Data from UFS P7: precipitation, surface temperature, and 500 hPa geopotential height daily data for August, September, October from 2011 to 2016, within the region from 95W to 72W and 23N 37N. This region covers part of the Southeast US, part of the Gulf of Mexico, and part of the Atlantic, which is where many tropical cyclones migrate to, so my reasoning was that this region would give me small enough datasets without overloading my storage while allowing me access to a relatively active hurricane region. 
* Data from International Best Track Archive: hurricane tracks, wind speeds, and pressures for tropical cyclones within the lat/long bounds of UFS data during the specified months and years. 
* Data from Physical Sciences Laboratory: Hurricane Activity Index = monthly total of storms per month per year, Accumulated Cyclone Energy Index = monthly total of cyclone energy per month per year, Tropical North Atlantic Index = monthly SST anomalies in degrees celsius. 
Sources linked in [data_sources](data_sources.md)

# Analysis Approach: 
* calculate climatology by month/year 
* calculate anomalies
* use HA index to determine highest months of TC activity
    * HA composites
* use ACE index to determine months of strongest TCs
    * ACE composites    
* use TNA index to determine correspondence of high SST anomalies with anomalies of UFS variables
    * TNA composites
* correlations and comparison plots with statistical significance
    * HA, ACE, TNA correlations
* linear regression

# Visualization of Initial Data: 

## Gridded Data:
### UFS Plots with the Corresponding Tropical Cyclones
[contours](contours.md)
### Tropical Cyclone Maximum Sustained Wind Speeds and Minimum Central Pressures
[hurricane_vars](hurricane_vars.md)

## Indices:
### Hurricane Activity Index
![haindex](https://user-images.githubusercontent.com/114028135/204729604-3605aa33-07fd-48a1-ba20-5364f88e8c75.png)

The Hurricane Acitivity Index (HA) is the total number of named tropical cyclones per month. 

### Accumulated Cyclone Energy Index
![aceindex](https://user-images.githubusercontent.com/114028135/204729725-6632743c-ef81-4870-ada5-bf0d35b8018e.png)

The Accumulated Cyclone Energy Index (ACE) of a season is the sum of the squares of every tropical cyclone with wind speeds of 35 kts (65 km/h) or higher every 6 hours. 1 ACE = 10^4 kts^2. If an ACE index for a season is above 159.6 It is extremely active, if it 73-126.1 it is near-normal, and below 73 is below normal. ACE indices can be calculated for individual cyclones, as well as a monthly total, which is what I am working with. 

### Tropical North Atlantic Index
![tnaindex](https://user-images.githubusercontent.com/114028135/204729760-f11dcccf-7e06-4f88-a491-77006e4f0c1f.png)

The Tropical North Atlantic SST Anomaly Index (TNA) is calculated in the TNA region of 55W-15W, 5N-25N.


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
So, is UFS reforecast data useful in reforecasting hurricanes? Not particularly. My approach was relatively informal and did not take into account the hurricane track data. I considered using it, but the time coordinate was tricky to parse out, and I did not have the time. The errors (perhaps lost data?) when aggregating the data from it's daily resample to a monthly resample and the nature of reforecast data being less accurate the farther you are from the initialization of the forecast could be contributing factors as to why the significance testing did not meet expectations/theory, why only some tropical cyclones match up with the UFS data directly, and why the complications with the complications with the composites exist.

In the future, I would include the data initialized on the 15th (in addition to the initialization on the 1st), use an observation dataset to compare the reforecast data to, and do a temporal correlation instead of a linear regression. I would also like to incorporate the hurricane tracks, wind speeds, and central pressures in analysis to get a full scope of the reforecast's capabilities. Another thing I would like to do is perform my climatology with an observation dataset, or even just more years from the UFS reforecast data. Having only 6 years worth of data makes the climatology and therefore the anomalies a bit skewed at best and meaningless at worst.

# Conda Environment

Need to insert the yml file thingy thing

# References

make this look nice later

https://web.archive.org/web/20180901052811/http://www.aoml.noaa.gov/hrd/tcfaq/E17.html

https://www.epa.gov/climate-indicators/climate-change-indicators-tropical-cyclone-activity#tab-4

https://www.nhc.noaa.gov/verification/

https://www.nhc.noaa.gov/data/#tcr

https://climateimpactcompany.com/tropical-feature-the-warm-tropical-north-atlantic-index-2/

https://nca2009.globalchange.gov/national-climate-change/index.html

https://rmets.onlinelibrary.wiley.com/doi/full/10.1002/met.1456

atmo.arizona.edu introduction to 500 mb height maps
