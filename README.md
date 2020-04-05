# World_Weather_Analysis
Module 6 of UofT Data Analytics Boot Camp

Code for Parts 1, 2, and 3 of the challenge.
1. Weather_Database.ipynb
2. Vacation_Search.ipynb
3. Vacation_Itinerary.ipynb

For Part 1, question "How many cities have recorded rainfall or snow?" is answered using the following Pandas methods.

```Python
snow_rain_city = city_data_df.loc[(city_data_df['Rain inches (last 3hrs)'] > 0) | (city_data_df['Snow inches (last 3hrs)'] > 0)]['City'].count()
rain_city = city_data_df.loc[(city_data_df['Rain inches (last 3hrs)'] > 0)]['City'].count()
snow_city = city_data_df.loc[(city_data_df['Snow inches (last 3hrs)'] > 0)]['City'].count()
print(f"{snow_rain_city} cities have recorded rainfall or snow (rain:{rain_city}, snow:{snow_city})")
```


A “data” folder containing the following CSV files.
1. WeatherPy_challenge.csv
2. WeatherPy_vacation.csv

An “image” folder containing the images of your maps for Parts 2 and 3.
1. WeatherPy_vacation_map.png
2. WeatherPy_travel_map.png
3. WeatherPy_travel_map_markers.png