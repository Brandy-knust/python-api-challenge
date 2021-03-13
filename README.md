# Python API Challenge
Homework for the API week using APIs and Python to pull data about the weather

![](https://github.com/Brandy-knust/python-api-challenge/blob/main/WeatherPy/figures/humidity_heat_map.png?raw=true)

## Weather Py

* In this activity, I used randomly selected 500+ lattitude and longitude locations, found the cities closest to those locations, and then made a dictionary of those cities and locations.
* I then used a weather API to pull weather data for current date and time for those selected cities, eliminating cities that had no current data.
* I then used that data to analyze current conditions around the globe to see if lattitude had effects on temperature, humidity, cloudiness, and wind speed.
* I created plots and linear regressions to show for each hemisphere how temperature, humidity, cloudiness, and wind speed were (or were not) related to lattitude.
* This shows the linear regression for the relationship between temperature in the Northern Hemisphere and the Lattitude. It shows that as you move further away from the equator, it gets colder, which is what you would expect. 

![](https://github.com/Brandy-knust/python-api-challenge/blob/main/WeatherPy/figures/NH_tempvlat.png?raw=true)

## Vacation Py

* In this activity, I used the csv file that was created from Weather Py, with all of the data for locations, cities, and all of the weather data to find an ideal vacation location. Keep in mind that this activity was done in early March, so it is the end of Winter for the Northern Hemisphere, and the end of Summer for the Southern Hemisphere.
* I started by using GMaps to create a heat map of the humidity for each of the locations from Weather Py. 
* After that, I created bins for each of the categories of temperature, wind speed, and cloudiness to find ideal weather conditions for a vacation. The parameters set were temperature between 70 and 80 degrees Fahrenheit, clear skies, and winds of less than 10 mph. 
* I further limited the locations in the end by humidity of less than 75% to limit the number of cities I would look for hotels in.
* I used the Google API to find hotel locations within 5000 meters of the latitude and longitude locations for each city, and plotted those on a map with markers of the hotel name, city name, and country name.

![](https://github.com/Brandy-knust/python-api-challenge/blob/main/WeatherPy/figures/Hotel_Locations.png?raw=true)

### Technologies used

* Python
* MatPlotLibs
* APIs
* GMaps
* Pandas
* SciPy