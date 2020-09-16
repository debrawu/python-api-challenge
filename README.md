# python-api-challenge
Week 6 / Python API Challenge

## WeatherPy
In this practice, we gathered data to prove how the weather had changed as we approach the equator, from both North and South Poles. The data was 500 randomly selected latitude  and longitude numbers, which we then used a citipy Python library to find the nearest cities to those randomly generated numbers. With these random numbers, we used a Weather API to generate temperatures, humidity, cloudiness, and windspeed from those locations. With this data, we were able showcase the relationship between latitude and temperature, humidity, cloudiness, and wind speed. To go into more details, we could also generate the difference between Northern and Southern Hemisphere and its effect with temperature, humidity, cloudiness, and wind speed in the form of scatterplots. All data has been exported to a CSV file and all scatterplots have been exported to images as well.

## VacationPy
With the CSV file from the previous practice, we used Google Places API to generate heatmaps of the locations gathered. First, in order to generate the data based on humidity, we had to clean the dataframe to drop any rows without full values. Then we can use the clean dataframe to plot the values of humidity across the map. Then, to generate the most ideal weather conditions, we dropped any values that did not have a max temperature falling between 70 and 80 degrees, with less that 10 mph wind speed, and zero cloudiness. With the new dataframe, we could use this to call Google APIs to find the nearest hotels within 5000 meters of the cities that met the previous weather conditions. Once found, we could plot these to the previous map.

## Three Observable Conclusions based on Data:
### 1. Cloudiness
![SHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93403828-2d567600-f84e-11ea-8088-efbc3e144c70.png)

![NHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93403829-2def0c80-f84e-11ea-96c9-c27c5457a9b1.png)

Based on both of these scatterplots, it seems that when the cities get closer to the equator, the cloudier it becomes. This could also be due to the weather and currently it being a rainy season and hence, more clouds.

### 2. Temperatures
![CityLatvsMaxTemp](https://user-images.githubusercontent.com/65466578/93404001-af469f00-f84e-11ea-9bab-1582edb8d56b.png)

As the cities move closer to the equator from both hemispheres, the maximum temperature tends to rise. There seems to be a greater correlation between how close the city is to the equator and its corresponding temperature. 

### 3. Wind Speed
![SHWindSpeedvsLatitude](https://user-images.githubusercontent.com/65466578/93290114-9a620100-f7a5-11ea-8a01-2fcbcb873108.png)

![NHWindSpeedvsLatitude](https://user-images.githubusercontent.com/65466578/93290115-9afa9780-f7a5-11ea-97c8-61a003995728.png)

In regards to wind speed, in the Northern Hemisphere, there seems to be little effect on the latitudinal location and the corresponding windspeend. However, with the Southern Hemisphere, as the location gets closer to the equator, the wind speed seems to be greater. 

