# CLIM 680 Project: Is the UFS Reforecast data useful for reforecasting hurricanes?



# Data: What Are We Working With?

## Gridded Data:
### UFS Plots with the corresponding tropical cyclones
![emily_contours](https://user-images.githubusercontent.com/114028135/204725380-9529aa34-eebf-480f-8141-880513438416.png)
![irene_contours](https://user-images.githubusercontent.com/114028135/204725436-8b3fd0e1-8d85-4185-adfd-bd6bcad5b04e.png)
![lee_contours](https://user-images.githubusercontent.com/114028135/204725441-65c1ac11-8621-4335-9f2f-6abf662c010d.png)


### Tropical Cyclone Maximum Sustained Wind Speeds
![2011_wind_speeds](https://user-images.githubusercontent.com/114028135/204839154-95fcc6c1-1aa9-41ec-a1d6-469036e83105.png)
![2012_wind_no_patty](https://user-images.githubusercontent.com/114028135/204844043-e89c1f3a-a090-4504-b22f-d07b3ca62aa8.png)
![2013_wind](https://user-images.githubusercontent.com/114028135/204839266-32b9366c-9ea7-4615-939d-d5493658a56a.png)
![2014_wind](https://user-images.githubusercontent.com/114028135/204839285-afa7e371-989d-45ad-8f66-0d49f35fd172.png)
![2015_wind](https://user-images.githubusercontent.com/114028135/204839303-e2b681b5-b612-4899-99da-51b2aad5c4cb.png)
![2016_wind](https://user-images.githubusercontent.com/114028135/204839317-d3b3d7dc-7f84-453e-9fcd-990272c24850.png)

### Tropical Cyclone Minimum Central Pressure
![2011_pres](https://user-images.githubusercontent.com/114028135/204839635-34420d02-2308-4ea9-a24f-e58d642751a6.png)
![2012_pres_no_patty](https://user-images.githubusercontent.com/114028135/204843843-67988a9c-2d36-4c06-b8a1-cf8de1f5ac6b.png)
![2013_pres](https://user-images.githubusercontent.com/114028135/204839654-aef5f47c-71ae-4bb6-9434-98d1cddedb99.png)
![2014_pres](https://user-images.githubusercontent.com/114028135/204839668-d56103b0-3191-4a56-805d-4771fafc0431.png)
![2015_pres](https://user-images.githubusercontent.com/114028135/204839679-0290ec7f-7e65-41bf-b84a-a7ae21625cdc.png)
![2016_pres](https://user-images.githubusercontent.com/114028135/204839690-3efe377b-c550-4fe6-94ab-7e577c3b87f6.png)




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
