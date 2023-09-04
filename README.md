# Final-Project-Statistical-Modelling-with-Python


## Project/Goals
Description: The project aims to analyze bike-sharing data from CityBikes and location-based data from Foursquare and Yelp to gain insights into the relationship between the availability of bikes in a particular location and the characteristics of points of interest (POIs) in that location. The project involves data collection, data integration, visualization, and regression modeling.

## Goals:

Part 1: Connecting to the CityBikes API and retrieving bike station data for a chosen city has been completed.
Part 2: Utilizing the Foursquare and Yelp APIs to gather information about restaurants, bars, and other POIs near each bike station has been completed.
Part 3: Joining the data from different sources to create a comprehensive dataset and exploring the data visually will be undertaken.
Part 4: Building a regression model to understand the relationship between bike availability and POI characteristics will be addressed.
Optionally, exploring the possibility of turning the regression problem into a classification one will be considered.

## Process
### (your step 1)
Part 1: Connecting to CityBikes API
The structure of the CityBikes API was explored.The code was setup to take user input as city name and return information about
the selected city. I chose Madrid as the city and all available bike stations, including their latitude, longitude, and the number of available bikes, were retrieved.
The JSON data file was subsequently parsed into a Pandas dataframe.

Part 2: Connecting to Foursquare and Yelp APIs
The DataFrame from part 1 was saved as a csv file and loaded into the DataFrame for analysis on the second part of the task.
Connections to the Foursquare and Yelp APIs were established.

### (your step 2)
For each bike station, queries to both APIs were been made to gather information about restaurants, bars, and other chosen POIs.
Separate dataframes for Yelp and Foursquare results have been created.
The quality and coverage of data from both APIs have been compared. 
## This was the most difficult task for me and took me almost 3 days as I had challenges in unpacking the nested json responses from the APIs.

Part 3: Joining Data (Future Step)
The data collected in Part 1 (bike station data) will be joined with the data from Part 2 (Yelp and Foursquare results).
Data visualization techniques will be used to explore the combined dataset.
An SQLite database will be created to store the collected POI data with careful consideration of the database structure.

Part 4: Building a Model (Future Step)
A regression model will be built using Python's statsmodels to analyze the relationship between bike availability and POI characteristics.
The results of the regression model will be interpreted.
Optionally, exploration of how to turn the regression problem into a classification problem will be considered.


## Results
I have found that both the Foursquare and Yelp APIs provide valuable data for various purposes. The choice of which one to use depends on your specific needs and the type of data you require. 

The Yelp API has been particularly helpful for me. It provided me with information primarily related to businesses and places, with a strong focus on user-generated reviews and ratings. This includes detailed information about businesses such as their names, addresses, contact details, ratings, reviews, and categories. It has proven to be very useful when I needed to analyze and compare user opinions, ratings, and reviews about restaurants, bars, and other businesses. I've found it to be more suitable for applications related to the hospitality and food service industry.

On the other hand, the Foursquare API has also been quite valuable in my work. It offers a broader range of location-based data and insights beyond just businesses and places. In addition to business details, Foursquare has provided me with data related to check-ins, user-generated tips, user profiles, and location trends. This extensive dataset has been instrumental in exploring user behavior, tracking trends in check-in activity, and understanding user preferences in a more general sense. It's a versatile choice for applications that require a deeper understanding of user engagement and location-based behavior.

In summary, if you primarily need detailed information about businesses, their ratings, and reviews, the Yelp API may be more suitable for your needs. On the other hand, if you're interested in a broader range of location-based data, including user activity and trends, the Foursquare API can provide valuable insights. Your choice should align with your specific analytical goals and the type of data that best serves your analysis."

## Challenges 
My major challenge really was unpacking the nested json responses from the API.

## Future Goals
Given more time, we would consider the following:

Conducting a more extensive analysis with larger datasets to further assess the strengths and weaknesses of each API.
Exploring additional data sources and APIs to enrich the location-based insights.
Developing a model or recommendation system based on the combined data from multiple sources to improve the accuracy of location-based recommendations.
This project lays the foundation for more in-depth research and application development in the field of location-based data analysis and user behavior modeling.