Similar to how I determined the composites for hurricane activity, I did the same with ACE, pulling the years of highest ACE and lowest ACE and doing a composite of anomalies of precipitation, z500, and temperature corresponding to the highest and lowest ACE years.

![ace_ts_high_comp](https://user-images.githubusercontent.com/114028135/204923463-102baaad-c44c-4b9b-a6b3-3d872f16e63c.png)

For high ACE surface temperature anomalies, the surface temperatures are actually a little below average, which does not really make much sense, considering that high surface temperatures are what basically drive tropical cyclones.

![ace_ts_low_comp](https://user-images.githubusercontent.com/114028135/204923474-154e4556-5be9-40ef-b5ec-3b5f1e1d8698.png)

For low ACE surface temperature anomalies, the anomalies are slightly above average.

![ace_precip_high_comp](https://user-images.githubusercontent.com/114028135/204925206-fcde7dde-dfd4-4db0-8939-9b63abc052fc.png)

For high ACE precipitation anomalies, we see a large area of above average precipitation in September, and low within the Gulf. 

![ace_precip_low_comp](https://user-images.githubusercontent.com/114028135/204925212-2ee24b66-990d-4764-9f17-8b65f2b4ee64.png)

For low ACE precipitation anomalies, we see the exact opposite.

![ace_z500_high_comp](https://user-images.githubusercontent.com/114028135/204925213-80ee6207-ba14-41d2-a846-e2f4f6b3d386.png)

For high ACE z500, we see

![ace_z500_low_comp](https://user-images.githubusercontent.com/114028135/204925216-fc3a53c8-932e-449b-8d8b-afed36ad755b.png)

For low ACE z500, we see

An error I encountered with HA that I did not have time to fix with ACE is that the low are the exact opposite of the high. With the HA index, I was able to solve this by manually aggregating the anomalies corresponding with the high and low activities, which involved having a average that was slightly below the average obtained with the .mean(dim='time') function. I did not do this for ACE.
