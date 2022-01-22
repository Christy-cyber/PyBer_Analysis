# PyBer Ride Share Analysis
## Overview and Metrics
Data from 2019 were analyzed for PyBer, a ride sharing company, in order to develop recommendations regarding access to ride share services for each city type (urban, suburban, and rural) and affordability of ride share services for underserved neighborhoods.  The following metrics were requested:
  - average fare cost by total rides per city, highlighting city type
  - average fare per driver
  - number of riders per city type 
  - amount of fare cost per city type
  - number of drivers per city type 
  - percentage of total fares per city type 
  - percentage of rides per city type 
  - percentage of drivers per city type 
  - weekly total fares from January through April 2019 per city type   


## Resources
- Data Sources: city_data.csv, ride_data.csv
- Software and Programming Languages: Jupyter Notebook v. 6.4.6; Python v. 3.8.3 :: Anaconda, Inc.; conda v. 4.11.0; Matplotlib v. 3.5.0

## Results
  - **Average fare cost and average fare per driver by total rides per city:**  There is an inverse relationship between total number of rides and average fare cost.  Urban cities have the greatest number of rides (1,625) but have the lowest average fare per ride ($24.53) and lowest average fare per driver ($16.57) when compared to rural cities that have the fewest rides (125) with the highest average fare per ride ($34.62) and highest average fare per driver ($55.49).  Fare cost and number of rides for suburban cities fall between the other two city types.  Additionally, the greatest number of drivers are found in urban areas (2,405), followed by suburban (490) and then rural cities (78).  Urban cities are responsible for approximately ten times more revenue than that of rural cities.  Rural and suburban cities have more rides than drivers, whereas urban cities have more drivers than rides (Table 1, Fig. 1).


Table 1. Summary of ride share data per city type.

![Summary Data Frame for ride share data](https://user-images.githubusercontent.com/95387273/150563147-a7919a17-2940-4f07-a40b-eec0cccb4a60.png)


Fig 1. Average fare cost by total number of rides per city.  Circle size correlates to the number of drivers per city.

![Fig1](https://user-images.githubusercontent.com/95387273/150434172-9a7b218f-b10f-45a1-8e08-dba052291994.png)

  - **Number of rides per city type:**  Urban cities had the highest *median* number rides at 24.  This was followed by 17 rides in suburban cities and 6 rides in rural cities.  A single city, West Angela, has the highest ride count of 39 (Fig. 2). 

Fig 2. Box plots indicating *median* number of rides per city, as well as 25th and 75th percentiles.
 
![Fig2](https://user-images.githubusercontent.com/95387273/150434203-d4a8a765-9902-4079-8cb6-fef22665092b.png)

  - **Fare cost per city type:**  Urban cities had the lowest *median* fare cost that approximated $25.00 per fare.  This was followed by ~$31.00 fares in suburban cities and ~$37.00 fares in rural areas (Fig. 3).

Fig 3. Box plots indicating *median* amount of fare cost per city type, as well as 25th and 75th percentiles.

![Fig3](https://user-images.githubusercontent.com/95387273/150434222-cabc0aa4-d1cf-4093-b85a-43a33b393c0c.png)

  - **Number of drivers per city type:**  Urban cities had the highest *median* number of drivers (37), followed by suburban cities (16), and rural cities (4).  There is a higher spread in the number of drivers in urban cities as is indicated by the standard deviation (Fig. 4).

Fig 4.  Box plots indicating *median* number of drivers per city type, as well as 25th and 75 percentiles.
 
![Fig4](https://user-images.githubusercontent.com/95387273/150434235-e7c58e0c-0049-4452-82d4-fafd5bb3ce60.png)

  - **Percentage of total fares per city type:** Urban cities had the highest percentage of total fares (62.7%), followed by suburban cities (30.5%), and rural cities (6.8%) (Fig. 5).

Fig 5.  Pie chart indicating % of total fares by city type.
 
![Fig5](https://user-images.githubusercontent.com/95387273/150434253-205a5f36-87e6-487c-b782-929a016db964.png)

  - **Percentage of rides per city type:**  Urban cities had the highest percentage of total rides (68.4%), followed by suburban cities (26.3%), and rural cities (5.3%) (Fig. 6).

Fig 6.  Pie chart indicating % of total rides by city type.

![Fig6](https://user-images.githubusercontent.com/95387273/150434274-d1be0bdb-5ab0-4810-8520-f38d35e4678c.png)

 - **Percentage of drivers by city type:**  Urban cities had the highest percentage of total drivers (80.9%), followed by suburban cities (16.5), and rural cities (2.6%) (Fig. 7.)

Fig 7.  Pie chart indicating % of total drivers by city type.

![Fig7](https://user-images.githubusercontent.com/95387273/150434281-3b4a6cdc-5651-48a9-83a7-211f1f4ad178.png)


  - **Weekly total fares from January through April 2019 per city type:**  Urban cities consistently outperformed suburban cities by nearly four times and rural cities by nearly ten times with respect to total fares each week from January through April 2019, with the exception of the first week of April.  This may be due to a weather event.

Fig 8.  Total fare amounts per week in $USD by city type from January through April 2019. 


![Fig8](https://user-images.githubusercontent.com/95387273/150434304-cffa52e2-0d99-4045-bb22-ca0d91f66d4a.png)


## Summary
It is expected that urban cities would have higher revenue, numbers of drivers, and numbers and rides when compared to suburban and rural cities given differences in population sizes of the three city types. 

### Limitations of the Data
The data do not include information for mileage for each rider.  Calculations performed for fares were made per ride and per driver.  It is expected that individuals in urban areas are most likely taking shorter rides, so their rider fares would naturally be less than an individual who lives in a rural area who would be more likely to take longer rides to get to their destination.  The fare cost of the rural rider is naturally going to be higher because of the implied distance of their trip, even though this could not be measured in this analysis. Any decisions based on average fare cost should be delayed until mileage data can be obtained.  This will show the true average fare cost per unit distance between the three city types.

### Recommendations
  1) Obtain mileage data for each rider.  This will determine whether or not rural riders (all riders) are being overcharged based on trip distance.
  2) Increase the number of drivers in West Angela.  This urban city has the highest number of rides as well as a high number of drivers.  The city can support an increase in the number of drivers based on ride count.
  3) Decrease the number of drivers in urban areas where there are higher numbers of drivers.  There are more drivers than there are rides in urban cities, so not all of the drivers are necessary.



