# World Weather Analysis

## Overview of Project

The purpose of this project is to create a program that will allow a user to get a list of potential vacation destinations based on a preferred temperature range. Once destinations are chosen, Google Maps API is leveraged to obtain lodging and travel route between destinations.

## Summary of Project

### 1. Generating Potential Destinations

This project uses the Python module CityPy to acquire the closest city to a latitude-longitude pair (credit to Winston Chen - https://github.com/wingchen/citipy).

### 2. Retrieving Current Weather

Cities retrieved using CityPy are then passed to the OpenWeatherMap API (https://openweathermap.org/api) to gather current weather data.

### 3. User Input and Google Maps

User enters the upper and lower bound of their preferred temperature range. The DataFrame generated using the retrieved weather data is then filtered by user's preferences. Lat-Lon pairs for filtered cities are then passed to Google Maps API to retrieve lodging for each city and return a map with markers. User picks destinations.

![destinations](https://github.com/cdeanatx/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### 4. Google Directions

Once user chooses vacation destinations, Google API is leveraged to provide directions to each location using user's preferred method of travel (driving, bicycling, walking).

![directions](https://github.com/cdeanatx/World_Weather_Analysis/blob/main/Vacation_Itenerary/WeatherPy_travel_map.png)