Similar to how I determined the composites for hurricane activity, I did the same with ACE, pulling the years of highest ACE and lowest ACE and doing a composite of anomalies of precipitation, z500, and temperature corresponding to the highest and lowest ACE years.

![ace_ts_high_comp](https://user-images.githubusercontent.com/114028135/204923463-102baaad-c44c-4b9b-a6b3-3d872f16e63c.png)

For high ACE surface temperature anomalies, the surface temperatures are a little bit below average (when compared to just the monthly average of 6 months of data, which should be taken with a grain of salt or two), which does make sense sort of. Hurricanes can cause the SST to decrease as they move past because of the exchange of energy in the form of heat. So, as the tropical cyclone gains energy (and thus heat) from the ocean, the ocean slightly decreases in temperature.

![ace_ts_low_comp](https://user-images.githubusercontent.com/114028135/204923474-154e4556-5be9-40ef-b5ec-3b5f1e1d8698.png)

For low ACE surface temperature anomalies, the anomalies are near-normal, which would make sense theoretically, if following the previous argument.

![ace_precip_high_comp](https://user-images.githubusercontent.com/114028135/204925206-fcde7dde-dfd4-4db0-8939-9b63abc052fc.png)

For high ACE precipitation anomalies, we see a large area of above average precipitation in the Gulf of Mexico, near the Mississippi River Delta in August. 

In September, we see a large area of above average precipitation in the Gulf of Mexico, across the Strait of Florida, and around the Bahamas. Since these are the regions that are usually affected the most by hurricanes, it would make sense that there would be high precipitation anomalies here. 

In October, we see near-normal precipitation, indicating that, at least from 2011-2016, there wasn't a major increase or decrease in precipitation during months of high ACE. 

![ace_precip_low_comp](https://user-images.githubusercontent.com/114028135/204925212-2ee24b66-990d-4764-9f17-8b65f2b4ee64.png)

For low ACE precipitation anomalies, we see the exact opposite. 

In August, there is a relatively large anomaly in precipitation near the coastal regions of the East Coast.

In September, we see that anomaly slightly increase, and move a little bit toward the East, while the precipitation anomalies over land increase as well. Since September is a rainy season for much of the South East, this makes sense logically. In the frame of ACE, we could potentially interpret this as the cyclones losing energy as they move over land, and bringing with them precipitation. 

In October, we see near-normal precipitation, indicating that, at least from 2011-2016, there wasn't a major increase or decrease in preciptation during months of low ACE.

Inwe see a large area of above average precipitation in the Atlantic centered around 32N in September, and low within the Gulf. Since September is the month of peak hurricane activity, it would make sense that if the accumulated cyclone energy is high, the precipitation will be higher than average, to a certain extent.

![ace_z500_high_comp](https://user-images.githubusercontent.com/114028135/204925213-80ee6207-ba14-41d2-a846-e2f4f6b3d386.png)

For high ACE z500 anomalies, we see that the anomalies in height aren't that drastic, considering that the 500 hPa level can be within 4,000 to 6,000 m. If we only see variation between about 10 meters either higher or lower, that doesn't really tell us anything significant about the affect those anomalies could have in regards to high ACE values. 

![ace_z500_low_comp](https://user-images.githubusercontent.com/114028135/204925216-fc3a53c8-932e-449b-8d8b-afed36ad755b.png)

For low ACE z500 anomalies, we see again, the exact inverse of the previous plot. 

An error I encountered with HA that I did not have time to fix with ACE is that the low are the exact opposite of the high. With the HA index, I was able to solve this by manually aggregating the anomalies corresponding with the high and low activities, which involved having a average that was slightly below the average obtained with the .mean(dim='time') function. I did not do this for ACE. 
