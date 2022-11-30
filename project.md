# Is the UFS Reforecast data useful for reforecasting hurricanes?
# Introduction:


# Data: What Are We Working With?

## Gridded Data:
### UFS Plots with the corresponding tropical cyclones
[contours](contours.md)
### Tropical Cyclone Maximum Sustained Wind Speeds and Minimum Central Pressures
[hurricane_vars](hurricane_vars.md)

## Indices:
### Hurricane Activity Index
![haindex](https://user-images.githubusercontent.com/114028135/204729604-3605aa33-07fd-48a1-ba20-5364f88e8c75.png)

### Accumulated Cyclone Energy Index
![aceindex](https://user-images.githubusercontent.com/114028135/204729725-6632743c-ef81-4870-ada5-bf0d35b8018e.png)

### Tropical North Atlantic Index
![tnaindex](https://user-images.githubusercontent.com/114028135/204729760-f11dcccf-7e06-4f88-a491-77006e4f0c1f.png)




# Analysis Approach: 
## What Do We Want to Know: Is the UFS Reforecast data useful for reforecasting hurricanes?
## How Do We Want to Investigate This:
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

# Climatology:
## Yearly:
![ts_yearly_clim](https://user-images.githubusercontent.com/114028135/204731700-4dc3bc30-eb5a-4c37-a5e6-648fbe26c950.png)
## Monthly:
![ts_monthly_clim](https://user-images.githubusercontent.com/114028135/204732370-37e2a6ea-aaa1-49d3-974a-32958ef591d4.png)


# Results: What Did We Find?

# Summary: What Did We Learn?

# Conda Environment

# References
