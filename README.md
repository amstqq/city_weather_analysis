# Weather Analysis

This is a two-part project aiming to visualize global weather trend. The first part of the project uses OpenWeatherMap API, Python requests, and JSON traversals to obtain weather data about 500+ random cities across the globe and create a representative model of weather across world cities. The second part of the project is a visualization dashboard website built with bootstrap using models and analysis obtained from part I. The website will contain all visualizations along with their corresponding explanations as well as the data used to create these visualizations. 

## Python packages

These packages are required to run the jupyter notebook.
- matplotlib
- pandas
- numpy
- requests
- time
- citipy

## Instructions

WeatherPy jupyter notebook contains the code to obtain weather data across hundreds of cities, create visualizations, and output collected data into csv format. Before running the jupter notebook, sign up for a free account at [openweathermap.org](https://openweathermap.org/) and obtain an API key. Then, copy paste your API key into api_keys.py file under PART_I_api folder.
_Note: the code used to pull data from API (for loops) take a long time to run._

To see the website created for this project, navigate to PART_II_web folder and open index.html in your browser.
