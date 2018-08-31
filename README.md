# Weather Analysis

This project uses OpenWeatherMap API, Python requests, and JSON traversals to obtain weather data about 500+ random cities across the globe and create a representative model of weather trend. A visualization dashboard website is built with bootstrap using data collected from OpenWeatherMapAPI. The website contains all charts and graphs, explanations for weather trends, and data used to create the visualizations.

## Python packages

These packages are required to run the jupyter notebook.
- matplotlib
- pandas
- numpy
- requests
- time
- citipy

## Navigation

PART-I-api folder contains part 1 of the project. WeatherPy.ipynb has all the code for data collection and analysis. The img folder contains visualizations of weather data created using matplotlib. The output_data folder contains the data collected from OpenWeatherMap API.

PART-II-web folder contains html files for the visualization website. 

## Instructions

WeatherPy jupyter notebook contains the code to obtain weather data across hundreds of cities, create visualizations, and output collected data into csv format. Before running the jupter notebook, sign up for a free account at [openweathermap.org](https://openweathermap.org/) and obtain an API key. Then, copy paste your API key into api_keys.py file under PART_I_api folder.
_Note: the code used to pull data from API (for loops) take a long time to run._

To see the website created for this project, store the repository into local folder. Then, navigate to PART_II_web folder and open index.html in your browser.
