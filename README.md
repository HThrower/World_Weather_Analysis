# World_Weather_Analysis
* Task: Collect and analyze weather data across cities worldwide.
* Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
## Retrieve Weather Data
Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

1) Create a new set of 2,000 random latitudes and longitudes.
2) Perform an API call with the OpenWeatherMap.
3) Retrieve the following information from the API call:

  * Latitude and longitude
  * Maximum temperature
  * Percent humidity
  * Percent cloudiness
  * Wind speed
  * Weather description (for example, clouds, fog, light rain, clear sky)
  
## Create a Customer Travel Destinations Map
Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

  1) Retrieve the latitude and longitude of each city to find the nearest hotel based on the search parameters from Step 6a, then add the          hotel name
  2) Add the city name, the country code, the weather description, and the maximum temperature for the city
  3) A marker layer map with pop-up markers for the cities in the vacation DataFrame
 
    * Hotel name
    * City
    * Country
    * Current weather description with the maximum temperature
 
## Create a Travel Itinerary Map
  Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.
  
  1) iterate through the hotel_df DataFrame, retrieve the latitude and longitude of each city to find the nearest hotel based on the search parameters from Step 6a, then add the hotel name to the hotel_df DataFrame. If a hotel isn't found, skip to the next city.
  2) use the provided list comprehension code to retrieve the city data from each row, which will then be added to the formatting template 
