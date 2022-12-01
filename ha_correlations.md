We want to know if there is any significant correlation between hurricane activity and the UFS data.

For reference:

red =  variable increases with increase in hurricane activity, and decreases when hurricane activity decreases.

blue = variable increases with decrease in hurricane activity, and decreases when hurricane activity increases.

near zero means no relationship with the 2.

Hashmarks indicate statistical significance.

# Correlation Between HA and TS:
![cor_ha_ts_anoms](https://user-images.githubusercontent.com/114028135/204928701-f2f1de0c-f841-4639-bb93-2ac7b915e7bc.png)

From the plot, we can see that surface temperature does not appear to have a significant correlation with hurricane activity. There are some spots of slight correlation, but not enough to be significant.

# Correlation Between HA and Precip:
![cor_ha_precip_anoms](https://user-images.githubusercontent.com/114028135/204928666-c8bb68e4-2dd9-496b-8626-e8c215b8391d.png)

There appears to be some significant positive correlation between hurricane activity and precipitation (at the bottom of the grib between 90W and 85W), and significant negative correlation between hurricane activity and precipitation near Kentucky (very specific). This means that in Kentucky, when hurricane activity increases, precipitation will decrease, and if the activity decreases, precipitation will increase. 

# Correlation Between HA and z500:
![cor_ha_z500_anoms](https://user-images.githubusercontent.com/114028135/204928780-86ad1ba6-a18a-44a7-a285-e685e52d42b1.png)

For z500, there appears to be some negative correlation between the 500hPa height contours and hurricane activity, which makes sense, because as hurricane activity increases, there should be a decrease in the height contours, and vice versa. This is because hurricanes are cyclonic, low pressure systems, so we should expect the height contours to dip down in height. There is not a positive correlation, which is also expected. 


Obviously, we know logically that there is a correlation between hurricane activity and surface temperature, specifically that higher SSTs drive hurricanes. This means that there's most likely something wrong with how I calculated my anomalies. It could also be due to the fact that I am working with reforecast data, and so the farther away the day is from the initialization, the less accurate it will be. 

I also expected a higher correlation with precipitation than I got, which could be due to the same things as previously mentioned. 
