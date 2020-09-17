# python-api-challenge
Week 6 / Python API Challenge

## WeatherPy
In this practice, we gathered data to prove how the weather had changed as we approach the equator, from both North and South Poles. The data was 500 randomly selected latitude  and longitude numbers, which we then used a citipy Python library to find the nearest cities to those randomly generated numbers. With these random numbers, we used a Weather API to generate temperatures, humidity, cloudiness, and windspeed from those locations. With this data, we were able showcase the relationship between latitude and temperature, humidity, cloudiness, and wind speed. To go into more details, we could also generate the difference between Northern and Southern Hemisphere and its effect with temperature, humidity, cloudiness, and wind speed in the form of scatterplots. All data has been exported to a CSV file and all scatterplots have been exported to images as well.

## VacationPy
With the CSV file from the previous practice, we used Google Places API to generate heatmaps of the locations gathered. First, in order to generate the data based on humidity, we had to clean the dataframe to drop any rows without full values. Then we can use the clean dataframe to plot the values of humidity across the map. Then, to generate the most ideal weather conditions, we dropped any values that did not have a max temperature falling between 70 and 80 degrees, with less that 10 mph wind speed, and zero cloudiness. With the new dataframe, we could use this to call Google APIs to find the nearest hotels within 5000 meters of the cities that met the previous weather conditions. Once found, we could plot these to the previous map.

## Three Observable Conclusions based on Data:
### 1. Cloudiness
![CityLatvsCloudiness](https://user-images.githubusercontent.com/65466578/93414030-1d4a9080-f866-11ea-862a-0982c894a258.png)

![NHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93414027-1d4a9080-f866-11ea-9c11-c6543a4b2d48.png)

![SHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93414025-1cb1fa00-f866-11ea-9534-ff9c54d671f4.png)

Between the North and South approaching the equator, the from the equator to the North seems to have little to no relationship on cloudiness, but there is more a distinct linear correlation when moving from the South to the equator. 

### 2. Temperatures
![CityLatvsMaxTemp](https://user-images.githubusercontent.com/65466578/93414075-34897e00-f866-11ea-89fa-89c241f42ab8.png)

As the cities move closer to the equator from both hemispheres, the maximum temperature tends to rise. There seems to be a greater correlation between how close the city is to the equator and its corresponding temperature. 

### 3. Wind Speed
![NHWindSpeedvsLatitude](https://user-images.githubusercontent.com/65466578/93414099-41a66d00-f866-11ea-874c-d87b840d2f8d.png)

![SHWindSpeedvsLatitude](https://user-images.githubusercontent.com/65466578/93414100-423f0380-f866-11ea-8599-9086b30e4685.png)

In regards to wind speed, in the Northern Hemisphere, there seems to be little effect on the latitudinal location and the corresponding windspeend. However, with the Southern Hemisphere, as the location gets closer to the equator, the wind speed seems to be greater. 

