# python-api-challenge
Week 6 / Python API Challenge

## WeatherPy
In this practice, we gathered data to prove how the weather had changed as we approach the equator, from both North and South Poles. The data was 500 randomly selected latitude  and longitude numbers, which we then used a citipy Python library to find the nearest cities to those randomly generated numbers. With these random numbers, we used a Weather API to generate temperatures, humidity, cloudiness, and windspeed from those locations. With this data, we were able showcase the relationship between latitude and temperature, humidity, cloudiness, and wind speed. To go into more details, we could also generate the difference between Northern and Southern Hemisphere and its effect with temperature, humidity, cloudiness, and wind speed in the form of scatterplots. All data has been exported to a CSV file and all scatterplots have been exported to images as well.

## VacationPy
With the CSV file from the previous practice, we used Google Places API to generate heatmaps of the locations gathered. First, in order to generate the data based on humidity, we had to clean the dataframe to drop any rows without full values. Then we can use the clean dataframe to plot the values of humidity across the map. Then, to generate the most ideal weather conditions, we dropped any values that did not have a max temperature falling between 70 and 80 degrees, with less that 10 mph wind speed, and zero cloudiness. With the new dataframe, we could use this to call Google APIs to find the nearest hotels within 5000 meters of the cities that met the previous weather conditions. Once found, we could plot these to the previous map.

## Three Observable Conclusions based on Data:
### 1. Cloudiness has no affect on the latitudinal location 
![SHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93274964-362d4600-f781-11ea-9468-c29f98bce462.png)

![NHCloudinessvsLatitude](https://user-images.githubusercontent.com/65466578/93274995-48a77f80-f781-11ea-9c4a-e9462e7e1435.png)

Based on both of these scatterplots, there is a very little change in cloudiness going from the South Pole to the equator, and also in the opposite direction. In the Northern Hemisphere to the equator, the linear regression has a very low slope value.

### 2. Temperatures and the Latitudinal Location do have a relationship
![CityLatvsMaxTemp](https://user-images.githubusercontent.com/65466578/93275160-c4093100-f781-11ea-8c47-b0de7f1de0dd.png)

As the cities move closer to the equator from both hemispheres, the maximum temperature tends to rise. There seems to be a greater correlation between how close the city is to the equator and its corresponding temperature. 
