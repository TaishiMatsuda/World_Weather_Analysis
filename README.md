# World_Weather_Analysis
Module 6 of UofT Data Analytics Boot Camp

## Python Code used for Parts 1, 2, and 3 of the challenge.
Part 1. Weather_Database.ipynb

Part 2. Vacation_Search.ipynb

Part 3. Vacation_Itinerary.ipynb

For Part 1, question "How many cities have recorded rainfall or snow?" was answered using the following Pandas methods.

```Python
snow_rain_city = city_data_df.loc[(city_data_df['Rain inches (last 3hrs)'] > 0) | (city_data_df['Snow inches (last 3hrs)'] > 0)]['City'].count()
rain_city = city_data_df.loc[(city_data_df['Rain inches (last 3hrs)'] > 0)]['City'].count()
snow_city = city_data_df.loc[(city_data_df['Snow inches (last 3hrs)'] > 0)]['City'].count()
print(f"{snow_rain_city} cities have recorded rainfall or snow (rain:{rain_city}, snow:{snow_city})")
```

For the DataFrame generated, the answer was 

"`80 cities have recorded rainfall or snow (rain:60, snow:20)`"

## CSV files generated
Part 1. WeatherPy_challenge.csv

Part 2. WeatherPy_vacation.csv

## Images of maps for Parts 2 and 3
Part 2. WeatherPy_vacation_map.png

Part 3. WeatherPy_travel_map.png & WeatherPy_travel_map_markers.png