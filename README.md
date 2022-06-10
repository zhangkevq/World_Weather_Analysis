# World Weather Analysis

## Using APIs for Vacation Plans

#### Goals
  The main goal of this project is to create a vacation itenerary based on weather patterns around the world using APIs. We will be looking for:
  1) The weather data around the world displayed in a figure layered over the map
  2) Hotels and cities randomly located around the world

### World Weather Patterns Layer and Map
  After getting a G-Maps API key and calling it into the notebook, we use Google Maps to create a DataFrame containing all city temperature, weather conditions, and their locations.
  
![WeatherPy Cities DF](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/cities_df_head.png)

After using the G-Maps API to plot these cities on the world map, we can generate the map of all cities found this way.

![WeatherPy Cities Map](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/all_df_cities.png)

### Creating the Travel Itinerary
  Next, we need to get hotels for all those cities, so we know where we can stay.
  
![WeatherPy Vacation DF](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/hotels_df_head.png)

The map for the hotels will include a layer that shows the temperature heatmap for the whole world. When clicking on any hotel point, you will be able to see the pop up info as well.

![hotels with temp heatmap](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/all_df_hotels.png)
![pop up info](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/WeatherPy_travel_map_markers.png)

Using the cities picked from the hotels DataFrame head, G Maps can try to create a travel roadmap from destination to destination if available. If no path is found, then an error will display.

![error attempt to find path, path not found](https://github.com/zhangkevq/World_Weather_Analysis/blob/main/Resources/gmaps_directions.png)

