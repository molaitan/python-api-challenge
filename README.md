# python-api-challenge
Homework 6 Python API 

Consists of 2 parts- WeatherPy and VacationPy Analysis

## Background

Used Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

## 3 Observations

1. There is definetly a direct relationship between latitude location and maximum temperatures. The highest maximum temperatures are found near 0, concentrated between -20 and 20. This is due to the sun's direct angle at this part of the Earth. As the latitudes move away from 0, temperatures drop. 

2. There appears to be no direct relationship between latitude location and humidity, wind, and cloudiness. 
These weather conditions may be effected by other factors unrelated to latitude. All have r-values that point to weak or no correlations.

3. The northern hemisphere's correlation of latitude location and maximum temperates are stronger than that of the southern hemisphere. The southern hemisphere may not have this strong of a relationship due to there being more bodies of water and less land compared to the northern hemisphere. The large bodies of water may be factor in the varying temperatures.

## WeatherPy
Created a series of scatter plots to showcase relationships:

Temperature (F) vs. Latitude
![lat_vs_temp_plot](https://user-images.githubusercontent.com/94502554/154144382-9bae917f-4b6c-46ff-8ece-8e13575ea866.png)

Humidity (%) vs. Latitude
![lat_vs_humidity_plot](https://user-images.githubusercontent.com/94502554/154144442-649fb1b7-9d7a-410a-ab0a-9e3018f2e09a.png)

Cloudiness (%) vs. Latitude
![lat_vs_cloudiness_plot](https://user-images.githubusercontent.com/94502554/154144475-c1df10ce-e6a4-4431-8c74-85fb4f97f1e7.png)

Wind Speed (mph) vs. Latitude
![lat_vs_wind_plot](https://user-images.githubusercontent.com/94502554/154144418-c6ec4ec6-f100-4b72-ae8e-946492e6ef32.png)


Northern Hemisphere - Temperature (F) vs. Latitude
Southern Hemisphere - Temperature (F) vs. Latitude
![north_hem_temp_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144049-c63466f6-d06c-4ffa-9cb3-b99dcc04ccb2.png)
![south_hem_temp_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144002-37c8b2da-22c6-4ccd-bc7c-40990a6d9dfa.png)

Northern Hemisphere - Humidity (%) vs. Latitude
Southern Hemisphere - Humidity (%) vs. Latitude
![north_hem_humudity_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144172-94101cac-9422-45c9-bd72-a9ebe5ed8afc.png)
![south_hem_humudity_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144118-d2a25c1c-08fa-45e7-9b0e-10f4d042779e.png)


Northern Hemisphere - Cloudiness (%) vs. Latitude
Southern Hemisphere - Cloudiness (%) vs. Latitude
![north_hem_cloudiness_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144255-8b2b37c4-1de6-4ec9-9c17-84a33e2823c2.png)
![south_hem_cloudiness_v_lat_plot](https://user-images.githubusercontent.com/94502554/154144220-ca6dbab1-3c40-48da-903f-2d036043fee4.png)

## VacationPy
Used jupyter-gmap and the Google Places API to work with the weather data to plan future vacations.

Ideal weather conditions: 
-Max temperature lower than 80 degrees but higher than 70
-Wind speed less than 10 mph
-Zero cloudiness
-Drop any rows that don't contain all three conditions

6 hotels fit the ideal weather criteria and were the first hotels located within 5000 meters of the city's coordinates.

Created a heat map that displays the humidity for every city from Part I.
![heatmap](https://user-images.githubusercontent.com/94502554/154146342-a83490bb-2a63-4764-85c9-9aa5896e159b.png)


Plotted the hotels on top of the humidity heatmap with markers
![heatmapwithmarkers](https://user-images.githubusercontent.com/94502554/154146326-ab36e61b-aff5-4b1d-9cb3-a41173fd5cd8.png)
