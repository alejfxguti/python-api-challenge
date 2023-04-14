# python-api-challenge: WeatherPy and VacationPy
"What is the weather like as we approach the equator?"

## Overview
This project involves creating two Jupyter notebooks - WeatherPy and VacationPy. In WeatherPy, a Python script is used to visualize weather data of over 500 cities located at varying distances from the equator. The citipy Python library and the OpenWeatherMap API are used to create a representative model of weather across cities. In VacationPy, weather data skills are employed to plan future vacations using Jupyter notebooks, the GeoViews Python library, and the Geoapify API.

## Part 1: WeatherPy
In WeatherPy, the following requirements are fulfilled:

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude
- The OpenWeatherMap API is used to retrieve weather data from the cities list generated in the starter code.
- A series of scatter plots is created to showcase the following relationships:
    - Latitude vs. Temperature
    - Latitude vs. Humidity
    - Latitude vs. Cloudiness
    - Latitude vs. Wind Speed

### Requirement 2: Compute Linear Regression for Each Relationship
- Linear regression is computed for each relationship.
- The plots are separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).
- A function is defined to create the linear regression plots.
- A series of scatter plots is created with the linear regression line, the model's formula, and the r values.

## Part 2: VacationPy
In VacationPy, the following requirements are fulfilled:

### Step 1: Create a Humidity Heatmap
- A map is created that displays a point for every city in the city_data_df DataFrame.
- The size of the point is the humidity in each city.

### Step 2: Narrow Down the DataFrame
- The city_data_df DataFrame is narrowed down to find the ideal weather condition, for example:
    - A max temperature lower than 27 degrees but higher than 21
    - Wind speed less than 4.5 m/s
    - Zero cloudiness
- A reasonable limit is set to the number of rows returned by the API requests.

### Step 3: Find the Hotel
- A new DataFrame called hotel_df is created to store the city, country, coordinates, and humidity.
- For each city, the Geoapify API is used to find the first hotel located within 10,000 meters of the coordinates.
- The hotel name and the country are added as additional information in the hover message for each city on the map.

## Conclusion
This project provides an opportunity to apply Python coding skills to real-world scenarios. The use of various APIs and libraries makes it possible to visualize and analyze weather data to plan future vacations.
