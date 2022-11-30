We see from the HA index plot that we have some spikes in activity over time. 

As a general observation, and from the tropical storm and hurricane frequency plot with a climatology from 1851-2017 (Landsea, Chris (contributor from the NHC). "Total and Average Number of Tropical Cylones by Month (1851-2017)". aoml.noaa.gov. National Oceanic and Atmospheric Administration, Atlantic Oceanographic and Meteorological Laboratory. Archived from the original on September 1, 2018.) we see that September is the most active month, with an average of 6 storms, August is the 2nd most active month, with an average of 4 storms, and October is the third most active month, with an average of 3 storms. This is why I have chosen August, September, and October as the months of investigation for my dataset. 

![image](https://user-images.githubusercontent.com/114028135/204910109-f2e0c6c5-269f-4299-a94d-80331f1d51b1.png)

For August, September, and October, the composite I am making is looking at the 3 largest and 3 smallest valued years for HAI for each month. To do this, I need to find the month with the most storms and the month with the least storms for each year. I ended up doing this by hand.

August: 6.25=2011, 6=2012, 0=2013, 4.25=2014, 3.5=2015, 6=2016

September: 12.25=2011, 13.37=2012, 3.25=2013, 4.5=2014, 1=2015, 3.5=2016

October: 7.5=2011, 8=2012, 0=2013, 6.75=2014, 6.5=2015, 15.5=2016

For August: 
* 3 largest years: 2011, 2012, 2016
* 3 smallest years: 2013, 2014, 2015

For September:
* 3 largest years: 2012, 2011, 2014
* 3 smallest years: 2015, 2013, 2016

For October: 
* 3 largest years: 2016, 2012, 2011
* 3 smallest years: 2013, 2014, 2015

Interestingly, August and October match up in terms of years.

# HA Composites
## High HA
![ts_high_ha_comp](https://user-images.githubusercontent.com/114028135/204893522-8f4d5d1a-dc32-423b-a7f7-24f452967b1c.png)
![precip_high_ha_comp](https://user-images.githubusercontent.com/114028135/204904559-33332cb9-9030-4ef8-aaf8-0396e3a981a7.png)
![z500_high_ha_comp](https://user-images.githubusercontent.com/114028135/204906386-78b00acc-3f83-41eb-a0fa-c1eaf9edd65e.png)

## Low HA
![ts_low_ha_comp](https://user-images.githubusercontent.com/114028135/204893537-9f5b43f7-c1fa-4d2f-b7c8-dbad2665a746.png)
![precip_low_ha_comp](https://user-images.githubusercontent.com/114028135/204904564-8b7066c0-5ca8-4e2b-8b80-11b55fd6b001.png)
![z500_low_ha_comp](https://user-images.githubusercontent.com/114028135/204906393-9ea8e7bc-f44e-4479-8660-3d1c301dd239.png)

# Observations:
Hurricanes favor warm water, and high relative humidity, and are low pressure systems. So, high anomalies in surface temperature and precipitation, and low anomalies in z500 can indicate conditions favorable for hurricane/tropical cyclone formation/places where tropical storms can migrate to (a big reason why many hurricanes have trajectories through warmer tropical/subtropical waters like the Caribbean Sea and the Gulf of Mexico). 

Using the composites from the alternative averaging method, we can make some observations:

Based on the surface temperature anomalies corresponding with high hurricane activity, we see that for August, the water was actually a little bit cooler than average, but September and October both had higher than average surface temperatures in the water. Since, we have more tropical cyclone activity in September and October, these composites make sense.

Based on the surface temperature anomalies corresponding with low hurricane activity, we that for August the water was warmer than average, but so was the land. For September, we see that the water was cooler than average around the tip of Florida, but was warmer in the higher latitudes of the subtropics. And for October, we see that the water did not really change beyond the average, meanwhile the land was warmer than average. 

Based on the precipitation anomalies corresponding with high hurricane activity, we see that for August, there was higher than average precipitation over Louisiana, mostly average precipitation throughout the majority of the Gulf and Atlantic, with places of below average precipitation over Florida and the Carolinas. For September, we see higher than average precipitation over Louisiana and parts of Florida, while the rest of the map shows average or below average precipitation. For October, we actually see below average precipitation over the majority of the Southeast region, with average precipitation over Florida.

Based on the precipitation anomalies corresponding with low hurricane activity, we see that for August it was mostly average and above average precipitation during the corresponding months. For September, it was mostly average, with locations of below average precipitation over Louisiana, Alabama, with high precipitation around the Bahamas. For October, it was mostly average if not slightly below average, with locations of below average precipitation around Cuba, and the Bahamas, and higher precipitation over the continent. 

Based on the z500 geopotential height anomalies corresponding with high hurricane activity, we see that for August, the height contours were lower in the atmosphere over Florida and into the water and higher over the continent, which could indicate storm activity in the Caribbean. For September, the anomalies have a very distinct shape that could indicate locations of low pressure around Louisiana, the Bahamas, and North Carolina, meaning that those are regions indicating storms. For October, the low z500 anomalies are up near the midlatitudes.

Based on the z500 anomalies corresponding with low hurricane activity, we see that for August, the low height anomalies were more over the continent, and the higher height anomalies were over the gulf. And since we know these are anomalies for low hurricane activity months, this makes sense. For September, all the height anomalies are positive, with the highest being out in the Atlantic. For October, again, all the height anomalies are positive, with the highest being in the mid latitudes over the continent. 
